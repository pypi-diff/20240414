# Comparing `tmp/pyreqwest_impersonate-0.1.1.tar.gz` & `tmp/pyreqwest_impersonate-0.1.2.tar.gz`

## Comparing `pyreqwest_impersonate-0.1.1.tar` & `pyreqwest_impersonate-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     5305 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/.gitignore
--rw-r--r--   0     1001      127     1850 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/README.md
--rw-r--r--   0     1001      127     5116 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127      341 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/tests/test_client.py
--rw-r--r--   0     1001      127    40959 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127     1073 2024-04-13 00:04:30.000000 pyreqwest_impersonate-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     5415 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/.gitignore
+-rw-r--r--   0     1001      127     2756 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/README.md
+-rw-r--r--   0     1001      127     8855 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127      854 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/tests/test_client.py
+-rw-r--r--   0     1001      127    46489 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127     1067 2024-04-13 23:30:52.000000 pyreqwest_impersonate-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3758 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.2/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.1.1/Cargo.toml` & `pyreqwest_impersonate-0.1.2/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
-description = "HTTP requests with impersonating web browsers. Impersonate browsers headers, `TLS/JA3` and `HTTP/2` fingerprints."
+description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pyreqwest_impersonate"
 crate-type = ["cdylib"]
@@ -14,18 +14,20 @@
 [dependencies]
 pyo3 = { version = "0.21", features = ["extension-module"] }
 reqwest-impersonate = { version = "0.11", default-features = false, features = [
     "cookies",
     "blocking",
     "boring-tls",
     "impersonate",
+    "trust-dns",  # async resolver instead of a default threadpool using `getaddrinfo`
     "socks",
     "gzip",
     "brotli",
     "deflate",
 ] }
-# bindgen = { version = "0.69", default-features = false, features = ["runtime"] }
 
 [profile.release]
-strip = true
-lto = true
 codegen-units = 1
+lto = "fat"
+opt-level = 3
+panic = "abort"
+strip = "symbols"
```

### Comparing `pyreqwest_impersonate-0.1.1/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.1.2/.github/workflows/CI.yml`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         with:
           name: wheels-linux-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
         shell: bash
         run: |
           set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pyreqwest_impersonate --find-links dist --no-index --force-reinstall
           pip install pytest
           pytest
 
   linux_aarch64:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
@@ -76,18 +76,19 @@
           CFLAGS_aarch64_unknown_linux_gnu: "-D__ARM_ARCH=8"
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-linux-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
+        if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pyreqwest_impersonate --find-links dist --no-index --force-reinstall
           pip install pytest
           pytest
 
   windows:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
@@ -114,15 +115,15 @@
           name: wheels-windows-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pyreqwest_impersonate --find-links dist --no-index --force-reinstall
           pip install pytest
           pytest
 
   macos:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
@@ -148,15 +149,15 @@
           name: wheels-macos-${{ matrix.platform.target }}-python${{ matrix.python-version }}
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pyreqwest_impersonate --find-links dist --no-index --force-reinstall
           pip install pytest
           pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
```

### Comparing `pyreqwest_impersonate-0.1.1/.gitignore` & `pyreqwest_impersonate-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.1/src/lib.rs` & `pyreqwest_impersonate-0.1.2/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use pyo3::exceptions;
 use pyo3::prelude::*;
+use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
+use reqwest_impersonate::redirect::Policy;
 use reqwest_impersonate::Method;
 use std::collections::HashMap;
 use std::str::FromStr;
 use std::time::Duration;
 
 #[pyclass]
 struct Response {
@@ -17,84 +19,152 @@
     #[pyo3(get)]
     text: String,
     #[pyo3(get)]
     url: String,
 }
 
 #[pyclass]
-/// A client for making HTTP requests with specific configurations.
-///
-/// This class allows for making HTTP requests with customizable timeout, proxy, and impersonation settings.
-/// It is designed to be used in scenarios where you need to make HTTP requests that mimic the behavior of a specific browser or entity.
+/// A blocking HTTP client that can impersonate web browsers.
 struct Client {
     client: reqwest_impersonate::blocking::Client,
 }
 
 #[pymethods]
 impl Client {
     #[new]
-    /// Creates a new `Client` instance with the specified configurations.
+    /// Initializes a blocking HTTP client that can impersonate web browsers.
     ///
-    /// Args:
-    ///     timeout (float, optional): The timeout for the HTTP requests in seconds. Default is None.
-    ///     proxy (str, optional): The proxy URL to use for the HTTP requests. Default is None.
-    ///     impersonate (str, optional): The identifier for the entity to impersonate. Default is None.
-    fn new(timeout: Option<f64>, proxy: Option<&str>, impersonate: Option<&str>) -> PyResult<Self> {
+    /// This function creates a new instance of a blocking HTTP client that can impersonate various web browsers.
+    /// It allows for customization of headers, proxy settings, timeout, impersonation type, SSL certificate verification,
+    /// and HTTP version preferences.
+    ///
+    /// # Arguments
+    ///
+    /// * `headers` - An optional map of HTTP headers to send with requests. If `impersonate` is set, this will be ignored.
+    /// * `proxy` - An optional proxy URL for HTTP requests.
+    /// * `timeout` - An optional timeout for HTTP requests in seconds.
+    /// * `impersonate` - An optional entity to impersonate. Supported browsers and versions include Chrome, Safari, OkHttp, and Edge.
+    /// * `redirects` - An optional number of redirects to follow. If set to 0, no redirects will be followed. Default is 10.
+    /// * `verify` - An optional boolean indicating whether to verify SSL certificates. Default is `true`.
+    /// * `http1` - An optional boolean indicating whether to use only HTTP/1.1. Default is `false`.
+    /// * `http2` - An optional boolean indicating whether to use only HTTP/2. Default is `false`.
+    ///
+    /// # Example
+    ///
+    /// ```
+    /// from reqwest_impersonate import Client
+    ///
+    /// client = Client(
+    ///     headers={"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.150 Safari/537.36"},
+    ///     proxy="http://127.0.0.1:8080",
+    ///     timeout=10,
+    ///     impersonate="chrome_123",
+    ///     redirects=0,
+    ///     verify=False,
+    ///     http1=True,
+    ///     http2=False,
+    /// )
+    /// ```
+    fn new(
+        headers: Option<HashMap<String, String>>,
+        proxy: Option<&str>,
+        timeout: Option<f64>,
+        impersonate: Option<&str>,
+        redirects: Option<usize>,
+        verify: Option<bool>,
+        http1: Option<bool>,
+        http2: Option<bool>,
+    ) -> PyResult<Self> {
         let mut client_builder = reqwest_impersonate::blocking::Client::builder()
-            .danger_accept_invalid_certs(true)
             .enable_ech_grease(true)
             .permute_extensions(true)
             .cookie_store(true)
+            .trust_dns(true)
             .timeout(timeout.map(Duration::from_secs_f64));
 
+        if let Some(headers) = headers {
+            let mut headers_new = HeaderMap::new();
+            for (key, value) in headers {
+                headers_new.insert(
+                    HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
+                        PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
+                    })?,
+                    HeaderValue::from_str(&value).map_err(|_| {
+                        PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
+                    })?,
+                );
+            }
+            client_builder = client_builder.default_headers(headers_new);
+        }
+
+        if let Some(proxy_url) = proxy {
+            let proxy = reqwest_impersonate::Proxy::all(proxy_url)
+                .map_err(|_| PyErr::new::<exceptions::PyValueError, _>("Invalid proxy URL"))?;
+            client_builder = client_builder.proxy(proxy);
+        }
+
         if let Some(impersonation_type) = impersonate {
             let impersonation = Impersonate::from_str(impersonation_type).map_err(|_| {
                 PyErr::new::<exceptions::PyValueError, _>("Invalid impersonate param")
             })?;
             client_builder = client_builder.impersonate(impersonation);
         }
 
-        if let Some(proxy_url) = proxy {
-            let proxy = reqwest_impersonate::Proxy::all(proxy_url)
-                .map_err(|_| PyErr::new::<exceptions::PyValueError, _>("Invalid proxy URL"))?;
-            client_builder = client_builder.proxy(proxy);
+        match redirects {
+            Some(0) => client_builder = client_builder.redirect(Policy::none()),
+            Some(n) => client_builder = client_builder.redirect(Policy::limited(n)),
+            None => client_builder = client_builder.redirect(Policy::limited(10)), // default to 10 redirects
+        }
+
+        if let Some(verify) = verify {
+            if !verify {
+                client_builder = client_builder.danger_accept_invalid_certs(true);
+            }
+        }
+
+        match (http1, http2) {
+            (Some(true), Some(true)) => {
+                return Err(PyErr::new::<exceptions::PyValueError, _>(
+                    "Both http1 and http2 cannot be true",
+                ));
+            }
+            (Some(true), _) => client_builder = client_builder.http1_only(),
+            (_, Some(true)) => client_builder = client_builder.http2_prior_knowledge(),
+            _ => (),
         }
 
         let client = client_builder
             .build()
             .map_err(|_| PyErr::new::<exceptions::PyValueError, _>("Failed to build client"))?;
 
         Ok(Client { client })
     }
 
-    ///
     /// This method constructs an HTTP request with the given method and URL, and optionally sets a timeout.
     /// It then sends the request and returns a `Response` object containing the server's response.
     ///
     /// Args:
     ///     method (str): The HTTP method to use (e.g., "GET", "POST").
     ///     url (str): The URL to which the request will be made.
-    ///     timeout (float, optional): The timeout for the request in seconds. Default is None.
+    ///     timeout (float, optional): The timeout for the request in seconds. Default is 30.
     ///
     /// Returns:
     ///     Response: A response object containing the server's response to the request.
     ///
     /// Raises:
     ///     PyException: If there is an error making the request.
     fn request(&self, method: &str, url: &str, timeout: Option<f64>) -> PyResult<Response> {
         let method = match method {
             "GET" => Ok(Method::GET),
             "POST" => Ok(Method::POST),
-            "PUT" => Ok(Method::PUT),
-            "DELETE" => Ok(Method::DELETE),
             "HEAD" => Ok(Method::HEAD),
             "OPTIONS" => Ok(Method::OPTIONS),
-            "CONNECT" => Ok(Method::CONNECT),
-            "TRACE" => Ok(Method::TRACE),
+            "PUT" => Ok(Method::PUT),
             "PATCH" => Ok(Method::PATCH),
+            "DELETE" => Ok(Method::DELETE),
             &_ => Err(PyErr::new::<exceptions::PyException, _>(
                 "Unrecognized HTTP method",
             )),
         };
         let method = method?;
         let request_builder = match timeout {
             Some(timeout_seconds) => {
@@ -123,14 +193,42 @@
             cookies,
             headers,
             status_code,
             text,
             url,
         })
     }
+
+    fn get(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("GET", url, timeout)
+    }
+
+    fn post(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("POST", url, timeout)
+    }
+
+    fn head(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("HEAD", url, timeout)
+    }
+
+    fn options(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("OPTIONS", url, timeout)
+    }
+
+    fn put(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("PUT", url, timeout)
+    }
+
+    fn patch(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("PATCH", url, timeout)
+    }
+
+    fn delete(&self, url: &str, timeout: Option<f64>) -> PyResult<Response> {
+        self.request("DELETE", url, timeout)
+    }
 }
 
 #[pymodule]
 fn pyreqwest_impersonate(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<Client>()?;
     Ok(())
 }
```

### Comparing `pyreqwest_impersonate-0.1.1/Cargo.lock` & `pyreqwest_impersonate-0.1.2/Cargo.lock`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,25 @@
  "futures-core",
  "memchr",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
+name = "async-trait"
+version = "0.1.80"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
@@ -290,38 +301,56 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "data-encoding"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
+
+[[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "enum-as-inner"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
+dependencies = [
+ "heck",
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "flate2"
@@ -420,14 +449,25 @@
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
+name = "getrandom"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "glob"
@@ -469,14 +509,25 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
+name = "hostname"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c731c3e10504cc8ed35cfe2f1db4c9274c3d35fa486e3b31df46f068ef3e867"
+dependencies = [
+ "libc",
+ "match_cfg",
+ "winapi",
+]
+
+[[package]]
 name = "http"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
@@ -555,14 +606,24 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "idna"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+dependencies = [
+ "unicode-bidi",
+ "unicode-normalization",
+]
+
+[[package]]
+name = "idna"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
@@ -580,14 +641,26 @@
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
+name = "ipconfig"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b58db92f96b720de98181bbbe63c831e87005ab460c1bf306eb2622b4707997f"
+dependencies = [
+ "socket2",
+ "widestring",
+ "windows-sys 0.48.0",
+ "winreg",
+]
+
+[[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itertools"
@@ -634,15 +707,15 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
@@ -669,14 +742,29 @@
 [[package]]
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
+name = "lru-cache"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "31e24f1ad8321ca0e8a1e0ac13f23cb668e6f5466c2c57319f6a5cf1cc8e3b1c"
+dependencies = [
+ "linked-hash-map",
+]
+
+[[package]]
+name = "match_cfg"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ffbee8634e0d45d258acb448e7eaab3fce7a0a467395d4d9f228e3c1f01fb2e4"
+
+[[package]]
 name = "memchr"
 version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
@@ -810,14 +898,20 @@
 [[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
+name = "ppv-lite86"
+version = "0.2.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
@@ -899,30 +993,66 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
  "reqwest-impersonate",
 ]
 
 [[package]]
+name = "quick-error"
+version = "1.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
+
+[[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rand"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34af8d1a0e25924bc5b7c43c079c942339d8f0a8b57c39049bef581b46327404"
+dependencies = [
+ "libc",
+ "rand_chacha",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_chacha"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6c10a63a0fa32252be49d21e7709d4d4baf8d231c2dbce1eaa8141b9b127d88"
+dependencies = [
+ "ppv-lite86",
+ "rand_core",
+]
+
+[[package]]
+name = "rand_core"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
+dependencies = [
+ "getrandom",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
@@ -990,22 +1120,33 @@
  "serde_urlencoded",
  "system-configuration",
  "tokio",
  "tokio-boring-imp",
  "tokio-socks",
  "tokio-util",
  "tower-service",
+ "trust-dns-resolver",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
+name = "resolv-conf"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "52e44394d2086d010551b14b53b1f24e31647570cd1deb0379e2c21b329aba00"
+dependencies = [
+ "hostname",
+ "quick-error",
+]
+
+[[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc-hash"
@@ -1271,27 +1412,85 @@
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
  "pin-project-lite",
+ "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
+name = "tracing-attributes"
+version = "0.1.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
+name = "trust-dns-proto"
+version = "0.23.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3119112651c157f4488931a01e586aa459736e9d6046d3bd9105ffb69352d374"
+dependencies = [
+ "async-trait",
+ "cfg-if",
+ "data-encoding",
+ "enum-as-inner",
+ "futures-channel",
+ "futures-io",
+ "futures-util",
+ "idna 0.4.0",
+ "ipnet",
+ "once_cell",
+ "rand",
+ "smallvec",
+ "thiserror",
+ "tinyvec",
+ "tokio",
+ "tracing",
+ "url",
+]
+
+[[package]]
+name = "trust-dns-resolver"
+version = "0.23.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "10a3e6c3aff1718b3c73e395d1f35202ba2ffa847c6a62eea0db8fb4cfe30be6"
+dependencies = [
+ "cfg-if",
+ "futures-util",
+ "ipconfig",
+ "lru-cache",
+ "once_cell",
+ "parking_lot",
+ "rand",
+ "resolv-conf",
+ "smallvec",
+ "thiserror",
+ "tokio",
+ "tracing",
+ "trust-dns-proto",
+]
+
+[[package]]
 name = "try-lock"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "unicode-bidi"
@@ -1425,14 +1624,42 @@
 checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "widestring"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7219d36b6eac893fa81e84ebe06485e7dcbb616177469b142df14f1f4deb1311"
+
+[[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.5",
 ]
```

### Comparing `pyreqwest_impersonate-0.1.1/pyproject.toml` & `pyreqwest_impersonate-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pyreqwest_impersonate"
-description = "HTTP requests with impersonating web browsers. Impersonate browsers headers, `TLS/JA3` and `HTTP/2` fingerprints."
+description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["python", "request", "impersonate"]
 authors = [
   {name = "deedy5"}
 ]
 classifiers = [
```

