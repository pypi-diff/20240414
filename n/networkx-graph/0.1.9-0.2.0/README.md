# Comparing `tmp/networkx_graph-0.1.9.tar.gz` & `tmp/networkx_graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networkx_graph-0.1.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "networkx_graph-0.2.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `networkx_graph-0.1.9.tar` & `networkx_graph-0.2.0.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.clang-format
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1787 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2162 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.gitignore
--rwxr-xr-x   0        0        0     1364 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.vscode/launch.json
--rwxr-xr-x   0        0        0      381 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/.vscode/settings.json
--rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/LICENSE
--rw-r--r--   0        0        0     3772 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/Makefile
--rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/README.md
--rw-r--r--   0        0        0     7688 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/docs/Makefile
--rw-r--r--   0        0        0     9501 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/docs/conf.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/docs/index.rst
--rw-r--r--   0        0        0     7265 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/docs/make.bat
--rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/docs/python_example.rst
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/noxfile.py
--rw-r--r--   0        0        0     2244 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    82609 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/ankerl/unordered_dense.h
--rw-r--r--   0        0        0    26798 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/dbg.h
--rw-r--r--   0        0        0    15784 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/heap.hpp
--rw-r--r--   0        0        0     3134 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/indexer.hpp
--rw-r--r--   0        0        0   115326 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/main.cpp
--rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/networkx_graph/__init__.py
--rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/networkx_graph/__main__.py
--rw-r--r--   0        0        0    62742 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/poolstl.hpp
--rw-r--r--   0        0        0     3920 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/async.h
--rw-r--r--   0        0        0     2618 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/async_logger-inl.h
--rw-r--r--   0        0        0     2337 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/async_logger.h
--rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/cfg/argv.h
--rw-r--r--   0        0        0     3239 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/cfg/helpers-inl.h
--rw-r--r--   0        0        0      713 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/cfg/helpers.h
--rw-r--r--   0        0        0     2138 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/common-inl.h
--rw-r--r--   0        0        0    11174 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/common.h
--rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/backtracer-inl.h
--rw-r--r--   0        0        0     1137 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/backtracer.h
--rw-r--r--   0        0        0     3398 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/circular_q.h
--rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/console_globals.h
--rw-r--r--   0        0        0     4585 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/file_helper-inl.h
--rw-r--r--   0        0        0     1743 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/file_helper.h
--rw-r--r--   0        0        0     4649 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/fmt_helper.h
--rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/log_msg-inl.h
--rw-r--r--   0        0        0     1198 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/log_msg.h
--rw-r--r--   0        0        0     1682 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/log_msg_buffer-inl.h
--rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/log_msg_buffer.h
--rw-r--r--   0        0        0     3823 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/mpmc_blocking_q.h
--rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/null_mutex.h
--rw-r--r--   0        0        0    16862 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/os-inl.h
--rw-r--r--   0        0        0     3895 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/os.h
--rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/periodic_worker-inl.h
--rw-r--r--   0        0        0     1796 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/periodic_worker.h
--rw-r--r--   0        0        0     8419 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/registry-inl.h
--rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/registry.h
--rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/synchronous_factory.h
--rw-r--r--   0        0        0     4338 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/tcp_client-windows.h
--rw-r--r--   0        0        0     4087 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/tcp_client.h
--rw-r--r--   0        0        0     3843 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/thread_pool-inl.h
--rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/thread_pool.h
--rw-r--r--   0        0        0     3159 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/udp_client-windows.h
--rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/udp_client.h
--rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/details/windows_include.h
--rw-r--r--   0        0        0     7346 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bin_to_hex.h
--rw-r--r--   0        0        0     8130 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/args.h
--rw-r--r--   0        0        0    74516 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/chrono.h
--rw-r--r--   0        0        0    26009 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/color.h
--rw-r--r--   0        0        0    23340 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/compile.h
--rw-r--r--   0        0        0     1408 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/fmt.license.rst
--rw-r--r--   0        0        0   114995 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/format-inl.h
--rw-r--r--   0        0        0   119390 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/format.h
--rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/locale.h
--rw-r--r--   0        0        0    16203 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/os.h
--rw-r--r--   0        0        0     4510 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/ostream.h
--rw-r--r--   0        0        0    22863 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/printf.h
--rw-r--r--   0        0        0    31522 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/ranges.h
--rw-r--r--   0        0        0     9249 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/bundled/xchar.h
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/chrono.h
--rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/compile.h
--rw-r--r--   0        0        0      880 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/fmt.h
--rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/ostr.h
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/ranges.h
--rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fmt/xchar.h
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/formatter.h
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/fwd.h
--rw-r--r--   0        0        0     6813 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/logger-inl.h
--rw-r--r--   0        0        0    15190 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/logger.h
--rw-r--r--   0        0        0    45280 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/pattern_formatter-inl.h
--rw-r--r--   0        0        0     3670 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/pattern_formatter.h
--rw-r--r--   0        0        0     4600 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/android_sink.h
--rw-r--r--   0        0        0     4772 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/ansicolor_sink-inl.h
--rw-r--r--   0        0        0     3973 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/ansicolor_sink.h
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/base_sink-inl.h
--rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/base_sink.h
--rw-r--r--   0        0        0     1111 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/basic_file_sink-inl.h
--rw-r--r--   0        0        0     1940 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/basic_file_sink.h
--rw-r--r--   0        0        0    10867 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/daily_file_sink.h
--rw-r--r--   0        0        0     2398 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/dist_sink.h
--rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/dup_filter_sink.h
--rw-r--r--   0        0        0     6830 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/hourly_file_sink.h
--rw-r--r--   0        0        0     3609 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/mongo_sink.h
--rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/msvc_sink.h
--rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/null_sink.h
--rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/ostream_sink.h
--rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/qt_sinks.h
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/ringbuffer_sink.h
--rw-r--r--   0        0        0     4927 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/rotating_file_sink-inl.h
--rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/rotating_file_sink.h
--rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/sink-inl.h
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/sink.h
--rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/stdout_color_sinks-inl.h
--rw-r--r--   0        0        0     1682 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/stdout_color_sinks.h
--rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/stdout_sinks-inl.h
--rw-r--r--   0        0        0     2430 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/stdout_sinks.h
--rw-r--r--   0        0        0     3920 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/syslog_sink.h
--rw-r--r--   0        0        0     4895 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/systemd_sink.h
--rw-r--r--   0        0        0     2135 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/tcp_sink.h
--rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/udp_sink.h
--rw-r--r--   0        0        0     9151 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/win_eventlog_sink.h
--rw-r--r--   0        0        0     6671 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/wincolor_sink-inl.h
--rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/sinks/wincolor_sink.h
--rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/spdlog-inl.h
--rw-r--r--   0        0        0    12035 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/spdlog.h
--rw-r--r--   0        0        0     1719 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/stopwatch.h
--rw-r--r--   0        0        0     6462 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/tweakme.h
--rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/spdlog/version.h
--rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/src/types.hpp
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0    40736 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/tests/test_basic.py
--rw-r--r--   0        0        0      821 2022-11-09 12:37:21.000000 networkx_graph-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.clang-format
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1787 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2162 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.gitignore
+-rwxr-xr-x   0        0        0     1364 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      367 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0      465 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.vscode/launch.json
+-rwxr-xr-x   0        0        0      381 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1779 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3772 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/Makefile
+-rw-r--r--   0        0        0       96 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/README.md
+-rw-r--r--   0        0        0     7688 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0     9501 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0     7265 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0       31 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/docs/python_example.rst
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/noxfile.py
+-rw-r--r--   0        0        0     2244 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    82609 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/ankerl/unordered_dense.h
+-rw-r--r--   0        0        0    26798 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/dbg.h
+-rw-r--r--   0        0        0    15784 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/heap.hpp
+-rw-r--r--   0        0        0     3134 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/indexer.hpp
+-rw-r--r--   0        0        0   115696 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/main.cpp
+-rw-r--r--   0        0        0     1409 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/networkx_graph/__init__.py
+-rw-r--r--   0        0        0      275 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/networkx_graph/__main__.py
+-rw-r--r--   0        0        0    62742 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/poolstl.hpp
+-rw-r--r--   0        0        0     3920 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/async.h
+-rw-r--r--   0        0        0     2618 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/async_logger-inl.h
+-rw-r--r--   0        0        0     2337 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/async_logger.h
+-rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/cfg/argv.h
+-rw-r--r--   0        0        0     3239 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/cfg/helpers-inl.h
+-rw-r--r--   0        0        0      713 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/cfg/helpers.h
+-rw-r--r--   0        0        0     2138 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/common-inl.h
+-rw-r--r--   0        0        0    11174 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/common.h
+-rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/backtracer-inl.h
+-rw-r--r--   0        0        0     1137 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/backtracer.h
+-rw-r--r--   0        0        0     3398 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/circular_q.h
+-rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/console_globals.h
+-rw-r--r--   0        0        0     4585 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/file_helper-inl.h
+-rw-r--r--   0        0        0     1743 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/file_helper.h
+-rw-r--r--   0        0        0     4649 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/fmt_helper.h
+-rw-r--r--   0        0        0     1208 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/log_msg-inl.h
+-rw-r--r--   0        0        0     1198 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/log_msg.h
+-rw-r--r--   0        0        0     1682 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/log_msg_buffer-inl.h
+-rw-r--r--   0        0        0      931 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/log_msg_buffer.h
+-rw-r--r--   0        0        0     3823 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/mpmc_blocking_q.h
+-rw-r--r--   0        0        0      955 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/null_mutex.h
+-rw-r--r--   0        0        0    16862 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/os-inl.h
+-rw-r--r--   0        0        0     3895 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/os.h
+-rw-r--r--   0        0        0      614 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/periodic_worker-inl.h
+-rw-r--r--   0        0        0     1796 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/periodic_worker.h
+-rw-r--r--   0        0        0     8419 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/registry-inl.h
+-rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/registry.h
+-rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/synchronous_factory.h
+-rw-r--r--   0        0        0     4338 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/tcp_client-windows.h
+-rw-r--r--   0        0        0     4087 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/tcp_client.h
+-rw-r--r--   0        0        0     3843 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/thread_pool-inl.h
+-rw-r--r--   0        0        0     3487 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/thread_pool.h
+-rw-r--r--   0        0        0     3159 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/udp_client-windows.h
+-rw-r--r--   0        0        0     2271 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/udp_client.h
+-rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/details/windows_include.h
+-rw-r--r--   0        0        0     7346 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bin_to_hex.h
+-rw-r--r--   0        0        0     8130 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/args.h
+-rw-r--r--   0        0        0    74516 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/chrono.h
+-rw-r--r--   0        0        0    26009 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/color.h
+-rw-r--r--   0        0        0    23340 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/compile.h
+-rw-r--r--   0        0        0     1408 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/fmt.license.rst
+-rw-r--r--   0        0        0   114995 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/format-inl.h
+-rw-r--r--   0        0        0   119390 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/format.h
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/locale.h
+-rw-r--r--   0        0        0    16203 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/os.h
+-rw-r--r--   0        0        0     4510 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/ostream.h
+-rw-r--r--   0        0        0    22863 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/printf.h
+-rw-r--r--   0        0        0    31522 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/ranges.h
+-rw-r--r--   0        0        0     9249 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/bundled/xchar.h
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/chrono.h
+-rw-r--r--   0        0        0      447 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/compile.h
+-rw-r--r--   0        0        0      880 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/fmt.h
+-rw-r--r--   0        0        0      442 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/ostr.h
+-rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/ranges.h
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fmt/xchar.h
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/formatter.h
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/fwd.h
+-rw-r--r--   0        0        0     6813 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/logger-inl.h
+-rw-r--r--   0        0        0    15190 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/logger.h
+-rw-r--r--   0        0        0    45280 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/pattern_formatter-inl.h
+-rw-r--r--   0        0        0     3670 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/pattern_formatter.h
+-rw-r--r--   0        0        0     4600 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/android_sink.h
+-rw-r--r--   0        0        0     4772 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/ansicolor_sink-inl.h
+-rw-r--r--   0        0        0     3973 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/ansicolor_sink.h
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/base_sink-inl.h
+-rw-r--r--   0        0        0     1570 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/base_sink.h
+-rw-r--r--   0        0        0     1111 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/basic_file_sink-inl.h
+-rw-r--r--   0        0        0     1940 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/basic_file_sink.h
+-rw-r--r--   0        0        0    10867 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/daily_file_sink.h
+-rw-r--r--   0        0        0     2398 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/dist_sink.h
+-rw-r--r--   0        0        0     3152 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/dup_filter_sink.h
+-rw-r--r--   0        0        0     6830 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/hourly_file_sink.h
+-rw-r--r--   0        0        0     3609 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/mongo_sink.h
+-rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/msvc_sink.h
+-rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/null_sink.h
+-rw-r--r--   0        0        0     1250 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/ostream_sink.h
+-rw-r--r--   0        0        0     3981 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/qt_sinks.h
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/ringbuffer_sink.h
+-rw-r--r--   0        0        0     4927 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/rotating_file_sink-inl.h
+-rw-r--r--   0        0        0     2871 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/rotating_file_sink.h
+-rw-r--r--   0        0        0      730 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/sink-inl.h
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/sink.h
+-rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/stdout_color_sinks-inl.h
+-rw-r--r--   0        0        0     1682 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/stdout_color_sinks.h
+-rw-r--r--   0        0        0     4424 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/stdout_sinks-inl.h
+-rw-r--r--   0        0        0     2430 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/stdout_sinks.h
+-rw-r--r--   0        0        0     3920 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/syslog_sink.h
+-rw-r--r--   0        0        0     4895 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/systemd_sink.h
+-rw-r--r--   0        0        0     2135 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/tcp_sink.h
+-rw-r--r--   0        0        0     1920 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/udp_sink.h
+-rw-r--r--   0        0        0     9151 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/win_eventlog_sink.h
+-rw-r--r--   0        0        0     6671 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/wincolor_sink-inl.h
+-rw-r--r--   0        0        0     2742 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/sinks/wincolor_sink.h
+-rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/spdlog-inl.h
+-rw-r--r--   0        0        0    12035 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/spdlog.h
+-rw-r--r--   0        0        0     1719 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/stopwatch.h
+-rw-r--r--   0        0        0     6462 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/tweakme.h
+-rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/spdlog/version.h
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/src/types.hpp
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0    40873 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/tests/test_basic.py
+-rw-r--r--   0        0        0      821 2022-11-09 12:37:21.000000 networkx_graph-0.2.0/PKG-INFO
```

### Comparing `networkx_graph-0.1.9/.clang-format` & `networkx_graph-0.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/.github/workflows/pip.yml` & `networkx_graph-0.2.0/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/.github/workflows/wheels.yml` & `networkx_graph-0.2.0/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/.gitignore` & `networkx_graph-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/.pre-commit-config.yaml` & `networkx_graph-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/CMakeLists.txt` & `networkx_graph-0.2.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/LICENSE` & `networkx_graph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/Makefile` & `networkx_graph-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/docs/Makefile` & `networkx_graph-0.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/docs/conf.py` & `networkx_graph-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/docs/make.bat` & `networkx_graph-0.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/pyproject.toml` & `networkx_graph-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core>=0.3.3", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "networkx_graph"
-version = "0.1.9"
+version = "0.2.0"
 url = "https://github.com/cubao/networkx-graph"
 description = "Some customized graph algorithms"
 readme = "README.md"
 authors = [
   { name = "district10", email = "dvorak4tzx@gmail.com" },
 ]
 requires-python = ">=3.7"
```

### Comparing `networkx_graph-0.1.9/src/ankerl/unordered_dense.h` & `networkx_graph-0.2.0/src/ankerl/unordered_dense.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/dbg.h` & `networkx_graph-0.2.0/src/dbg.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/heap.hpp` & `networkx_graph-0.2.0/src/heap.hpp`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/indexer.hpp` & `networkx_graph-0.2.0/src/indexer.hpp`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/main.cpp` & `networkx_graph-0.2.0/src/main.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2227,21 +2227,28 @@
                     nids.push_back(std::get<0>(*nid_len));
                     lengths.push_back(std::get<1>(*nid_len));
                 }
                 double dist = 0.0;
                 for (size_t i = 1; i < N - 1; ++i) {
                     dist += lengths[i];
                 }
-                if (start_offset) {
+                if (N == 1 && start_offset && end_offset) {
                     start_offset = CLIP(0.0, *start_offset, lengths.front());
-                    dist += lengths.front() - *start_offset;
-                }
-                if (end_offset) {
                     end_offset = CLIP(0.0, *end_offset, lengths.back());
-                    dist += *end_offset;
+                    dist = *end_offset - *start_offset;
+                } else {
+                    if (start_offset) {
+                        start_offset =
+                            CLIP(0.0, *start_offset, lengths.front());
+                        dist += lengths.front() - *start_offset;
+                    }
+                    if (end_offset) {
+                        end_offset = CLIP(0.0, *end_offset, lengths.back());
+                        dist += *end_offset;
+                    }
                 }
                 auto p = Path(&graph, dist, nids, start_offset, end_offset);
                 auto round_scale = graph.round_scale();
                 if (round_scale) {
                     p.round(*round_scale);
                 }
                 if (binding) {
```

### Comparing `networkx_graph-0.1.9/src/networkx_graph/__init__.py` & `networkx_graph-0.2.0/src/networkx_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/poolstl.hpp` & `networkx_graph-0.2.0/src/poolstl.hpp`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/async.h` & `networkx_graph-0.2.0/src/spdlog/async.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/async_logger-inl.h` & `networkx_graph-0.2.0/src/spdlog/async_logger-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/async_logger.h` & `networkx_graph-0.2.0/src/spdlog/async_logger.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/cfg/argv.h` & `networkx_graph-0.2.0/src/spdlog/cfg/argv.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/cfg/helpers-inl.h` & `networkx_graph-0.2.0/src/spdlog/cfg/helpers-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/cfg/helpers.h` & `networkx_graph-0.2.0/src/spdlog/cfg/helpers.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/common-inl.h` & `networkx_graph-0.2.0/src/spdlog/common-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/common.h` & `networkx_graph-0.2.0/src/spdlog/common.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/backtracer-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/backtracer-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/backtracer.h` & `networkx_graph-0.2.0/src/spdlog/details/backtracer.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/circular_q.h` & `networkx_graph-0.2.0/src/spdlog/details/circular_q.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/console_globals.h` & `networkx_graph-0.2.0/src/spdlog/details/console_globals.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/file_helper-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/file_helper-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/file_helper.h` & `networkx_graph-0.2.0/src/spdlog/details/file_helper.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/fmt_helper.h` & `networkx_graph-0.2.0/src/spdlog/details/fmt_helper.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/log_msg-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/log_msg-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/log_msg.h` & `networkx_graph-0.2.0/src/spdlog/details/log_msg.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/log_msg_buffer-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/log_msg_buffer-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/log_msg_buffer.h` & `networkx_graph-0.2.0/src/spdlog/details/log_msg_buffer.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/mpmc_blocking_q.h` & `networkx_graph-0.2.0/src/spdlog/details/mpmc_blocking_q.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/null_mutex.h` & `networkx_graph-0.2.0/src/spdlog/details/null_mutex.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/os-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/os-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/os.h` & `networkx_graph-0.2.0/src/spdlog/details/os.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/periodic_worker-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/periodic_worker-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/periodic_worker.h` & `networkx_graph-0.2.0/src/spdlog/details/periodic_worker.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/registry-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/registry-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/registry.h` & `networkx_graph-0.2.0/src/spdlog/details/registry.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/synchronous_factory.h` & `networkx_graph-0.2.0/src/spdlog/details/synchronous_factory.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/tcp_client-windows.h` & `networkx_graph-0.2.0/src/spdlog/details/tcp_client-windows.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/tcp_client.h` & `networkx_graph-0.2.0/src/spdlog/details/tcp_client.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/thread_pool-inl.h` & `networkx_graph-0.2.0/src/spdlog/details/thread_pool-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/thread_pool.h` & `networkx_graph-0.2.0/src/spdlog/details/thread_pool.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/udp_client-windows.h` & `networkx_graph-0.2.0/src/spdlog/details/udp_client-windows.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/details/udp_client.h` & `networkx_graph-0.2.0/src/spdlog/details/udp_client.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bin_to_hex.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bin_to_hex.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/args.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/args.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/chrono.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/chrono.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/color.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/color.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/compile.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/compile.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/fmt.license.rst` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/fmt.license.rst`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/format-inl.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/format-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/format.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/format.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/os.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/os.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/ostream.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/ostream.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/printf.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/printf.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/ranges.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/ranges.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/bundled/xchar.h` & `networkx_graph-0.2.0/src/spdlog/fmt/bundled/xchar.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/chrono.h` & `networkx_graph-0.2.0/src/spdlog/fmt/chrono.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/fmt/fmt.h` & `networkx_graph-0.2.0/src/spdlog/fmt/fmt.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/logger-inl.h` & `networkx_graph-0.2.0/src/spdlog/logger-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/logger.h` & `networkx_graph-0.2.0/src/spdlog/logger.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/pattern_formatter-inl.h` & `networkx_graph-0.2.0/src/spdlog/pattern_formatter-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/pattern_formatter.h` & `networkx_graph-0.2.0/src/spdlog/pattern_formatter.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/android_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/android_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/ansicolor_sink-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/ansicolor_sink-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/ansicolor_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/ansicolor_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/base_sink-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/base_sink-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/base_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/base_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/basic_file_sink-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/basic_file_sink-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/basic_file_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/basic_file_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/daily_file_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/daily_file_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/dist_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/dist_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/dup_filter_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/dup_filter_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/hourly_file_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/hourly_file_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/mongo_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/mongo_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/msvc_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/msvc_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/null_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/null_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/ostream_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/ostream_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/qt_sinks.h` & `networkx_graph-0.2.0/src/spdlog/sinks/qt_sinks.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/ringbuffer_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/ringbuffer_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/rotating_file_sink-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/rotating_file_sink-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/rotating_file_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/rotating_file_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/sink-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/sink-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/stdout_color_sinks-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/stdout_color_sinks-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/stdout_color_sinks.h` & `networkx_graph-0.2.0/src/spdlog/sinks/stdout_color_sinks.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/stdout_sinks-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/stdout_sinks-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/stdout_sinks.h` & `networkx_graph-0.2.0/src/spdlog/sinks/stdout_sinks.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/syslog_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/syslog_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/systemd_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/systemd_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/tcp_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/tcp_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/udp_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/udp_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/win_eventlog_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/win_eventlog_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/wincolor_sink-inl.h` & `networkx_graph-0.2.0/src/spdlog/sinks/wincolor_sink-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/sinks/wincolor_sink.h` & `networkx_graph-0.2.0/src/spdlog/sinks/wincolor_sink.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/spdlog-inl.h` & `networkx_graph-0.2.0/src/spdlog/spdlog-inl.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/spdlog.h` & `networkx_graph-0.2.0/src/spdlog/spdlog.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/stopwatch.h` & `networkx_graph-0.2.0/src/spdlog/stopwatch.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/spdlog/tweakme.h` & `networkx_graph-0.2.0/src/spdlog/tweakme.h`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/src/types.hpp` & `networkx_graph-0.2.0/src/types.hpp`

 * *Files identical despite different names*

### Comparing `networkx_graph-0.1.9/tests/test_basic.py` & `networkx_graph-0.2.0/tests/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 hash_md5.update(block)
     except OSError:
         return None
     return hash_md5.hexdigest()
 
 
 def test_version():
-    assert m.__version__ == "0.1.9"
+    assert m.__version__ == "0.2.0"
 
 
 def test_add():
     assert m.add(1, 2) == 3
 
 
 def test_sub():
@@ -1409,14 +1409,22 @@
         path.nodes,
         start_offset=5.12345,
         end_offset=27.0,
         binding=("w3", (5.0, 5.0, "something")),
     )
     assert path2.binding == ("w3", (5.0, 5.0, "something"))
 
+    path2 = Path.Build(
+        G,
+        ["w1"],
+        start_offset=1.8,
+        end_offset=3.3,
+    )
+    assert path2.dist == 1.5
+
     with pytest.raises(ValueError) as e:  # noqa: PT011
         path2 = Path.Build(G, ["w1", "w3", "no_such_road"])
     assert "missing node no_such_road" in repr(e)
     with pytest.raises(ValueError) as e:  # noqa: PT011
         path2 = Path.Build(
             G,
             path.nodes,
```

### Comparing `networkx_graph-0.1.9/PKG-INFO` & `networkx_graph-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networkx_graph
-Version: 0.1.9
+Version: 0.2.0
 Summary: Some customized graph algorithms
 Author-Email: district10 <dvorak4tzx@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

