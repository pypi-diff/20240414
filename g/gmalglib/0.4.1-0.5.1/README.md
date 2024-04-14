# Comparing `tmp/gmalglib-0.4.1.tar.gz` & `tmp/gmalglib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.4.1.tar", last modified: Fri Apr 12 17:26:29 2024, max compression
+gzip compressed data, was "gmalglib-0.5.1.tar", last modified: Sun Apr 14 09:56:57 2024, max compression
```

## Comparing `gmalglib-0.4.1.tar` & `gmalglib-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.097212 gmalglib-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-12 17:26:23.000000 gmalglib-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 17:26:29.097212 gmalglib-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:26:23.000000 gmalglib-0.4.1/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:26:23.000000 gmalglib-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.089212 gmalglib-0.4.1/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.093212 gmalglib-0.4.1/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 17:26:23.000000 gmalglib-0.4.1/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-12 17:26:23.000000 gmalglib-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:26:29.097212 gmalglib-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-12 17:26:23.000000 gmalglib-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.089212 gmalglib-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.093212 gmalglib-0.4.1/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.097212 gmalglib-0.4.1/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    19150 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    29971 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 17:26:23.000000 gmalglib-0.4.1/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:26:29.097212 gmalglib-0.4.1/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 17:26:29.000000 gmalglib-0.4.1/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 09:56:49.000000 gmalglib-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 09:56:57.068384 gmalglib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-14 09:56:49.000000 gmalglib-0.5.1/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-14 09:56:49.000000 gmalglib-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.060384 gmalglib-0.5.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.064384 gmalglib-0.5.1/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 09:56:49.000000 gmalglib-0.5.1/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-14 09:56:49.000000 gmalglib-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:56:57.068384 gmalglib-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 09:56:49.000000 gmalglib-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.060384 gmalglib-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33914 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 09:56:49.000000 gmalglib-0.5.1/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:56:57.068384 gmalglib-0.5.1/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:56:57.000000 gmalglib-0.5.1/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.4.1/LICENSE` & `gmalglib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/include/gmalglib/bignum.h` & `gmalglib-0.5.1/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/include/gmalglib/random.h` & `gmalglib-0.5.1/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/include/gmalglib/sm2.h` & `gmalglib-0.5.1/include/gmalglib/sm2.h`

 * *Files 8% similar despite different names*

```diff
@@ -3,42 +3,47 @@
 
 #include <stdint.h>
 #include <gmalglib/bignum.h>
 #include <gmalglib/random.h>
 #include <gmalglib/sm2curve.h>
 #include <gmalglib/sm3.h>
 
-#define SM2_DEFAULT_UID_LENGTH                  16
-#define SM2_UID_MAX_LENGTH                      8191  // (0xFFFF >> 3)
-#define SM2_ENTITYINFO_LENGTH                   SM3_DIGEST_LENGTH
-
-#define SM2_SK_LENGTH                           SM2_PARAMS_LENGTH
-#define SM2_PK_HALF_LENGTH                      SM2_POINTBYTES_HALF_LENGTH
-#define SM2_PK_FULL_LENGTH                      SM2_POINTBYTES_FULL_LENGTH
-#define SM2_GET_PK_LENGTH(pc_mode)              SM2_GET_POINTBYTES_LENGTH(pc_mode)
-
-#define SM2_MSG_MAX_LENGTH                      ((SM3_MAX_MSG_BITLEN >> 3) - SM2_ENTITYINFO_LENGTH)
-#define SM2_SIGN_R_LENGTH                       SM2_PARAMS_LENGTH
-#define SM2_SIGN_S_LENGTH                       SM2_PARAMS_LENGTH
-#define SM2_SIGNATURE_LENGTH                    (SM2_SIGN_R_LENGTH + SM2_SIGN_S_LENGTH)
-
-#define SM2_ENCRYPT_C1_HALF_LENGTH              SM2_POINTBYTES_HALF_LENGTH
-#define SM2_ENCRYPT_C1_FULL_LENGTH              SM2_POINTBYTES_FULL_LENGTH
-#define SM2_GET_ENCRYPT_C1_LENGTH(pc_mode)      SM2_GET_POINTBYTES_LENGTH(pc_mode)
-#define SM2_ENCRYPT_C3_LENGTH                   SM3_DIGEST_LENGTH
-
+#define SM2_DEFAULT_UID_LENGTH                      16
+#define SM2_UID_MAX_LENGTH                          8191  // (0xFFFF >> 3)
+#define SM2_ENTITYINFO_LENGTH                       SM3_DIGEST_LENGTH
+
+#define SM2_SK_LENGTH                               SM2_PARAMS_LENGTH
+#define SM2_PK_HALF_LENGTH                          SM2_POINTBYTES_HALF_LENGTH
+#define SM2_PK_FULL_LENGTH                          SM2_POINTBYTES_FULL_LENGTH
+#define SM2_GET_PK_LENGTH(pc_mode)                  SM2_GET_POINTBYTES_LENGTH(pc_mode)
+
+#define SM2_MSG_MAX_LENGTH                          ((SM3_MAX_MSG_BITLEN >> 3) - SM2_ENTITYINFO_LENGTH)
+#define SM2_SIGN_R_LENGTH                           SM2_PARAMS_LENGTH
+#define SM2_SIGN_S_LENGTH                           SM2_PARAMS_LENGTH
+#define SM2_SIGNATURE_LENGTH                        (SM2_SIGN_R_LENGTH + SM2_SIGN_S_LENGTH)
+
+#define SM2_ENCRYPT_C1_HALF_LENGTH                  SM2_POINTBYTES_HALF_LENGTH
+#define SM2_ENCRYPT_C1_FULL_LENGTH                  SM2_POINTBYTES_FULL_LENGTH
+#define SM2_GET_ENCRYPT_C1_LENGTH(pc_mode)          SM2_GET_POINTBYTES_LENGTH(pc_mode)
+#define SM2_ENCRYPT_C3_LENGTH                       SM3_DIGEST_LENGTH
+#define SM2_GET_ENCRYPT_HEADER_LENGTH(pc_mode)      (SM2_GET_ENCRYPT_C1_LENGTH(pc_mode) + SM2_ENCRYPT_C3_LENGTH)
 
 #define SM2_ERR_UID_OVERFLOW            -1
 #define SM2_ERR_INVALID_SK              -2
 #define SM2_ERR_INVALID_PK              -3
 #define SM2_ERR_MSG_OVERFLOW            -4
 #define SM2_ERR_NEED_SK                 -5
 #define SM2_ERR_RANDOM_FAILED           -6
 #define SM2_ERR_INVALID_SIGN            -7
 #define SM2_ERR_NEED_PK                 -8
+#define SM2_ERR_NO_MEMORY               -9
+#define SM2_ERR_DATA_OVERFLOW           -10
+#define SM2_ERR_INVALID_C1              -11
+#define SM2_ERR_INVALID_C3              -12
+#define SM2_ERR_INVALID_CIPHER          -13
 
 typedef UInt256 SM2ModN;
 typedef SM2ModN SM2ModNMont;
 
 typedef struct _SM2 {
     int has_sk;
     SM2ModN sk;
@@ -67,13 +72,15 @@
 int SM2_Init(SM2* self, const uint8_t* sk, const uint8_t* pk, uint64_t pk_len, const uint8_t* uid, uint64_t uid_len, int pc_mode, RandomAlg* rand_alg);
 int SM2_GenerateKeyPair(SM2* self, uint8_t* sk, uint8_t* pk);
 int SM2_GetEntityInfo(SM2* self, uint8_t* entity_info);
 int SM2_SignDigest(SM2* self, const uint8_t* digest, uint8_t* signature);
 int SM2_VerifyDigest(SM2* self, const uint8_t* digest, const uint8_t* signature);
 int SM2_Sign(SM2* self, const uint8_t* msg, uint64_t msg_len, uint8_t* signature);
 int SM2_Verify(SM2* self, const uint8_t* msg, uint64_t msg_len, const uint8_t* signature);
+int SM2_Encrypt(SM2* self, const uint8_t* plain, uint64_t plain_len, uint8_t* cipher);
+int SM2_Decrypt(SM2* self, const uint8_t* cipher, uint64_t cipher_len, uint8_t* plain, uint64_t* plain_len);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif // !GMALGLIB_SM2_H
```

### Comparing `gmalglib-0.4.1/include/gmalglib/sm2curve.h` & `gmalglib-0.5.1/include/gmalglib/sm2curve.h`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 extern const UInt256* const SM2_PARAMS_B;
 extern const SM2Point* const SM2_PARAMS_G;
 extern const UInt256* const SM2_PARAMS_N;
 
 void SM2JacobPointMont_ToPoint(const SM2JacobPointMont* X, SM2Point* Y);
 void SM2JacobPointMont_FromPoint(const SM2Point* X, SM2JacobPointMont* Y);
 
-uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, uint8_t* bytes, int pc_mode);
+uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, int pc_mode, uint8_t* bytes);
 int SM2JacobPointMont_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2JacobPointMont* X);
 
 int SM2JacobPointMont_IsInf(const SM2JacobPointMont* X);
 void SM2JacobPointMont_SetInf(SM2JacobPointMont* X);
 int SM2JacobPointMont_IsOnCurve(const SM2JacobPointMont* X);
 int SM2JacobPointMont_IsEqual(const SM2JacobPointMont* X, const SM2JacobPointMont* Y);
 void SM2JacobPointMont_Add(const SM2JacobPointMont* X, const SM2JacobPointMont* Y, SM2JacobPointMont* Z);
```

### Comparing `gmalglib-0.4.1/include/gmalglib/sm3.h` & `gmalglib-0.5.1/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/pyproject.toml` & `gmalglib-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/setup.py` & `gmalglib-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/src/gmalglib/core/bignum.c` & `gmalglib-0.5.1/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.1/src/gmalglib/core/sm2curve.c`

 * *Files 2% similar despite different names*

```diff
@@ -18,38 +18,34 @@
 
 // -3
 // 0xFFFFFFFE_FFFFFFFF_FFFFFFFF_FFFFFFFF_FFFFFFFF_00000000_FFFFFFFF_FFFFFFFC
 static const UInt256 _CONSTS_A = { .u32 = {
     0xFFFFFFFC, 0xFFFFFFFF, 0x00000000, 0xFFFFFFFF, 
     0xFFFFFFFF, 0xFFFFFFFF, 0xFFFFFFFF, 0xFFFFFFFE
 } };
-static const UInt256* const CONSTS_A = &_CONSTS_A;
 
 // 0x28E9FA9E_9D9F5E34_4D5A9E4B_CF6509A7_F39789F5_15AB8F92_DDBCBD41_4D940E93
 static const UInt256 _CONSTS_B = { .u32 = {
     0x4D940E93, 0xDDBCBD41, 0x15AB8F92, 0xF39789F5,
     0xCF6509A7, 0x4D5A9E4B, 0x9D9F5E34, 0x28E9FA9E
 } };
-static const UInt256* const CONSTS_B = &_CONSTS_B;
 
 // 0x32C4AE2C_1F198119_5F990446_6A39C994_8FE30BBF_F2660BE1_715A4589_334C74C7
 // 0xBC3736A2_F4F6779C_59BDCEE3_6B692153_D0A9877C_C62A4740_02DF32E5_2139F0A0
 static const SM2Point _CONSTS_POINT_G = {
     {.u32 = { 0x334C74C7, 0x715A4589, 0xF2660BE1, 0x8FE30BBF, 0x6A39C994, 0x5F990446, 0x1F198119, 0x32C4AE2C } },
     {.u32 = { 0x2139F0A0, 0x02DF32E5, 0xC62A4740, 0xD0A9877C, 0x6B692153, 0x59BDCEE3, 0xF4F6779C, 0xBC3736A2 } },
     0
 };
-static const SM2Point* const CONSTS_POINT_G = &_CONSTS_POINT_G;
 
 // 0xFFFFFFFE_FFFFFFFF_FFFFFFFF_FFFFFFFF_7203DF6B_21C6052B_53BBF409_39D54123
 static const UInt256 _CONSTS_N = { .u32 = {
     0x39D54123, 0x53BBF409, 0x21C6052B, 0x7203DF6B, 
     0xFFFFFFFF, 0xFFFFFFFF, 0xFFFFFFFF, 0xFFFFFFFE
 } };
-static const UInt256* const CONSTS_N = &_CONSTS_N;
 
 const UInt256* const SM2_PARAMS_P = &_CONSTS_P;
 const UInt256* const SM2_PARAMS_A = &_CONSTS_A;
 const UInt256* const SM2_PARAMS_B = &_CONSTS_B;
 const SM2Point* const SM2_PARAMS_G = &_CONSTS_POINT_G;
 const UInt256* const SM2_PARAMS_N = &_CONSTS_N;
 
@@ -371,15 +367,15 @@
     {
         SM2ModP_ToMont(&X->x, &Y->x);
         SM2ModP_ToMont(&X->y, &Y->y);
         Y->z = *CONSTS_MODP_MONT_ONE;
     }
 }
 
-uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, uint8_t* bytes, int pc_mode)
+uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, int pc_mode, uint8_t* bytes)
 {
     SM2Point pt = { 0 };
     SM2JacobPointMont_ToPoint(X, &pt);
 
     if (pt.is_inf)
     {
         bytes[0] = 0x00;
@@ -459,15 +455,15 @@
         SM2ModP_MontMul(&X->x, &X->y, &X->y);
         SM2ModP_MontAdd(&X->y, CONSTS_MODP_MONT_B, &X->y);
         if (!SM2ModP_MontHasSqrt(&X->y, &X->y))
             return SM2CURVE_ERR_NOTONCURVE;
 
         SM2ModP_FromMont(&X->y, &pt.y);
         ylsb = pt.y.u8[0] & 0x1;
-        if (pc == 0x02 && ylsb || pc == 0x03 && !ylsb)
+        if ((pc == 0x02 && ylsb) || (pc == 0x03 && !ylsb))
         {
             SM2ModP_MontNeg(&X->y, &X->y);
         }
     }
     else
     {
         return SM2CURVE_ERR_INVALIDPC;
```

### Comparing `gmalglib-0.4.1/src/gmalglib/core/sm3.c` & `gmalglib-0.5.1/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/src/gmalglib/core/sm4.c` & `gmalglib-0.5.1/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/src/gmalglib/core/zuc.c` & `gmalglib-0.5.1/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.4.1/src/gmalglib/coremodule.c` & `gmalglib-0.5.1/src/gmalglib/coremodule.c`

 * *Files 12% similar despite different names*

```diff
@@ -92,26 +92,22 @@
         return NULL;
 
     key_buffer = (uint8_t*)PyMem_RawCalloc(klen, sizeof(uint8_t));
     if (!key_buffer)
         return PyErr_NoMemory();
 
     sm3_ret = SM3_DeriveKey(&self->sm3, klen, key_buffer);
-    if (sm3_ret == SM3_ERR_OVERFLOW)
+
+    switch (sm3_ret)
     {
-        PyErr_SetString(PyExc_OverflowError, "Data too long.");
-        goto cleanup;
+    case SM3_ERR_OVERFLOW:          PyErr_SetString(PyExc_OverflowError, "Data too long.");             goto cleanup;
+    case SM3_ERR_KDF_OVERFLOW:      PyErr_SetString(PyExc_OverflowError, "Key stream too long.");       goto cleanup;
+    default:
+        ret = PyBytes_FromStringAndSize((char*)key_buffer, klen);
     }
-    if (sm3_ret == SM3_ERR_KDF_OVERFLOW)
-    {
-        PyErr_SetString(PyExc_OverflowError, "Key stream too long.");
-        goto cleanup;
-    }
-
-    ret = PyBytes_FromStringAndSize((char*)key_buffer, klen);
 
 cleanup:
     PyMem_RawFree(key_buffer);
     return ret;
 }
 
 static PyObject* PySM3_mac(PySM3Object* self, PyObject* args, PyObject* kwargs)
@@ -133,20 +129,20 @@
         return NULL;
     }
 
     return PyBytes_FromStringAndSize((char*)mac, SM3_MAC_LENGTH);
 }
 
 static PyMethodDef py_methods_def_SM3[] = {
-    {"update", (PyCFunction)PySM3_update, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("Update internal state with data stream.")},
-    {"digest", (PyCFunction)PySM3_digest, METH_NOARGS, PyDoc_STR("Get digest.")},
-    {"reset", (PyCFunction)PySM3_reset, METH_NOARGS, PyDoc_STR("Reset internal state to empty.")},
-    {"copy", (PyCFunction)PySM3_copy, METH_NOARGS, PyDoc_STR("Copy state to a new object.")},
-    {"derive_key", (PyCFunction)PySM3_derive_key, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("Key derivation function.")},
-    {"mac", (PyCFunction)PySM3_mac, METH_VARARGS | METH_KEYWORDS, PyDoc_STR("SM3 MAC.")},
+    {"update",      (PyCFunction)PySM3_update,      METH_VARARGS | METH_KEYWORDS,   PyDoc_STR("Update internal state with data stream.")},
+    {"digest",      (PyCFunction)PySM3_digest,      METH_NOARGS,                    PyDoc_STR("Get digest.")},
+    {"reset",       (PyCFunction)PySM3_reset,       METH_NOARGS,                    PyDoc_STR("Reset internal state to empty.")},
+    {"copy",        (PyCFunction)PySM3_copy,        METH_NOARGS,                    PyDoc_STR("Copy state to a new object.")},
+    {"derive_key",  (PyCFunction)PySM3_derive_key,  METH_VARARGS | METH_KEYWORDS,   PyDoc_STR("Key derivation function.")},
+    {"mac",         (PyCFunction)PySM3_mac,         METH_VARARGS | METH_KEYWORDS,   PyDoc_STR("SM3 MAC.")},
     {NULL}
 };
 
 static PyTypeObject py_type_SM3 = {
     .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "gmalglib.core.SM3",
     .tp_doc = PyDoc_STR("SM3 Object."),
@@ -157,24 +153,26 @@
     .tp_init = (initproc)PySM3_init,
     .tp_methods = py_methods_def_SM3,
 };
 
 static int PyModule_AddSM3(PyObject* py_module) 
 {
     PyObject* py_long_SM3_MAX_MSG_BITLEN = NULL;
+    PyObject* py_long_SM3_KDF_MAX_LENGTH = NULL;
 
     if (PyType_Ready(&py_type_SM3) < 0) return 0;
 
     Py_INCREF(&py_type_SM3);
-    if (PyModule_AddObject(py_module, "SM3", (PyObject*)&py_type_SM3) < 0) goto error;
-    if (!(py_long_SM3_MAX_MSG_BITLEN = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN))) goto error;
-    if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_SM3_MAX_MSG_BITLEN) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, SM3_DIGEST_LENGTH) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, SM3_KDF_MAX_LENGTH) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, SM3_MAC_LENGTH) < 0) goto error;
+    if (PyModule_AddObject(py_module, "SM3", (PyObject*)&py_type_SM3) < 0)                      goto error;
+    if (!(py_long_SM3_MAX_MSG_BITLEN = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN)))        goto error;
+    if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_SM3_MAX_MSG_BITLEN) < 0)    goto error;
+    if (PyModule_AddIntMacro(py_module, SM3_DIGEST_LENGTH) < 0)                                 goto error;
+    if (!(py_long_SM3_KDF_MAX_LENGTH = PyLong_FromUnsignedLongLong(SM3_KDF_MAX_LENGTH)))        goto error;
+    if (PyModule_AddObject(py_module, "SM3_KDF_MAX_LENGTH", py_long_SM3_KDF_MAX_LENGTH) < 0)    goto error;
+    if (PyModule_AddIntMacro(py_module, SM3_MAC_LENGTH) < 0)                                    goto error;
 
     return 1;
 
 error:
     Py_XDECREF(py_long_SM3_MAX_MSG_BITLEN);
     Py_DECREF(&py_type_SM3);
     return 0;
@@ -279,17 +277,17 @@
 };
 
 static int PyModule_AddSM4(PyObject* py_module) 
 {
     if (PyType_Ready(&py_type_SM4) < 0) return 0;
 
     Py_INCREF(&py_type_SM4);
-    if (PyModule_AddObject(py_module, "SM4", (PyObject*)&py_type_SM4) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, SM4_KEY_LENGTH) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, SM4_BLOCK_LENGTH) < 0) goto error;
+    if (PyModule_AddObject(py_module, "SM4", (PyObject*)&py_type_SM4) < 0)      goto error;
+    if (PyModule_AddIntMacro(py_module, SM4_KEY_LENGTH) < 0)                    goto error;
+    if (PyModule_AddIntMacro(py_module, SM4_BLOCK_LENGTH) < 0)                  goto error;
 
     return 1;
 
 error:
     Py_DECREF(&py_type_SM4);
     return 0;
 }
@@ -347,16 +345,16 @@
         return NULL;
 
     other->zuc = self->zuc;
     return (PyObject*)other;
 }
 
 static PyMethodDef py_methods_def_ZUC[] = {
-    {"generate", (PyCFunction)PyZUC_generate, METH_NOARGS, PyDoc_STR("Generate a word (4 bytes).")},
-    {"copy", (PyCFunction)PyZUC_copy, METH_NOARGS, PyDoc_STR("Copy state to a new object.")},
+    {"generate",    (PyCFunction)PyZUC_generate,    METH_NOARGS,    PyDoc_STR("Generate a word (4 bytes).")},
+    {"copy",        (PyCFunction)PyZUC_copy,        METH_NOARGS,    PyDoc_STR("Copy state to a new object.")},
     {NULL}
 };
 
 static PyTypeObject py_type_ZUC = {
     .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "gmalglib.core.ZUC",
     .tp_doc = PyDoc_STR("ZUC Object."),
@@ -369,18 +367,18 @@
 };
 
 static int PyModule_AddZUC(PyObject* py_module) 
 {
     if (PyType_Ready(&py_type_ZUC) < 0) return 0;
 
     Py_INCREF(&py_type_ZUC);
-    if (PyModule_AddObject(py_module, "ZUC", (PyObject*)&py_type_ZUC) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, ZUC_KEY_LENGTH) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, ZUC_IV_LENGTH) < 0) goto error;
-    if (PyModule_AddIntMacro(py_module, ZUC_WORD_LENGTH) < 0) goto error;
+    if (PyModule_AddObject(py_module, "ZUC", (PyObject*)&py_type_ZUC) < 0)      goto error;
+    if (PyModule_AddIntMacro(py_module, ZUC_KEY_LENGTH) < 0)                    goto error;
+    if (PyModule_AddIntMacro(py_module, ZUC_IV_LENGTH) < 0)                     goto error;
+    if (PyModule_AddIntMacro(py_module, ZUC_WORD_LENGTH) < 0)                   goto error;
 
     return 1;
 
 error:
     Py_DECREF(&py_type_ZUC);
     return 0;
 }
@@ -400,15 +398,15 @@
 
     if (PyObject_GetBuffer(py_bytes, &py_buffer, PyBUF_SIMPLE) != 0)
     {
         Py_CLEAR(py_bytes);
         return 0;
     }
 
-    if (py_buffer.len != bytes_len)
+    if ((uint64_t)py_buffer.len != bytes_len)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect random bytes length.");
         goto cleanup;
     }
 
     for (i = 0; i < py_buffer.len; i++)
     {
@@ -501,29 +499,21 @@
         &self->sm2, 
         py_buffer_sk.buf, 
         py_buffer_pk.buf, py_buffer_pk.len, 
         py_buffer_uid.buf, py_buffer_uid.len,
         pc_mode, 
         rnd_alg
     );
-
-    if (sm2_ret == SM2_ERR_INVALID_SK)
-    {
-        PyErr_SetString(PyExc_ValueError, "Invalid secret key.");
-        goto cleanup;
-    }
-    if (sm2_ret == SM2_ERR_INVALID_PK)
+    switch (sm2_ret)
     {
-        PyErr_SetString(PyExc_ValueError, "Invalid public key.");
-        goto cleanup;
-    }
-    if (sm2_ret == SM2_ERR_UID_OVERFLOW)
-    {
-        PyErr_SetString(PyExc_OverflowError, "uid too long.");
-        goto cleanup;
+    case SM2_ERR_INVALID_SK:        PyErr_SetString(PyExc_ValueError, "Invalid secret key.");       goto cleanup;
+    case SM2_ERR_INVALID_PK:        PyErr_SetString(PyExc_ValueError, "Invalid public key.");       goto cleanup;
+    case SM2_ERR_UID_OVERFLOW:      PyErr_SetString(PyExc_OverflowError, "uid too long.");          goto cleanup;
+    default:
+        break;
     }
 
     // self->sm2.rand_alg is untouched if SM2_Init failed
     // self->py_callable_rand_func should change after SM2_Init succeeded
     if (py_callable_rnd_fn)
     {
         Py_INCREF(py_callable_rnd_fn);
@@ -633,15 +623,15 @@
 
     if (SM2_GenerateKeyPair(&self->sm2, sk, pk) == SM2_ERR_RANDOM_FAILED)
     {
         PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");
         return NULL;
     }
 
-    return Py_BuildValue("y#y#", sk, (Py_ssize_t)SM2_SK_LENGTH, pk, (Py_ssize_t)SM2_GET_PK_LENGTH(self->sm2.pc_mode));
+    return Py_BuildValue("y#y#", (char*)sk, (Py_ssize_t)SM2_SK_LENGTH, pk, (Py_ssize_t)SM2_GET_PK_LENGTH(self->sm2.pc_mode));
 }
 
 static PyObject* PySM2_get_entity_info(PySM2Object* self, PyObject* Py_UNUSED(args))
 {
     uint8_t entity_info[SM2_ENTITYINFO_LENGTH] = { 0 };
     if (SM2_GetEntityInfo(&self->sm2, entity_info) != 0)
         Py_RETURN_NONE;
@@ -663,27 +653,22 @@
     if (py_buffer_digest.len != SM3_DIGEST_LENGTH)
     {
         PyErr_SetString(PyExc_ValueError, "Incorrect digest length.");
         goto cleanup;
     }
 
     sm2_ret = SM2_SignDigest(&self->sm2, py_buffer_digest.buf, signature);
-    if (sm2_ret == SM2_ERR_NEED_SK)
-    {
-        PyErr_SetString(PyExc_AttributeError, "Need secret key.");
-        goto cleanup;
-    }
-    if (sm2_ret == SM2_ERR_RANDOM_FAILED)
+    switch (sm2_ret)
     {
-        PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");
-        goto cleanup;
+    case SM2_ERR_NEED_SK:           PyErr_SetString(PyExc_AttributeError, "Need secret key.");              goto cleanup;
+    case SM2_ERR_RANDOM_FAILED:     PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");     goto cleanup;
+    default:
+        ret = PyBytes_FromStringAndSize((char*)signature, SM2_SIGNATURE_LENGTH);
     }
 
-    ret = PyBytes_FromStringAndSize((char*)signature, SM2_SIGNATURE_LENGTH);
-
 cleanup:
     PyBuffer_Release(&py_buffer_digest);
     return ret;
 }
 
 static PyObject* PySM2_verify_digest(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
@@ -735,37 +720,23 @@
     PyObject* ret = NULL;
     int sm2_ret = 0;
 
     if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:sign", keys, &py_buffer_message))
         return NULL;
 
     sm2_ret = SM2_Sign(&self->sm2, py_buffer_message.buf, py_buffer_message.len, signature);
-    if (sm2_ret == SM2_ERR_NEED_SK)
-    {
-        PyErr_SetString(PyExc_AttributeError, "Need secret key.");
-        goto cleanup;
-    }
-    if (sm2_ret == SM2_ERR_NEED_PK)
-    {
-        PyErr_SetString(PyExc_AttributeError, "Need public key.");
-        goto cleanup;
-    }
-    if (sm2_ret == SM2_ERR_MSG_OVERFLOW)
+    switch (sm2_ret)
     {
-        PyErr_SetString(PyExc_OverflowError, "Message too long.");
-        goto cleanup;
-    }
-    if (sm2_ret == SM2_ERR_RANDOM_FAILED)
-    {
-        PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");
-        goto cleanup;
+    case SM2_ERR_NEED_SK:           PyErr_SetString(PyExc_AttributeError, "Need secret key.");              goto cleanup;
+    case SM2_ERR_MSG_OVERFLOW:      PyErr_SetString(PyExc_OverflowError, "Message too long.");              goto cleanup;
+    case SM2_ERR_RANDOM_FAILED:     PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");     goto cleanup;
+    default:
+        ret = PyBytes_FromStringAndSize((char*)signature, SM2_SIGNATURE_LENGTH);
     }
 
-    ret = PyBytes_FromStringAndSize((char*)signature, SM2_SIGNATURE_LENGTH);
-
 cleanup:
     PyBuffer_Release(&py_buffer_message);
     return ret;
 }
 
 static PyObject* PySM2_verify(PySM2Object* self, PyObject* args, PyObject* kwargs)
 {
@@ -804,24 +775,105 @@
     {
         Py_RETURN_FALSE;
     }
 
     Py_RETURN_TRUE;
 }
 
+static PyObject* PySM2_encrypt(PySM2Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "plain", NULL };
+    Py_buffer py_buffer_plain = { 0 };
+    uint8_t* cipher = NULL;
+    uint64_t cipher_len = 0;
+    PyObject* ret = NULL;
+    int sm2_ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:encrypt", keys, &py_buffer_plain))
+        return NULL;
+
+    cipher_len = SM2_GET_ENCRYPT_HEADER_LENGTH(self->sm2.pc_mode) + py_buffer_plain.len;
+    cipher = (uint8_t*)calloc(cipher_len, sizeof(uint8_t));
+    if (!cipher)
+    {
+        PyErr_SetString(PyExc_MemoryError, "Failed to allocate buffer.");
+        goto cleanup;
+    }
+
+    sm2_ret = SM2_Encrypt(&self->sm2, py_buffer_plain.buf, py_buffer_plain.len, cipher);
+    switch (sm2_ret)
+    {
+    case SM2_ERR_NEED_PK:           PyErr_SetString(PyExc_AttributeError, "Need public key.");              goto cleanup;
+    case SM2_ERR_DATA_OVERFLOW:     PyErr_SetString(PyExc_OverflowError, "Data too long.");                 goto cleanup;
+    case SM2_ERR_NO_MEMORY:         PyErr_SetString(PyExc_MemoryError, "Failed to allocate buffer.");       goto cleanup;
+    case SM2_ERR_RANDOM_FAILED:     PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");     goto cleanup;
+    default:
+        ret = PyBytes_FromStringAndSize((char*)cipher, cipher_len);
+    }
+
+cleanup:
+    if (cipher)
+        free(cipher);
+    PyBuffer_Release(&py_buffer_plain);
+    return ret;
+}
+
+static PyObject* PySM2_decrypt(PySM2Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "cipher", NULL };
+    Py_buffer py_buffer_cipher = { 0 };
+    uint8_t* plain = NULL;
+    uint64_t plain_len = 0;
+    PyObject* ret = NULL;
+    int sm2_ret = 0;
+
+    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "y*:decrypt", keys, &py_buffer_cipher))
+        return NULL;
+
+    // cipher_len exactly greater than plain_len
+    plain_len = py_buffer_cipher.len - SM2_GET_ENCRYPT_HEADER_LENGTH(SM2_PCMODE_COMPRESS);
+    plain = (uint8_t*)calloc(plain_len, sizeof(uint8_t));
+    if (!plain)
+    {
+        PyErr_SetString(PyExc_MemoryError, "Failed to allocate buffer.");
+        goto cleanup;
+    }
+
+    sm2_ret = SM2_Decrypt(&self->sm2, py_buffer_cipher.buf, py_buffer_cipher.len, plain, &plain_len);
+    switch (sm2_ret)
+    {
+    case SM2_ERR_NEED_SK:           PyErr_SetString(PyExc_AttributeError, "Need secret key.");              goto cleanup;
+    case SM2_ERR_DATA_OVERFLOW:     PyErr_SetString(PyExc_OverflowError, "Data too long.");                 goto cleanup;
+    case SM2_ERR_NO_MEMORY:         PyErr_SetString(PyExc_MemoryError, "Failed to allocate buffer.");       goto cleanup;
+    case SM2_ERR_INVALID_CIPHER:    PyErr_SetString(PyExc_ValueError, "Invalid cipher.");                   goto cleanup;
+    case SM2_ERR_INVALID_C1:        PyErr_SetString(PyExc_ValueError, "Invalid C1.");                       goto cleanup;
+    case SM2_ERR_INVALID_C3:        PyErr_SetString(PyExc_ValueError, "Invalid C3.");                       goto cleanup;
+    default:
+        ret = PyBytes_FromStringAndSize((char*)plain, plain_len);
+    }
+
+cleanup:
+    if (plain)
+        free(plain);
+    PyBuffer_Release(&py_buffer_cipher);
+    return ret;
+}
+
 static PyMethodDef py_methods_def_SM2[] = {
     {"is_sk_valid",         (PyCFunction)PySM2_is_sk_valid,         METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check sk is valid.")},
     {"is_pk_valid",         (PyCFunction)PySM2_is_pk_valid,         METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check pk is valid.")},
     {"get_pk",              (PyCFunction)PySM2_get_pk,              METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Get public key bytes.")},
     {"generate_keypair",    (PyCFunction)PySM2_generate_keypair,    METH_NOARGS,                                    PyDoc_STR("Generate key pair.")},
     {"get_entity_info",     (PyCFunction)PySM2_get_entity_info,     METH_NOARGS,                                    PyDoc_STR("Get entity info.")},
     {"sign_digest",         (PyCFunction)PySM2_sign_digest,         METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Sign on digest.")},
     {"verify_digest",       (PyCFunction)PySM2_verify_digest,       METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Verify on digest.")},
     {"sign",                (PyCFunction)PySM2_sign,                METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Sign on full message.")},
     {"verify",              (PyCFunction)PySM2_verify,              METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Verify on full message.")},
+    {"encrypt",             (PyCFunction)PySM2_encrypt,             METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Encrypt data.")},
+    {"decrypt",             (PyCFunction)PySM2_decrypt,             METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Decrypt data.")},
     {NULL}
 };
 
 static PyTypeObject py_type_SM2 = {
     .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "gmalglib.core.SM2",
     .tp_doc = PyDoc_STR("SM2 Object."),
@@ -851,39 +903,39 @@
     if (PyType_Ready(&py_type_SM2) < 0) return 0;
 
     Py_INCREF(&py_type_SM2);
     if (PyModule_AddObject(py_module, "SM2", (PyObject*)&py_type_SM2) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_PARAMS_LENGTH) < 0) goto error;
     
     UInt256_ToBytes(SM2_PARAMS_P, buffer);
-    if (!(py_bytes_SM2_PARAMS_P = PyBytes_FromStringAndSize(buffer, SM2_PARAMS_LENGTH))) goto error;
+    if (!(py_bytes_SM2_PARAMS_P = PyBytes_FromStringAndSize((char*)buffer, SM2_PARAMS_LENGTH))) goto error;
     if (PyModule_AddObject(py_module, "SM2_PARAMS_P", py_bytes_SM2_PARAMS_P) < 0) goto error;
 
     UInt256_ToBytes(SM2_PARAMS_A, buffer);
-    if (!(py_bytes_SM2_PARAMS_A = PyBytes_FromStringAndSize(buffer, SM2_PARAMS_LENGTH))) goto error;
+    if (!(py_bytes_SM2_PARAMS_A = PyBytes_FromStringAndSize((char*)buffer, SM2_PARAMS_LENGTH))) goto error;
     if (PyModule_AddObject(py_module, "SM2_PARAMS_A", py_bytes_SM2_PARAMS_A) < 0) goto error;
 
     UInt256_ToBytes(SM2_PARAMS_B, buffer);
-    if (!(py_bytes_SM2_PARAMS_B = PyBytes_FromStringAndSize(buffer, SM2_PARAMS_LENGTH))) goto error;
+    if (!(py_bytes_SM2_PARAMS_B = PyBytes_FromStringAndSize((char*)buffer, SM2_PARAMS_LENGTH))) goto error;
     if (PyModule_AddObject(py_module, "SM2_PARAMS_B", py_bytes_SM2_PARAMS_B) < 0) goto error;
 
     UInt256_ToBytes(&SM2_PARAMS_G->x, buffer);
     UInt256_ToBytes(&SM2_PARAMS_G->y, buffer + SM2_PARAMS_LENGTH);
-    if (!(py_tuple_SM2_PARAMS_G = Py_BuildValue("y#y#", buffer, (Py_ssize_t)SM2_PARAMS_LENGTH, buffer + SM2_PARAMS_LENGTH, (Py_ssize_t)SM2_PARAMS_LENGTH))) goto error;
+    if (!(py_tuple_SM2_PARAMS_G = Py_BuildValue("y#y#", (char*)buffer, (Py_ssize_t)SM2_PARAMS_LENGTH, buffer + SM2_PARAMS_LENGTH, (Py_ssize_t)SM2_PARAMS_LENGTH))) goto error;
     if (PyModule_AddObject(py_module, "SM2_PARAMS_G", py_tuple_SM2_PARAMS_G) < 0) goto error;
 
     UInt256_ToBytes(SM2_PARAMS_N, buffer);
-    if (!(py_bytes_SM2_PARAMS_N = PyBytes_FromStringAndSize(buffer, SM2_PARAMS_LENGTH))) goto error;
+    if (!(py_bytes_SM2_PARAMS_N = PyBytes_FromStringAndSize((char*)buffer, SM2_PARAMS_LENGTH))) goto error;
     if (PyModule_AddObject(py_module, "SM2_PARAMS_N", py_bytes_SM2_PARAMS_N) < 0) goto error;
 
     if (PyModule_AddIntMacro(py_module, SM2_PCMODE_RAW) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_PCMODE_COMPRESS) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_PCMODE_MIX) < 0) goto error;
     
-    if (!(py_bytes_SM2_DEFAULT_UID = PyBytes_FromStringAndSize(SM2_DEFAULT_UID, SM2_DEFAULT_UID_LENGTH))) goto error;
+    if (!(py_bytes_SM2_DEFAULT_UID = PyBytes_FromStringAndSize((char*)SM2_DEFAULT_UID, SM2_DEFAULT_UID_LENGTH))) goto error;
     if (PyModule_AddObject(py_module, "SM2_DEFAULT_UID", py_bytes_SM2_DEFAULT_UID) < 0) goto error;
 
     if (PyModule_AddIntMacro(py_module, SM2_UID_MAX_LENGTH) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_ENTITYINFO_LENGTH) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_SK_LENGTH) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_PK_HALF_LENGTH) < 0) goto error;
     if (PyModule_AddIntMacro(py_module, SM2_PK_FULL_LENGTH) < 0) goto error;
```

### Comparing `gmalglib-0.4.1/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.1/src/gmalglib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/gmalglib/coremodule.c
 src/gmalglib/sm2.py
 src/gmalglib/sm2.pyi
 src/gmalglib/sm3.py
 src/gmalglib/sm3.pyi
 src/gmalglib/sm4.py
 src/gmalglib/sm4.pyi
+src/gmalglib/wrapped.py
 src/gmalglib/zuc.py
 src/gmalglib/zuc.pyi
 src/gmalglib.egg-info/PKG-INFO
 src/gmalglib.egg-info/SOURCES.txt
 src/gmalglib.egg-info/dependency_links.txt
 src/gmalglib.egg-info/top_level.txt
 src/gmalglib/core/bignum.c
```

