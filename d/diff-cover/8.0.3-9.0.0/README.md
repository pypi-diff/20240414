# Comparing `tmp/diff_cover-8.0.3.tar.gz` & `tmp/diff_cover-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diff_cover-8.0.3.tar", max compression
+gzip compressed data, was "diff_cover-9.0.0.tar", max compression
```

## Comparing `diff_cover-8.0.3.tar` & `diff_cover-9.0.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0    10174 2023-11-26 20:29:29.260372 diff_cover-8.0.3/LICENSE
--rw-r--r--   0        0        0    15616 2023-11-26 20:29:29.260610 diff_cover-8.0.3/README.rst
--rw-r--r--   0        0        0      417 2023-11-26 20:29:29.260689 diff_cover-8.0.3/diff_cover/__init__.py
--rw-r--r--   0        0        0     2028 2023-12-16 20:11:11.631833 diff_cover-8.0.3/diff_cover/command_runner.py
--rw-r--r--   0        0        0     2295 2023-11-26 20:29:29.260788 diff_cover-8.0.3/diff_cover/config_parser.py
--rw-r--r--   0        0        0     9236 2023-11-26 20:29:29.260871 diff_cover-8.0.3/diff_cover/diff_cover_tool.py
--rw-r--r--   0        0        0    11548 2023-11-26 20:29:29.260924 diff_cover-8.0.3/diff_cover/diff_quality_tool.py
--rw-r--r--   0        0        0    16718 2023-11-26 20:29:29.260995 diff_cover-8.0.3/diff_cover/diff_reporter.py
--rw-r--r--   0        0        0     3839 2023-11-26 20:29:29.261076 diff_cover-8.0.3/diff_cover/git_diff.py
--rw-r--r--   0        0        0     2036 2023-11-26 20:29:29.261128 diff_cover-8.0.3/diff_cover/git_path.py
--rw-r--r--   0        0        0      123 2023-11-26 20:29:29.261176 diff_cover-8.0.3/diff_cover/hook.py
--rw-r--r--   0        0        0      240 2023-11-26 20:29:29.261228 diff_cover-8.0.3/diff_cover/hookspecs.py
--rw-r--r--   0        0        0    14359 2024-01-20 15:03:34.860996 diff_cover-8.0.3/diff_cover/report_generator.py
--rw-r--r--   0        0        0    14118 2023-11-26 20:29:29.261503 diff_cover-8.0.3/diff_cover/snippets.py
--rw-r--r--   0        0        0      742 2023-11-26 20:29:29.261581 diff_cover-8.0.3/diff_cover/templates/console_coverage_report.txt
--rw-r--r--   0        0        0      787 2023-11-26 20:29:29.261628 diff_cover-8.0.3/diff_cover/templates/console_quality_report.txt
--rw-r--r--   0        0        0      174 2023-11-26 20:29:29.261682 diff_cover-8.0.3/diff_cover/templates/external_style.css
--rw-r--r--   0        0        0     1632 2023-11-26 20:29:29.261734 diff_cover-8.0.3/diff_cover/templates/html_coverage_report.html
--rw-r--r--   0        0        0     1880 2023-11-26 20:29:29.261788 diff_cover-8.0.3/diff_cover/templates/html_quality_report.html
--rw-r--r--   0        0        0      759 2023-11-26 20:29:29.261841 diff_cover-8.0.3/diff_cover/templates/markdown_coverage_report.md
--rw-r--r--   0        0        0      754 2023-11-26 20:29:29.261889 diff_cover-8.0.3/diff_cover/templates/markdown_quality_report.md
--rw-r--r--   0        0        0      371 2023-11-26 20:29:29.261939 diff_cover-8.0.3/diff_cover/templates/snippet_content.html
--rw-r--r--   0        0        0      229 2023-11-26 20:29:29.261985 diff_cover-8.0.3/diff_cover/templates/snippet_content.md
--rw-r--r--   0        0        0      204 2023-11-26 20:29:29.262029 diff_cover-8.0.3/diff_cover/templates/snippet_content.txt
--rw-r--r--   0        0        0      419 2023-11-26 20:29:29.262077 diff_cover-8.0.3/diff_cover/templates/snippet_style.html
--rw-r--r--   0        0        0      687 2023-11-26 20:29:29.262143 diff_cover-8.0.3/diff_cover/util.py
--rw-r--r--   0        0        0        0 2023-11-26 20:29:29.262194 diff_cover-8.0.3/diff_cover/violationsreporters/__init__.py
--rw-r--r--   0        0        0     8455 2023-11-26 20:29:29.262266 diff_cover-8.0.3/diff_cover/violationsreporters/base.py
--rw-r--r--   0        0        0     5837 2023-11-26 20:29:29.262333 diff_cover-8.0.3/diff_cover/violationsreporters/java_violations_reporter.py
--rw-r--r--   0        0        0    26028 2023-11-26 20:29:29.262416 diff_cover-8.0.3/diff_cover/violationsreporters/violations_reporter.py
--rw-r--r--   0        0        0     3466 2024-01-20 15:07:26.508794 diff_cover-8.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-26 20:29:29.262806 diff_cover-8.0.3/tests/__init__.py
--rw-r--r--   0        0        0      220 2023-11-26 20:29:29.262912 diff_cover-8.0.3/tests/fixtures/add_console_report.txt
--rw-r--r--   0        0        0     5234 2023-11-26 20:29:29.262985 diff_cover-8.0.3/tests/fixtures/add_html_report.html
--rw-r--r--   0        0        0      192 2023-11-26 20:29:29.263033 diff_cover-8.0.3/tests/fixtures/changed_console_report.txt
--rw-r--r--   0        0        0     4372 2023-11-26 20:29:29.263086 diff_cover-8.0.3/tests/fixtures/changed_html_report.html
--rw-r--r--   0        0        0      855 2023-11-26 20:29:29.263152 diff_cover-8.0.3/tests/fixtures/coverage.xml
--rw-r--r--   0        0        0      855 2023-11-26 20:29:29.263214 diff_cover-8.0.3/tests/fixtures/coverage1.xml
--rw-r--r--   0        0        0      855 2023-11-26 20:29:29.263289 diff_cover-8.0.3/tests/fixtures/coverage2.xml
--rw-r--r--   0        0        0      159 2023-11-26 20:29:29.263355 diff_cover-8.0.3/tests/fixtures/delete_console_report.txt
--rw-r--r--   0        0        0     3946 2023-11-26 20:29:29.263405 diff_cover-8.0.3/tests/fixtures/delete_html_report.html
--rw-r--r--   0        0        0     2664 2023-11-26 20:29:29.263455 diff_cover-8.0.3/tests/fixtures/dotnet_coverage.xml
--rw-r--r--   0        0        0      219 2023-11-26 20:29:29.263498 diff_cover-8.0.3/tests/fixtures/dotnet_coverage_console_report.txt
--rw-r--r--   0        0        0        0 2023-11-26 20:29:29.263517 diff_cover-8.0.3/tests/fixtures/empty.txt
--rw-r--r--   0        0        0      235 2023-11-26 20:29:29.263577 diff_cover-8.0.3/tests/fixtures/empty_pycodestyle_violations.txt
--rw-r--r--   0        0        0      913 2023-11-26 20:29:29.263632 diff_cover-8.0.3/tests/fixtures/external_css_html_report.html
--rw-r--r--   0        0        0     3400 2023-11-26 20:29:29.263691 diff_cover-8.0.3/tests/fixtures/external_style.css
--rw-r--r--   0        0        0      216 2023-11-26 20:29:29.263749 diff_cover-8.0.3/tests/fixtures/git_diff_add.txt
--rw-r--r--   0        0        0      216 2023-11-26 20:29:29.263798 diff_cover-8.0.3/tests/fixtures/git_diff_changed.txt
--rw-r--r--   0        0        0      560 2023-11-26 20:29:29.263851 diff_cover-8.0.3/tests/fixtures/git_diff_code_dupe.txt
--rw-r--r--   0        0        0      220 2023-11-26 20:29:29.263898 diff_cover-8.0.3/tests/fixtures/git_diff_delete.txt
--rw-r--r--   0        0        0      365 2023-11-26 20:29:29.263952 diff_cover-8.0.3/tests/fixtures/git_diff_dotnet.txt
--rw-r--r--   0        0        0      216 2023-11-26 20:29:29.264000 diff_cover-8.0.3/tests/fixtures/git_diff_external_css.txt
--rw-r--r--   0        0        0      259 2023-11-26 20:29:29.264050 diff_cover-8.0.3/tests/fixtures/git_diff_lua.txt
--rw-r--r--   0        0        0      216 2023-11-26 20:29:29.264095 diff_cover-8.0.3/tests/fixtures/git_diff_moved.txt
--rw-r--r--   0        0        0      216 2023-11-26 20:29:29.264136 diff_cover-8.0.3/tests/fixtures/git_diff_mult.txt
--rw-r--r--   0        0        0      228 2023-11-26 20:29:29.264183 diff_cover-8.0.3/tests/fixtures/git_diff_subdir.txt
--rw-r--r--   0        0        0      310 2023-11-26 20:29:29.264226 diff_cover-8.0.3/tests/fixtures/git_diff_unicode.txt
--rw-r--r--   0        0        0      543 2023-11-26 20:29:29.264274 diff_cover-8.0.3/tests/fixtures/git_diff_violations.txt
--rw-r--r--   0        0        0      266 2023-11-26 20:29:29.264320 diff_cover-8.0.3/tests/fixtures/git_diff_violations_two_files.txt
--rw-r--r--   0        0        0       33 2023-11-26 20:29:29.264360 diff_cover-8.0.3/tests/fixtures/hello.py
--rw-r--r--   0        0        0       33 2023-11-26 20:29:29.264402 diff_cover-8.0.3/tests/fixtures/hi.py
--rw-r--r--   0        0        0     1237 2023-11-26 20:29:29.264453 diff_cover-8.0.3/tests/fixtures/html_report.html
--rw-r--r--   0        0        0      677 2023-11-26 20:29:29.264505 diff_cover-8.0.3/tests/fixtures/html_report_empty.html
--rw-r--r--   0        0        0     1652 2023-11-26 20:29:29.264553 diff_cover-8.0.3/tests/fixtures/html_report_one_snippet.html
--rw-r--r--   0        0        0     1756 2023-11-26 20:29:29.264618 diff_cover-8.0.3/tests/fixtures/html_report_two_snippets.html
--rw-r--r--   0        0        0      232 2023-11-26 20:29:29.264667 diff_cover-8.0.3/tests/fixtures/lcov.info
--rw-r--r--   0        0        0      214 2023-11-26 20:29:29.264730 diff_cover-8.0.3/tests/fixtures/lua_console_report.txt
--rw-r--r--   0        0        0     1641 2023-11-26 20:29:29.264781 diff_cover-8.0.3/tests/fixtures/luacoverage.xml
--rw-r--r--   0        0        0      357 2023-11-26 20:29:29.264828 diff_cover-8.0.3/tests/fixtures/markdown_report_one_snippet.md
--rw-r--r--   0        0        0      469 2023-11-26 20:29:29.264896 diff_cover-8.0.3/tests/fixtures/markdown_report_two_snippets.md
--rw-r--r--   0        0        0      220 2023-11-26 20:29:29.264956 diff_cover-8.0.3/tests/fixtures/moved_console_report.txt
--rw-r--r--   0        0        0      855 2023-11-26 20:29:29.265021 diff_cover-8.0.3/tests/fixtures/moved_coverage.xml
--rw-r--r--   0        0        0     5234 2023-11-26 20:29:29.265087 diff_cover-8.0.3/tests/fixtures/moved_html_report.html
--rw-r--r--   0        0        0      218 2023-11-26 20:29:29.265141 diff_cover-8.0.3/tests/fixtures/mult_inputs_console_report.txt
--rw-r--r--   0        0        0     5207 2023-11-26 20:29:29.265191 diff_cover-8.0.3/tests/fixtures/mult_inputs_html_report.html
--rw-r--r--   0        0        0      262 2023-11-26 20:29:29.265248 diff_cover-8.0.3/tests/fixtures/pycodestyle_report.txt
--rw-r--r--   0        0        0     7135 2023-11-26 20:29:29.265330 diff_cover-8.0.3/tests/fixtures/pycodestyle_violations_report.html
--rw-r--r--   0        0        0      435 2023-11-26 20:29:29.265380 diff_cover-8.0.3/tests/fixtures/pycodestyle_violations_report.txt
--rw-r--r--   0        0        0     4434 2023-11-26 20:29:29.265473 diff_cover-8.0.3/tests/fixtures/pycodestyle_violations_report_external_css.html
--rw-r--r--   0        0        0      309 2023-11-26 20:29:29.265542 diff_cover-8.0.3/tests/fixtures/pyflakes_two_files.txt
--rw-r--r--   0        0        0     5810 2023-11-26 20:29:29.265606 diff_cover-8.0.3/tests/fixtures/pyflakes_violations_report.html
--rw-r--r--   0        0        0      314 2023-11-26 20:29:29.265663 diff_cover-8.0.3/tests/fixtures/pyflakes_violations_report.txt
--rw-r--r--   0        0        0     3172 2023-11-26 20:29:29.265729 diff_cover-8.0.3/tests/fixtures/pylint_dupe.txt
--rw-r--r--   0        0        0      284 2023-11-26 20:29:29.265803 diff_cover-8.0.3/tests/fixtures/pylint_dupe_violations_report.txt
--rw-r--r--   0        0        0     2884 2023-11-26 20:29:29.265867 diff_cover-8.0.3/tests/fixtures/pylint_report.txt
--rw-r--r--   0        0        0      516 2023-11-26 20:29:29.265927 diff_cover-8.0.3/tests/fixtures/pylint_violations_console_report.txt
--rw-r--r--   0        0        0     7583 2023-11-26 20:29:29.265977 diff_cover-8.0.3/tests/fixtures/pylint_violations_report.html
--rw-r--r--   0        0        0      418 2023-11-26 20:29:29.266017 diff_cover-8.0.3/tests/fixtures/pylint_violations_report.txt
--rw-r--r--   0        0        0        0 2023-11-26 20:29:29.266039 diff_cover-8.0.3/tests/fixtures/pylintrc
--rw-r--r--   0        0        0      379 2023-11-26 20:29:29.266093 diff_cover-8.0.3/tests/fixtures/show_uncovered_lines_console.txt
--rw-r--r--   0        0        0      355 2023-11-26 20:29:29.266138 diff_cover-8.0.3/tests/fixtures/snippet.css
--rw-r--r--   0        0        0      106 2023-11-26 20:29:29.266203 diff_cover-8.0.3/tests/fixtures/snippet_8859.py
--rw-r--r--   0        0        0     1410 2023-11-26 20:29:29.266263 diff_cover-8.0.3/tests/fixtures/snippet_arabic_output.html
--rw-r--r--   0        0        0      864 2023-11-26 20:29:29.266311 diff_cover-8.0.3/tests/fixtures/snippet_default.html
--rw-r--r--   0        0        0      814 2023-11-26 20:29:29.266364 diff_cover-8.0.3/tests/fixtures/snippet_invalid_violations.html
--rw-r--r--   0        0        0     4525 2023-11-26 20:29:29.266421 diff_cover-8.0.3/tests/fixtures/snippet_list.html
--rw-r--r--   0        0        0      275 2023-11-26 20:29:29.266469 diff_cover-8.0.3/tests/fixtures/snippet_list.md
--rw-r--r--   0        0        0      105 2023-11-26 20:29:29.266512 diff_cover-8.0.3/tests/fixtures/snippet_list2.md
--rw-r--r--   0        0        0      126 2023-11-26 20:29:29.266555 diff_cover-8.0.3/tests/fixtures/snippet_list3.md
--rw-r--r--   0        0        0      840 2023-11-26 20:29:29.266597 diff_cover-8.0.3/tests/fixtures/snippet_no_filename_ext.html
--rw-r--r--   0        0        0      791 2023-11-26 20:29:29.266637 diff_cover-8.0.3/tests/fixtures/snippet_src.py
--rw-r--r--   0        0        0       83 2023-11-26 20:29:29.266683 diff_cover-8.0.3/tests/fixtures/snippet_src2.cpp
--rw-r--r--   0        0        0      264 2023-11-26 20:29:29.266736 diff_cover-8.0.3/tests/fixtures/snippet_src3.cpp
--rw-r--r--   0        0        0      279 2023-11-26 20:29:29.266802 diff_cover-8.0.3/tests/fixtures/snippet_unicode.html
--rw-r--r--   0        0        0      888 2023-11-26 20:29:29.266849 diff_cover-8.0.3/tests/fixtures/snippet_unicode.py
--rw-r--r--   0        0        0     4749 2023-11-26 20:29:29.266900 diff_cover-8.0.3/tests/fixtures/snippet_unicode_html_output.html
--rw-r--r--   0        0        0      224 2023-11-26 20:29:29.266948 diff_cover-8.0.3/tests/fixtures/subdir_coverage_console_report.txt
--rw-r--r--   0        0        0     5282 2023-11-26 20:29:29.267000 diff_cover-8.0.3/tests/fixtures/subdir_coverage_html_report.html
--rw-r--r--   0        0        0       71 2023-11-26 20:29:29.267041 diff_cover-8.0.3/tests/fixtures/test_src.txt
--rw-r--r--   0        0        0      228 2023-11-26 20:29:29.267087 diff_cover-8.0.3/tests/fixtures/unicode_console_report.txt
--rw-r--r--   0        0        0      871 2023-11-26 20:29:29.267131 diff_cover-8.0.3/tests/fixtures/unicode_coverage.xml
--rw-r--r--   0        0        0     5400 2023-11-26 20:29:29.267187 diff_cover-8.0.3/tests/fixtures/unicode_html_report.html
--rw-r--r--   0        0        0      141 2023-11-26 20:29:29.267231 diff_cover-8.0.3/tests/fixtures/unicode_test_src.txt
--rw-r--r--   0        0        0      302 2023-11-26 20:29:29.267276 diff_cover-8.0.3/tests/fixtures/violations_test_file.py
--rw-r--r--   0        0        0     5801 2023-11-26 20:29:29.267335 diff_cover-8.0.3/tests/helpers.py
--rw-r--r--   0        0        0     3055 2023-11-26 20:29:29.267383 diff_cover-8.0.3/tests/snippet_list_unicode.html
--rw-r--r--   0        0        0     1575 2023-11-26 20:29:29.267507 diff_cover-8.0.3/tests/test_clover_violations_reporter/test.xml
--rw-r--r--   0        0        0      690 2023-11-26 20:29:29.267438 diff_cover-8.0.3/tests/test_clover_violations_reporter.py
--rw-r--r--   0        0        0     3066 2023-11-26 20:29:29.267562 diff_cover-8.0.3/tests/test_config_parser.py
--rw-r--r--   0        0        0     1018 2023-11-26 20:29:29.267617 diff_cover-8.0.3/tests/test_diff_cover_main.py
--rw-r--r--   0        0        0     2511 2023-11-26 20:29:29.267672 diff_cover-8.0.3/tests/test_diff_cover_tool.py
--rw-r--r--   0        0        0     4099 2023-11-26 20:29:29.267742 diff_cover-8.0.3/tests/test_diff_quality_main.py
--rw-r--r--   0        0        0    20454 2023-11-26 20:29:29.267844 diff_cover-8.0.3/tests/test_diff_reporter.py
--rw-r--r--   0        0        0     5243 2023-11-26 20:29:29.268071 diff_cover-8.0.3/tests/test_git_diff.py
--rw-r--r--   0        0        0     2703 2023-11-26 20:29:29.268133 diff_cover-8.0.3/tests/test_git_path.py
--rw-r--r--   0        0        0    21071 2023-11-26 20:29:29.268213 diff_cover-8.0.3/tests/test_integration.py
--rw-r--r--   0        0        0    22017 2023-11-26 20:29:29.268361 diff_cover-8.0.3/tests/test_java_violations_reporter.py
--rw-r--r--   0        0        0    18248 2023-11-26 20:29:29.268458 diff_cover-8.0.3/tests/test_report_generator.py
--rw-r--r--   0        0        0     8462 2023-11-26 20:29:29.268579 diff_cover-8.0.3/tests/test_snippets.py
--rw-r--r--   0        0        0      356 2023-11-26 20:29:29.268631 diff_cover-8.0.3/tests/test_util.py
--rw-r--r--   0        0        0    65432 2023-11-26 20:29:29.268709 diff_cover-8.0.3/tests/test_violations_reporter.py
--rw-r--r--   0        0        0    17011 1970-01-01 00:00:00.000000 diff_cover-8.0.3/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-11-26 20:29:29.260372 diff_cover-9.0.0/LICENSE
+-rw-r--r--   0        0        0    15616 2023-11-26 20:29:29.260610 diff_cover-9.0.0/README.rst
+-rw-r--r--   0        0        0      417 2023-11-26 20:29:29.260689 diff_cover-9.0.0/diff_cover/__init__.py
+-rw-r--r--   0        0        0     2084 2024-03-23 22:43:34.376780 diff_cover-9.0.0/diff_cover/command_runner.py
+-rw-r--r--   0        0        0     2295 2023-11-26 20:29:29.260788 diff_cover-9.0.0/diff_cover/config_parser.py
+-rw-r--r--   0        0        0     9236 2023-11-26 20:29:29.260871 diff_cover-9.0.0/diff_cover/diff_cover_tool.py
+-rw-r--r--   0        0        0    11548 2023-11-26 20:29:29.260924 diff_cover-9.0.0/diff_cover/diff_quality_tool.py
+-rw-r--r--   0        0        0    16719 2024-03-23 22:43:34.377090 diff_cover-9.0.0/diff_cover/diff_reporter.py
+-rw-r--r--   0        0        0     3840 2024-03-23 22:43:34.377407 diff_cover-9.0.0/diff_cover/git_diff.py
+-rw-r--r--   0        0        0     2037 2024-03-23 22:43:34.377684 diff_cover-9.0.0/diff_cover/git_path.py
+-rw-r--r--   0        0        0      123 2023-11-26 20:29:29.261176 diff_cover-9.0.0/diff_cover/hook.py
+-rw-r--r--   0        0        0      240 2023-11-26 20:29:29.261228 diff_cover-9.0.0/diff_cover/hookspecs.py
+-rw-r--r--   0        0        0    14360 2024-03-23 22:43:34.378272 diff_cover-9.0.0/diff_cover/report_generator.py
+-rw-r--r--   0        0        0    14560 2024-04-14 20:05:38.515375 diff_cover-9.0.0/diff_cover/snippets.py
+-rw-r--r--   0        0        0      742 2023-11-26 20:29:29.261581 diff_cover-9.0.0/diff_cover/templates/console_coverage_report.txt
+-rw-r--r--   0        0        0      787 2023-11-26 20:29:29.261628 diff_cover-9.0.0/diff_cover/templates/console_quality_report.txt
+-rw-r--r--   0        0        0      174 2023-11-26 20:29:29.261682 diff_cover-9.0.0/diff_cover/templates/external_style.css
+-rw-r--r--   0        0        0     1632 2023-11-26 20:29:29.261734 diff_cover-9.0.0/diff_cover/templates/html_coverage_report.html
+-rw-r--r--   0        0        0     1880 2023-11-26 20:29:29.261788 diff_cover-9.0.0/diff_cover/templates/html_quality_report.html
+-rw-r--r--   0        0        0      759 2023-11-26 20:29:29.261841 diff_cover-9.0.0/diff_cover/templates/markdown_coverage_report.md
+-rw-r--r--   0        0        0      754 2023-11-26 20:29:29.261889 diff_cover-9.0.0/diff_cover/templates/markdown_quality_report.md
+-rw-r--r--   0        0        0      371 2023-11-26 20:29:29.261939 diff_cover-9.0.0/diff_cover/templates/snippet_content.html
+-rw-r--r--   0        0        0      229 2023-11-26 20:29:29.261985 diff_cover-9.0.0/diff_cover/templates/snippet_content.md
+-rw-r--r--   0        0        0      204 2023-11-26 20:29:29.262029 diff_cover-9.0.0/diff_cover/templates/snippet_content.txt
+-rw-r--r--   0        0        0      419 2023-11-26 20:29:29.262077 diff_cover-9.0.0/diff_cover/templates/snippet_style.html
+-rw-r--r--   0        0        0      687 2023-11-26 20:29:29.262143 diff_cover-9.0.0/diff_cover/util.py
+-rw-r--r--   0        0        0        0 2023-11-26 20:29:29.262194 diff_cover-9.0.0/diff_cover/violationsreporters/__init__.py
+-rw-r--r--   0        0        0     8455 2023-11-26 20:29:29.262266 diff_cover-9.0.0/diff_cover/violationsreporters/base.py
+-rw-r--r--   0        0        0     5837 2023-11-26 20:29:29.262333 diff_cover-9.0.0/diff_cover/violationsreporters/java_violations_reporter.py
+-rw-r--r--   0        0        0    26028 2023-11-26 20:29:29.262416 diff_cover-9.0.0/diff_cover/violationsreporters/violations_reporter.py
+-rw-r--r--   0        0        0     3465 2024-04-14 20:06:47.733014 diff_cover-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-26 20:29:29.262806 diff_cover-9.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      220 2023-11-26 20:29:29.262912 diff_cover-9.0.0/tests/fixtures/add_console_report.txt
+-rw-r--r--   0        0        0     5234 2023-11-26 20:29:29.262985 diff_cover-9.0.0/tests/fixtures/add_html_report.html
+-rw-r--r--   0        0        0      192 2023-11-26 20:29:29.263033 diff_cover-9.0.0/tests/fixtures/changed_console_report.txt
+-rw-r--r--   0        0        0     4372 2023-11-26 20:29:29.263086 diff_cover-9.0.0/tests/fixtures/changed_html_report.html
+-rw-r--r--   0        0        0      855 2023-11-26 20:29:29.263152 diff_cover-9.0.0/tests/fixtures/coverage.xml
+-rw-r--r--   0        0        0      855 2023-11-26 20:29:29.263214 diff_cover-9.0.0/tests/fixtures/coverage1.xml
+-rw-r--r--   0        0        0      855 2023-11-26 20:29:29.263289 diff_cover-9.0.0/tests/fixtures/coverage2.xml
+-rw-r--r--   0        0        0      159 2023-11-26 20:29:29.263355 diff_cover-9.0.0/tests/fixtures/delete_console_report.txt
+-rw-r--r--   0        0        0     3946 2023-11-26 20:29:29.263405 diff_cover-9.0.0/tests/fixtures/delete_html_report.html
+-rw-r--r--   0        0        0     2664 2023-11-26 20:29:29.263455 diff_cover-9.0.0/tests/fixtures/dotnet_coverage.xml
+-rw-r--r--   0        0        0      219 2023-11-26 20:29:29.263498 diff_cover-9.0.0/tests/fixtures/dotnet_coverage_console_report.txt
+-rw-r--r--   0        0        0        0 2023-11-26 20:29:29.263517 diff_cover-9.0.0/tests/fixtures/empty.txt
+-rw-r--r--   0        0        0      235 2023-11-26 20:29:29.263577 diff_cover-9.0.0/tests/fixtures/empty_pycodestyle_violations.txt
+-rw-r--r--   0        0        0      913 2023-11-26 20:29:29.263632 diff_cover-9.0.0/tests/fixtures/external_css_html_report.html
+-rw-r--r--   0        0        0     3400 2023-11-26 20:29:29.263691 diff_cover-9.0.0/tests/fixtures/external_style.css
+-rw-r--r--   0        0        0      216 2023-11-26 20:29:29.263749 diff_cover-9.0.0/tests/fixtures/git_diff_add.txt
+-rw-r--r--   0        0        0      216 2023-11-26 20:29:29.263798 diff_cover-9.0.0/tests/fixtures/git_diff_changed.txt
+-rw-r--r--   0        0        0      560 2023-11-26 20:29:29.263851 diff_cover-9.0.0/tests/fixtures/git_diff_code_dupe.txt
+-rw-r--r--   0        0        0      220 2023-11-26 20:29:29.263898 diff_cover-9.0.0/tests/fixtures/git_diff_delete.txt
+-rw-r--r--   0        0        0      365 2023-11-26 20:29:29.263952 diff_cover-9.0.0/tests/fixtures/git_diff_dotnet.txt
+-rw-r--r--   0        0        0      216 2023-11-26 20:29:29.264000 diff_cover-9.0.0/tests/fixtures/git_diff_external_css.txt
+-rw-r--r--   0        0        0      259 2023-11-26 20:29:29.264050 diff_cover-9.0.0/tests/fixtures/git_diff_lua.txt
+-rw-r--r--   0        0        0      216 2023-11-26 20:29:29.264095 diff_cover-9.0.0/tests/fixtures/git_diff_moved.txt
+-rw-r--r--   0        0        0      216 2023-11-26 20:29:29.264136 diff_cover-9.0.0/tests/fixtures/git_diff_mult.txt
+-rw-r--r--   0        0        0      228 2023-11-26 20:29:29.264183 diff_cover-9.0.0/tests/fixtures/git_diff_subdir.txt
+-rw-r--r--   0        0        0      310 2023-11-26 20:29:29.264226 diff_cover-9.0.0/tests/fixtures/git_diff_unicode.txt
+-rw-r--r--   0        0        0      543 2023-11-26 20:29:29.264274 diff_cover-9.0.0/tests/fixtures/git_diff_violations.txt
+-rw-r--r--   0        0        0      266 2023-11-26 20:29:29.264320 diff_cover-9.0.0/tests/fixtures/git_diff_violations_two_files.txt
+-rw-r--r--   0        0        0       33 2023-11-26 20:29:29.264360 diff_cover-9.0.0/tests/fixtures/hello.py
+-rw-r--r--   0        0        0       33 2023-11-26 20:29:29.264402 diff_cover-9.0.0/tests/fixtures/hi.py
+-rw-r--r--   0        0        0     1237 2023-11-26 20:29:29.264453 diff_cover-9.0.0/tests/fixtures/html_report.html
+-rw-r--r--   0        0        0      677 2023-11-26 20:29:29.264505 diff_cover-9.0.0/tests/fixtures/html_report_empty.html
+-rw-r--r--   0        0        0     1652 2023-11-26 20:29:29.264553 diff_cover-9.0.0/tests/fixtures/html_report_one_snippet.html
+-rw-r--r--   0        0        0     1756 2023-11-26 20:29:29.264618 diff_cover-9.0.0/tests/fixtures/html_report_two_snippets.html
+-rw-r--r--   0        0        0      232 2023-11-26 20:29:29.264667 diff_cover-9.0.0/tests/fixtures/lcov.info
+-rw-r--r--   0        0        0      214 2023-11-26 20:29:29.264730 diff_cover-9.0.0/tests/fixtures/lua_console_report.txt
+-rw-r--r--   0        0        0     1641 2023-11-26 20:29:29.264781 diff_cover-9.0.0/tests/fixtures/luacoverage.xml
+-rw-r--r--   0        0        0      357 2023-11-26 20:29:29.264828 diff_cover-9.0.0/tests/fixtures/markdown_report_one_snippet.md
+-rw-r--r--   0        0        0      469 2023-11-26 20:29:29.264896 diff_cover-9.0.0/tests/fixtures/markdown_report_two_snippets.md
+-rw-r--r--   0        0        0      220 2023-11-26 20:29:29.264956 diff_cover-9.0.0/tests/fixtures/moved_console_report.txt
+-rw-r--r--   0        0        0      855 2023-11-26 20:29:29.265021 diff_cover-9.0.0/tests/fixtures/moved_coverage.xml
+-rw-r--r--   0        0        0     5234 2023-11-26 20:29:29.265087 diff_cover-9.0.0/tests/fixtures/moved_html_report.html
+-rw-r--r--   0        0        0      218 2023-11-26 20:29:29.265141 diff_cover-9.0.0/tests/fixtures/mult_inputs_console_report.txt
+-rw-r--r--   0        0        0     5207 2023-11-26 20:29:29.265191 diff_cover-9.0.0/tests/fixtures/mult_inputs_html_report.html
+-rw-r--r--   0        0        0      262 2023-11-26 20:29:29.265248 diff_cover-9.0.0/tests/fixtures/pycodestyle_report.txt
+-rw-r--r--   0        0        0     7135 2023-11-26 20:29:29.265330 diff_cover-9.0.0/tests/fixtures/pycodestyle_violations_report.html
+-rw-r--r--   0        0        0      435 2023-11-26 20:29:29.265380 diff_cover-9.0.0/tests/fixtures/pycodestyle_violations_report.txt
+-rw-r--r--   0        0        0     4434 2023-11-26 20:29:29.265473 diff_cover-9.0.0/tests/fixtures/pycodestyle_violations_report_external_css.html
+-rw-r--r--   0        0        0      309 2023-11-26 20:29:29.265542 diff_cover-9.0.0/tests/fixtures/pyflakes_two_files.txt
+-rw-r--r--   0        0        0     5810 2023-11-26 20:29:29.265606 diff_cover-9.0.0/tests/fixtures/pyflakes_violations_report.html
+-rw-r--r--   0        0        0      314 2023-11-26 20:29:29.265663 diff_cover-9.0.0/tests/fixtures/pyflakes_violations_report.txt
+-rw-r--r--   0        0        0     3172 2023-11-26 20:29:29.265729 diff_cover-9.0.0/tests/fixtures/pylint_dupe.txt
+-rw-r--r--   0        0        0      284 2023-11-26 20:29:29.265803 diff_cover-9.0.0/tests/fixtures/pylint_dupe_violations_report.txt
+-rw-r--r--   0        0        0     2884 2023-11-26 20:29:29.265867 diff_cover-9.0.0/tests/fixtures/pylint_report.txt
+-rw-r--r--   0        0        0      516 2023-11-26 20:29:29.265927 diff_cover-9.0.0/tests/fixtures/pylint_violations_console_report.txt
+-rw-r--r--   0        0        0     7583 2023-11-26 20:29:29.265977 diff_cover-9.0.0/tests/fixtures/pylint_violations_report.html
+-rw-r--r--   0        0        0      418 2023-11-26 20:29:29.266017 diff_cover-9.0.0/tests/fixtures/pylint_violations_report.txt
+-rw-r--r--   0        0        0        0 2023-11-26 20:29:29.266039 diff_cover-9.0.0/tests/fixtures/pylintrc
+-rw-r--r--   0        0        0      379 2023-11-26 20:29:29.266093 diff_cover-9.0.0/tests/fixtures/show_uncovered_lines_console.txt
+-rw-r--r--   0        0        0      355 2023-11-26 20:29:29.266138 diff_cover-9.0.0/tests/fixtures/snippet.css
+-rw-r--r--   0        0        0      106 2023-11-26 20:29:29.266203 diff_cover-9.0.0/tests/fixtures/snippet_8859.py
+-rw-r--r--   0        0        0     1410 2023-11-26 20:29:29.266263 diff_cover-9.0.0/tests/fixtures/snippet_arabic_output.html
+-rw-r--r--   0        0        0      864 2023-11-26 20:29:29.266311 diff_cover-9.0.0/tests/fixtures/snippet_default.html
+-rw-r--r--   0        0        0      814 2023-11-26 20:29:29.266364 diff_cover-9.0.0/tests/fixtures/snippet_invalid_violations.html
+-rw-r--r--   0        0        0     4525 2023-11-26 20:29:29.266421 diff_cover-9.0.0/tests/fixtures/snippet_list.html
+-rw-r--r--   0        0        0      415 2024-04-14 20:05:38.516405 diff_cover-9.0.0/tests/fixtures/snippet_list.md
+-rw-r--r--   0        0        0      129 2024-04-14 20:05:38.516559 diff_cover-9.0.0/tests/fixtures/snippet_list2.md
+-rw-r--r--   0        0        0      171 2024-04-14 20:05:38.516722 diff_cover-9.0.0/tests/fixtures/snippet_list3.md
+-rw-r--r--   0        0        0      840 2023-11-26 20:29:29.266597 diff_cover-9.0.0/tests/fixtures/snippet_no_filename_ext.html
+-rw-r--r--   0        0        0      791 2023-11-26 20:29:29.266637 diff_cover-9.0.0/tests/fixtures/snippet_src.py
+-rw-r--r--   0        0        0       83 2023-11-26 20:29:29.266683 diff_cover-9.0.0/tests/fixtures/snippet_src2.cpp
+-rw-r--r--   0        0        0      264 2023-11-26 20:29:29.266736 diff_cover-9.0.0/tests/fixtures/snippet_src3.cpp
+-rw-r--r--   0        0        0      279 2023-11-26 20:29:29.266802 diff_cover-9.0.0/tests/fixtures/snippet_unicode.html
+-rw-r--r--   0        0        0      888 2023-11-26 20:29:29.266849 diff_cover-9.0.0/tests/fixtures/snippet_unicode.py
+-rw-r--r--   0        0        0     4749 2023-11-26 20:29:29.266900 diff_cover-9.0.0/tests/fixtures/snippet_unicode_html_output.html
+-rw-r--r--   0        0        0      224 2023-11-26 20:29:29.266948 diff_cover-9.0.0/tests/fixtures/subdir_coverage_console_report.txt
+-rw-r--r--   0        0        0     5282 2023-11-26 20:29:29.267000 diff_cover-9.0.0/tests/fixtures/subdir_coverage_html_report.html
+-rw-r--r--   0        0        0       71 2023-11-26 20:29:29.267041 diff_cover-9.0.0/tests/fixtures/test_src.txt
+-rw-r--r--   0        0        0      228 2023-11-26 20:29:29.267087 diff_cover-9.0.0/tests/fixtures/unicode_console_report.txt
+-rw-r--r--   0        0        0      871 2023-11-26 20:29:29.267131 diff_cover-9.0.0/tests/fixtures/unicode_coverage.xml
+-rw-r--r--   0        0        0     5400 2023-11-26 20:29:29.267187 diff_cover-9.0.0/tests/fixtures/unicode_html_report.html
+-rw-r--r--   0        0        0      141 2023-11-26 20:29:29.267231 diff_cover-9.0.0/tests/fixtures/unicode_test_src.txt
+-rw-r--r--   0        0        0      302 2023-11-26 20:29:29.267276 diff_cover-9.0.0/tests/fixtures/violations_test_file.py
+-rw-r--r--   0        0        0     5802 2024-03-23 22:43:34.379183 diff_cover-9.0.0/tests/helpers.py
+-rw-r--r--   0        0        0     3055 2023-11-26 20:29:29.267383 diff_cover-9.0.0/tests/snippet_list_unicode.html
+-rw-r--r--   0        0        0     1575 2023-11-26 20:29:29.267507 diff_cover-9.0.0/tests/test_clover_violations_reporter/test.xml
+-rw-r--r--   0        0        0      690 2023-11-26 20:29:29.267438 diff_cover-9.0.0/tests/test_clover_violations_reporter.py
+-rw-r--r--   0        0        0     3066 2023-11-26 20:29:29.267562 diff_cover-9.0.0/tests/test_config_parser.py
+-rw-r--r--   0        0        0     1018 2023-11-26 20:29:29.267617 diff_cover-9.0.0/tests/test_diff_cover_main.py
+-rw-r--r--   0        0        0     2511 2023-11-26 20:29:29.267672 diff_cover-9.0.0/tests/test_diff_cover_tool.py
+-rw-r--r--   0        0        0     4099 2023-11-26 20:29:29.267742 diff_cover-9.0.0/tests/test_diff_quality_main.py
+-rw-r--r--   0        0        0    20454 2023-11-26 20:29:29.267844 diff_cover-9.0.0/tests/test_diff_reporter.py
+-rw-r--r--   0        0        0     5243 2023-11-26 20:29:29.268071 diff_cover-9.0.0/tests/test_git_diff.py
+-rw-r--r--   0        0        0     2703 2023-11-26 20:29:29.268133 diff_cover-9.0.0/tests/test_git_path.py
+-rw-r--r--   0        0        0    21071 2023-11-26 20:29:29.268213 diff_cover-9.0.0/tests/test_integration.py
+-rw-r--r--   0        0        0    22017 2023-11-26 20:29:29.268361 diff_cover-9.0.0/tests/test_java_violations_reporter.py
+-rw-r--r--   0        0        0    18248 2023-11-26 20:29:29.268458 diff_cover-9.0.0/tests/test_report_generator.py
+-rw-r--r--   0        0        0     8462 2023-11-26 20:29:29.268579 diff_cover-9.0.0/tests/test_snippets.py
+-rw-r--r--   0        0        0      356 2023-11-26 20:29:29.268631 diff_cover-9.0.0/tests/test_util.py
+-rw-r--r--   0        0        0    65432 2023-11-26 20:29:29.268709 diff_cover-9.0.0/tests/test_violations_reporter.py
+-rw-r--r--   0        0        0    17011 1970-01-01 00:00:00.000000 diff_cover-9.0.0/PKG-INFO
```

### Comparing `diff_cover-8.0.3/LICENSE` & `diff_cover-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/README.rst` & `diff_cover-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/command_runner.py` & `diff_cover-9.0.0/diff_cover/command_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,19 @@
     process = subprocess.Popen(command, stdout=stdout_pipe, stderr=stdout_pipe)
     try:
         stdout, stderr = process.communicate()
     except OSError:
         sys.stderr.write(
             " ".join(
                 [
-                    cmd.decode(sys.getfilesystemencoding())
-                    if isinstance(cmd, bytes)
-                    else cmd
+                    (
+                        cmd.decode(sys.getfilesystemencoding())
+                        if isinstance(cmd, bytes)
+                        else cmd
+                    )
                     for cmd in command
                 ]
             )
         )
         raise
 
     stderr = _ensure_unicode(stderr)
```

### Comparing `diff_cover-8.0.3/diff_cover/config_parser.py` & `diff_cover-9.0.0/diff_cover/config_parser.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/diff_cover_tool.py` & `diff_cover-9.0.0/diff_cover/diff_cover_tool.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/diff_quality_tool.py` & `diff_cover-9.0.0/diff_cover/diff_quality_tool.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/diff_reporter.py` & `diff_cover-9.0.0/diff_cover/diff_reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Classes for querying which lines have changed based on a diff.
 """
+
 import fnmatch
 import glob
 import os
 import re
 from abc import ABC, abstractmethod
 
 from diff_cover.git_diff import GitDiffError
```

### Comparing `diff_cover-8.0.3/diff_cover/git_diff.py` & `diff_cover-9.0.0/diff_cover/git_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Wrapper for `git diff` command.
 """
+
 from textwrap import dedent
 
 from diff_cover.command_runner import CommandError, execute
 
 
 class GitDiffError(Exception):
     """
```

### Comparing `diff_cover-8.0.3/diff_cover/git_path.py` & `diff_cover-9.0.0/diff_cover/git_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Converter for `git diff` paths
 """
+
 import os
 import sys
 
 from diff_cover.command_runner import execute
 
 
 class GitPathTool:
```

### Comparing `diff_cover-8.0.3/diff_cover/report_generator.py` & `diff_cover-9.0.0/diff_cover/report_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Classes for generating diff coverage reports.
 """
+
 import contextlib
 import json
 import os
 from abc import ABC, abstractmethod
 from gettext import gettext, ngettext
 
 from jinja2 import Environment, PackageLoader, select_autoescape
```

### Comparing `diff_cover-8.0.3/diff_cover/snippets.py` & `diff_cover-9.0.0/diff_cover/snippets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Load snippets from source files to show violation lines
 in HTML reports.
 """
+
 import contextlib
 from tokenize import open as openpy
 
 import chardet
 import pygments
 from pygments.formatters.html import HtmlFormatter
 from pygments.formatters.terminal import TerminalFormatter
@@ -111,26 +112,41 @@
         return pygments.format(self.src_tokens(), formatter)
 
     def markdown(self):
         """
         Return a Markdown representation of the snippet using Markdown fenced code blocks.
         See https://github.github.com/gfm/#fenced-code-blocks.
         """
+
+        line_number_length = len(str(self._last_line))
+
+        text = ""
+        for i, line in enumerate(self.text().splitlines(), start=self._start_line):
+            if i > self._start_line:
+                text += "\n"
+
+            notice = " "
+            if i in self._violation_lines:
+                notice = "!"
+
+            format_string = "{} {:>" + str(line_number_length) + "} {}"
+            text += format_string.format(notice, i, line)
+
         header = "Lines %d-%d\n\n" % (self._start_line, self._last_line)
         if self._lexer_name in self.LEXER_TO_MARKDOWN_CODE_HINT:
             return header + (
                 "```"
                 + self.LEXER_TO_MARKDOWN_CODE_HINT[self._lexer_name]
                 + "\n"
-                + self.text()
+                + text
                 + "\n```\n"
             )
 
         # unknown programming language, return a non-decorated fenced code block:
-        return "```\n" + self.text() + "\n```\n"
+        return "```\n" + text + "\n```\n"
 
     def terminal(self):
         """
         Return a Terminal-friendly (with ANSI color sequences) representation of the snippet.
         """
         formatter = TerminalFormatter(
             linenos=True,
```

### Comparing `diff_cover-8.0.3/diff_cover/templates/console_coverage_report.txt` & `diff_cover-9.0.0/diff_cover/templates/console_coverage_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/templates/console_quality_report.txt` & `diff_cover-9.0.0/diff_cover/templates/console_quality_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/templates/html_coverage_report.html` & `diff_cover-9.0.0/diff_cover/templates/html_coverage_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/templates/html_quality_report.html` & `diff_cover-9.0.0/diff_cover/templates/html_quality_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/templates/markdown_coverage_report.md` & `diff_cover-9.0.0/diff_cover/templates/markdown_coverage_report.md`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/templates/markdown_quality_report.md` & `diff_cover-9.0.0/diff_cover/templates/markdown_quality_report.md`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/util.py` & `diff_cover-9.0.0/diff_cover/util.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/violationsreporters/base.py` & `diff_cover-9.0.0/diff_cover/violationsreporters/base.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/violationsreporters/java_violations_reporter.py` & `diff_cover-9.0.0/diff_cover/violationsreporters/java_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/diff_cover/violationsreporters/violations_reporter.py` & `diff_cover-9.0.0/diff_cover/violationsreporters/violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/pyproject.toml` & `diff_cover-9.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "diff_cover"
-version = "8.0.3"
+version = "9.0.0"
 description = "Run coverage and linting reports on diffs"
 authors = ["See Contributors"]
 homepage = "https://github.com/Bachmann1234/diff-cover"
 repository = "https://github.com/Bachmann1234/diff-cover"
 license = "Apache-2.0"
 readme = "README.rst"
 classifiers=[
@@ -45,24 +45,24 @@
 Jinja2 = ">=2.7.1"
 pluggy = ">=0.13.1,<2"
 chardet = ">=3.0.0"
 tomli = {version = ">=1.2.1", optional = true}
 setuptools = { version = ">=17.0.0", python = "<3.8" }
 
 [tool.poetry.dev-dependencies]
-pytest-cov = "^4.1.0"
+pytest-cov = "^5.0.0"
 pytest-datadir = "^1.5.0"
-pytest-mock = "^3.12.0"
+pytest-mock = "^3.14.0"
 pycodestyle = ">=2.9.1"
 flake8 = "^5.0.4"
 pyflakes = "^2.5.0"
-pylint = "^3.0.3"
+pylint = "^3.1.0"
 pylint-pytest = "^1.1.7"
 pydocstyle = "^6.1.1"
-black = "^23.12.1"
+black = "^24.3.0"
 isort = "^5.13.2"
 doc8 = "1.1.1"
 
 [tool.poetry.extras]
 toml = ["tomli"]
 
 [build-system]
```

### Comparing `diff_cover-8.0.3/tests/fixtures/add_html_report.html` & `diff_cover-9.0.0/tests/fixtures/add_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/changed_html_report.html` & `diff_cover-9.0.0/tests/fixtures/changed_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/coverage.xml` & `diff_cover-9.0.0/tests/fixtures/coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/coverage1.xml` & `diff_cover-9.0.0/tests/fixtures/coverage1.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/coverage2.xml` & `diff_cover-9.0.0/tests/fixtures/coverage2.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/delete_html_report.html` & `diff_cover-9.0.0/tests/fixtures/delete_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/dotnet_coverage.xml` & `diff_cover-9.0.0/tests/fixtures/dotnet_coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/external_css_html_report.html` & `diff_cover-9.0.0/tests/fixtures/external_css_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/external_style.css` & `diff_cover-9.0.0/tests/fixtures/external_style.css`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/git_diff_code_dupe.txt` & `diff_cover-9.0.0/tests/fixtures/git_diff_code_dupe.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/git_diff_violations.txt` & `diff_cover-9.0.0/tests/fixtures/git_diff_violations.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/html_report.html` & `diff_cover-9.0.0/tests/fixtures/html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/html_report_empty.html` & `diff_cover-9.0.0/tests/fixtures/html_report_empty.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/html_report_one_snippet.html` & `diff_cover-9.0.0/tests/fixtures/html_report_one_snippet.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/html_report_two_snippets.html` & `diff_cover-9.0.0/tests/fixtures/html_report_two_snippets.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/luacoverage.xml` & `diff_cover-9.0.0/tests/fixtures/luacoverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/moved_coverage.xml` & `diff_cover-9.0.0/tests/fixtures/moved_coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/moved_html_report.html` & `diff_cover-9.0.0/tests/fixtures/moved_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/mult_inputs_html_report.html` & `diff_cover-9.0.0/tests/fixtures/mult_inputs_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pycodestyle_violations_report.html` & `diff_cover-9.0.0/tests/fixtures/pycodestyle_violations_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pycodestyle_violations_report_external_css.html` & `diff_cover-9.0.0/tests/fixtures/pycodestyle_violations_report_external_css.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pyflakes_violations_report.html` & `diff_cover-9.0.0/tests/fixtures/pyflakes_violations_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pylint_dupe.txt` & `diff_cover-9.0.0/tests/fixtures/pylint_dupe.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pylint_report.txt` & `diff_cover-9.0.0/tests/fixtures/pylint_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pylint_violations_console_report.txt` & `diff_cover-9.0.0/tests/fixtures/pylint_violations_console_report.txt`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/pylint_violations_report.html` & `diff_cover-9.0.0/tests/fixtures/pylint_violations_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_arabic_output.html` & `diff_cover-9.0.0/tests/fixtures/snippet_arabic_output.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_default.html` & `diff_cover-9.0.0/tests/fixtures/snippet_default.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_invalid_violations.html` & `diff_cover-9.0.0/tests/fixtures/snippet_invalid_violations.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_list.html` & `diff_cover-9.0.0/tests/fixtures/snippet_list.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_no_filename_ext.html` & `diff_cover-9.0.0/tests/fixtures/snippet_no_filename_ext.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_src.py` & `diff_cover-9.0.0/tests/fixtures/snippet_src.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_unicode.py` & `diff_cover-9.0.0/tests/fixtures/snippet_unicode.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/snippet_unicode_html_output.html` & `diff_cover-9.0.0/tests/fixtures/snippet_unicode_html_output.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/subdir_coverage_html_report.html` & `diff_cover-9.0.0/tests/fixtures/subdir_coverage_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/unicode_coverage.xml` & `diff_cover-9.0.0/tests/fixtures/unicode_coverage.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/fixtures/unicode_html_report.html` & `diff_cover-9.0.0/tests/fixtures/unicode_html_report.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/helpers.py` & `diff_cover-9.0.0/tests/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test helper functions.
 """
+
 import os.path
 import random
 
 HUNK_BUFFER = 2
 MAX_LINE_LENGTH = 300
 LINE_STRINGS = ["test", "+ has a plus sign", "- has a minus sign"]
```

### Comparing `diff_cover-8.0.3/tests/snippet_list_unicode.html` & `diff_cover-9.0.0/tests/snippet_list_unicode.html`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_clover_violations_reporter/test.xml` & `diff_cover-9.0.0/tests/test_clover_violations_reporter/test.xml`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_clover_violations_reporter.py` & `diff_cover-9.0.0/tests/test_clover_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_config_parser.py` & `diff_cover-9.0.0/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_diff_cover_main.py` & `diff_cover-9.0.0/tests/test_diff_cover_main.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_diff_cover_tool.py` & `diff_cover-9.0.0/tests/test_diff_cover_tool.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_diff_quality_main.py` & `diff_cover-9.0.0/tests/test_diff_quality_main.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_diff_reporter.py` & `diff_cover-9.0.0/tests/test_diff_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_git_diff.py` & `diff_cover-9.0.0/tests/test_git_diff.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_git_path.py` & `diff_cover-9.0.0/tests/test_git_path.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_integration.py` & `diff_cover-9.0.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_java_violations_reporter.py` & `diff_cover-9.0.0/tests/test_java_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_report_generator.py` & `diff_cover-9.0.0/tests/test_report_generator.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_snippets.py` & `diff_cover-9.0.0/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/tests/test_violations_reporter.py` & `diff_cover-9.0.0/tests/test_violations_reporter.py`

 * *Files identical despite different names*

### Comparing `diff_cover-8.0.3/PKG-INFO` & `diff_cover-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diff_cover
-Version: 8.0.3
+Version: 9.0.0
 Summary: Run coverage and linting reports on diffs
 Home-page: https://github.com/Bachmann1234/diff-cover
 License: Apache-2.0
 Author: See Contributors
 Requires-Python: >=3.8.10,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

