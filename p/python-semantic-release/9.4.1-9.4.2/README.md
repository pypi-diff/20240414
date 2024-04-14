# Comparing `tmp/python-semantic-release-9.4.1.tar.gz` & `tmp/python_semantic_release-9.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-9.4.1.tar", last modified: Sat Apr  6 19:50:33 2024, max compression
+gzip compressed data, was "python_semantic_release-9.4.2.tar", last modified: Sun Apr 14 01:45:40 2024, max compression
```

## Comparing `python-semantic-release-9.4.1.tar` & `python_semantic_release-9.4.2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.068435 python-semantic-release-9.4.1/
--rw-r--r--   0 root         (0) root         (0)      230 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5281 2024-04-06 19:50:33.068435 python-semantic-release-9.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.040435 python-semantic-release-9.4.1/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.040435 python-semantic-release-9.4.1/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    15332 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    13275 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    23320 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3501 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8866 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9689 2024-04-06 19:50:26.000000 python-semantic-release-9.4.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5281 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5538 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      613 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.044435 python-semantic-release-9.4.1/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-04-06 19:50:26.000000 python-semantic-release-9.4.1/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.044435 python-semantic-release-9.4.1/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.044435 python-semantic-release-9.4.1/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.048435 python-semantic-release-9.4.1/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4087 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1703 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    22111 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    16070 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2110 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.048435 python-semantic-release-9.4.1/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2609 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4393 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5777 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3194 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.032435 python-semantic-release-9.4.1/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.048435 python-semantic-release-9.4.1/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      379 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5635 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     4626 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)     9146 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10710 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6154 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 19:50:33.068435 python-semantic-release-9.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11474 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    28853 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     1107 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     8953 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13280 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)     4494 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6225 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3563 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5468 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     2129 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5952 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2483 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)     5363 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    22326 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    26340 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    13318 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     6070 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.353688 python_semantic_release-9.4.2/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.353688 python_semantic_release-9.4.2/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    15332 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    13289 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    28291 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8866 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9689 2024-04-14 01:45:34.000000 python_semantic_release-9.4.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5538 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-14 01:45:40.000000 python_semantic_release-9.4.2/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.357688 python_semantic_release-9.4.2/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-04-14 01:45:34.000000 python_semantic_release-9.4.2/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.357688 python_semantic_release-9.4.2/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    23015 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    17574 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.345687 python_semantic_release-9.4.2/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.361688 python_semantic_release-9.4.2/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.365688 python_semantic_release-9.4.2/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5232 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)    11004 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    11450 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    16297 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.365688 python_semantic_release-9.4.2/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.365688 python_semantic_release-9.4.2/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11528 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    28853 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     8953 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13292 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.369688 python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.373688 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.377688 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5840 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.377688 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.377688 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    10521 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    27246 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    34206 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    15576 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 01:45:40.381688 python_semantic_release-9.4.2/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2024-04-14 01:44:20.000000 python_semantic_release-9.4.2/tests/util.py
```

### Comparing `python-semantic-release-9.4.1/LICENSE` & `python_semantic_release-9.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/PKG-INFO` & `python_semantic_release-9.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.4.1
+Version: 9.4.2
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -26,21 +26,21 @@
 Requires-Dist: requests~=2.25
 Requires-Dist: jinja2~=3.1
 Requires-Dist: python-gitlab~=4.0
 Requires-Dist: tomlkit~=0.11
 Requires-Dist: dotty-dict~=1.3
 Requires-Dist: importlib-resources~=6.0
 Requires-Dist: pydantic~=2.0
-Requires-Dist: rich~=12.5
+Requires-Dist: rich~=13.0
 Requires-Dist: shellingham~=1.5
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.0; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc==0.5.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
-Requires-Dist: furo~=2023.3; extra == "docs"
+Requires-Dist: furo~=2024.1; extra == "docs"
 Provides-Extra: test
 Requires-Dist: coverage[toml]~=7.0; extra == "test"
 Requires-Dist: pytest~=7.0; extra == "test"
 Requires-Dist: pytest-env~=1.0; extra == "test"
 Requires-Dist: pytest-xdist~=3.0; extra == "test"
 Requires-Dist: pytest-mock~=3.0; extra == "test"
 Requires-Dist: pytest-lazy-fixture~=0.6.3; extra == "test"
```

### Comparing `python-semantic-release-9.4.1/README.rst` & `python_semantic_release-9.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/Makefile` & `python_semantic_release-9.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/algorithm.rst` & `python_semantic_release-9.4.2/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/automatic-releases/cronjobs.rst` & `python_semantic_release-9.4.2/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/automatic-releases/github-actions.rst` & `python_semantic_release-9.4.2/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/automatic-releases/index.rst` & `python_semantic_release-9.4.2/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/automatic-releases/travis.rst` & `python_semantic_release-9.4.2/docs/automatic-releases/travis.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/changelog_templates.rst` & `python_semantic_release-9.4.2/docs/changelog_templates.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/commands.rst` & `python_semantic_release-9.4.2/docs/commands.rst`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 Print the last released version based on the Git tags.  This flag is useful if you just
 want to see the released version without determining what the next version will be.
 Note if the version can not be found nothing will be printed.
 
 .. _cmd-version-option-print-last-released-tag:
 
 ``--print-last-released-tag``
-***************
+*****************************
 
 Same as the :ref:`cmd-version-option-print-last-released` flag but prints the
 complete tag name (ex. ``v1.0.0`` or ``py-v1.0.0``) instead of the raw version
 number (``1.0.0``).
 
 .. _cmd-version-option-force-level:
```

### Comparing `python-semantic-release-9.4.1/docs/commit-parsing.rst` & `python_semantic_release-9.4.2/docs/commit-parsing.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/conf.py` & `python_semantic_release-9.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/configuration.rst` & `python_semantic_release-9.4.2/docs/configuration.rst`

 * *Files 21% similar despite different names*

```diff
@@ -96,29 +96,35 @@
     specified by ``env`` is considered required.
 
 .. _config-settings:
 
 Settings
 --------
 
+----
+
 .. _config-root:
 
 ``[tool.semantic_release]``
 ***************************
 
+----
+
 .. _config-assets:
 
 ``assets (List[str])``
 """"""""""""""""""""""
 
 One or more paths to additional assets that should committed to the remote repository
 in addition to any files modified by writing the new version.
 
 **Default:** ``[]``
 
+----
+
 .. _config-branches:
 
 ``branches``
 """"""""""""
 
 This setting is discussed in more detail at :ref:`multibranch-releases`
 
@@ -127,23 +133,27 @@
 .. code-block:: toml
 
     [tool.semantic_release.branches.main]
     match = "(main|master)"
     prerelease_token = "rc"
     prerelease = false
 
+----
+
 .. _config-build-command:
 
 ``build_command (Optional[str])``
 """""""""""""""""""""""""""""""""
 
 Command to use when building the current project during :ref:`cmd-version`
 
 **Default:** ``None`` (not specified)
 
+----
+
 .. _config-commit_author:
 
 ``commit_author (str)``
 """""""""""""""""""""""
 Author used in commits in the format ``name <email>``.
 
 .. note::
@@ -152,28 +162,32 @@
   ``git_committer_name`` and ``git_committer_name`` inputs.
 
 .. seealso::
    - :ref:`github-actions`
 
 **Default:** ``semantic-release <semantic-release>``
 
+----
+
 .. _config-commit-message:
 
 ``commit_message (str)``
 """"""""""""""""""""""""
 
 Commit message to use when making release commits. The message can use ``{version}``
 as a format key, in which case the version being released will be formatted into
 the message.
 
 If at some point in your project's lifetime you change this, you may wish to consider,
 adding the old message pattern(s) to :ref:`exclude_commit_patterns <config-changelog-exclude-commit-patterns>`.
 
 **Default:** ``"{version}\n\nAutomatically generated by python-semantic-release"``
 
+----
+
 .. _config-commit-parser:
 
 ``commit_parser (str)``
 """""""""""""""""""""""
 
 Specify which commit parser Python Semantic Release should use to parse the commits
 within the Git repository.
@@ -187,14 +201,16 @@
 You can set any of the built-in parsers by their keyword but you can also specify
 your own commit parser in ``module:attr`` form.
 
 For more information see :ref:`commit-parsing`.
 
 **Default:** ``"angular"``
 
+----
+
 .. _config-commit-parser-options:
 
 ``commit_parser_options (Dict[str, Any])``
 """"""""""""""""""""""""""""""""""""""""""
 
 These options are passed directly to the ``parser_options`` method of
 :ref:`the commit parser <config-commit-parser>`, without validation
@@ -254,24 +270,28 @@
 ``"module:class"``  ->   ``**module:class.parser_options()``
 ==================  ==   =================================
 
 **Default:** ``ParserOptions { ... }``, where ``...`` depends on
 :ref:`commit_parser <config-commit-parser>` as indicated above.
 
 
+----
+
 .. _config-logging-use-named-masks:
 
 ``logging_use_named_masks (bool)``
 """"""""""""""""""""""""""""""""""
 
 Whether or not to replace secrets identified in logging messages with named masks
 identifying which secrets were replaced, or use a generic string to mask them.
 
 **Default:** ``false``
 
+----
+
 .. _config-allow-zero-version:
 
 ``allow_zero_version (bool)``
 """""""""""""""""""""""""""""
 
 This flag controls whether or not Python Semantic Release will use version
 numbers aligning with the ``0.x.x`` pattern.
@@ -284,14 +304,16 @@
 If set to ``false``, Python Semantic Release will consider the first possible
 version to be ``1.0.0``, regardless of patch, minor, or major change level.
 Additionally, when ``allow_zero_version`` is set to ``false``,
 the :ref:`major_on_zero` setting is ignored.
 
 **Default:** ``true``
 
+----
+
 .. _config-major-on-zero:
 
 ``major_on_zero (bool)``
 """"""""""""""""""""""""
 
 This flag controls whether or not Python Semantic Release will increment the major
 version upon a breaking change when the version matches ``0.y.z``. This value is
@@ -312,14 +334,16 @@
 When you are ready to release a stable version, set ``major_on_zero`` to ``true`` and
 run Python Semantic Release again. This will increment the major version to ``1.0.0``.
 
 When :ref:`allow_zero_version` is set to ``false``, this setting is ignored.
 
 **Default:** ``true``
 
+----
+
 .. _config-tag-format:
 
 ``tag_format (str)``
 """"""""""""""""""""
 
 Specify the format to be used for the Git tag that will be added to the repo during
 a release invoked via :ref:`cmd-version`. The format string is a regular expression,
@@ -346,14 +370,16 @@
                             ``2.1.0-alpha.1+build.1234``
 ================ =========  ========
 
 Tags which do not match this format will not be considered as versions of your project.
 
 **Default:** ``"v{version}"``
 
+----
+
 .. _config-version-variables:
 
 ``version_variables (List[str])``
 """""""""""""""""""""""""""""""""
 
 Each entry represents a location where the version is stored in the source code,
 specified in ``file:variable`` format. For example:
@@ -364,14 +390,16 @@
     version_variables = [
         "semantic_release/__init__.py:__version__",
         "docs/conf.py:version",
     ]
 
 **Default:** ``[]``
 
+----
+
 .. _config-version-toml:
 
 ``version_toml (List[str])``
 """"""""""""""""""""""""""""
 Similar to :ref:`config-version-variables`, but allows the version number to be
 identified safely in a toml file like ``pyproject.toml``, with each entry using
 dotted notation to indicate the key for which the value represents the version:
@@ -381,40 +409,48 @@
     [tool.semantic_release]
     version_toml = [
         "pyproject.toml:tool.poetry.version",
     ]
 
 **Default:** ``[]``
 
+----
+
 .. _config-changelog:
 
 ``[tool.semantic_release.changelog]``
 *************************************
 
+----
+
 .. _config-changelog-template-dir:
 
 ``template_dir (str)``
 """"""""""""""""""""""
 
 If given, specifies a directory of templates that will be rendered during creation
 of the changelog. If not given, the default changelog template will be used.
 
 This option is discussed in more detail at :ref:`changelog-templates`
 
 **Default:** ``"templates"``
 
+----
+
 .. _config-changelog-changelog-file:
 
 ``changelog_file (str)``
 """"""""""""""""""""""""
 
 Specify the name of the changelog file (after template rendering has taken place).
 
 **Default:** ``"CHANGELOG.md"``
 
+----
+
 .. _config-changelog-exclude-commit-patterns:
 
 ``exclude_commit_patterns (List[str])``
 """""""""""""""""""""""""""""""""""""""
 
 Any patterns specified here will be excluded from the commits which are available
 to your changelog. This allows, for example, automated commits to be removed if desired.
@@ -422,144 +458,173 @@
 therefore if you change the automated commit message that Python Semantic Release uses when
 making commits, you may wish to add the *old* commit message pattern here.
 
 The patterns in this list are treated as regular expressions.
 
 **Default:** ``[]``
 
+----
+
 .. _config-changelog-environment:
 
 ``[tool.semantic_release.changelog.environment]``
 *************************************************
 
 .. note::
    This section of the configuration contains options which customize the template
    environment used to render templates such as the changelog. Most options are
    passed directly to the `jinja2.Environment`_ constructor, and further
    documentation one these parameters can be found there.
 
 .. _`jinja2.Environment`: https://jinja.palletsprojects.com/en/3.1.x/api/#jinja2.Environment
 
+----
+
 .. _config-changelog-environment-block-start-string:
 
 ``block_start_string (str)``
 """"""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``"{%"``
 
+----
+
 .. _config-changelog-environment-block-end-string:
 
 ``block_end_string (str)``
 """"""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``"%}"``
 
+----
+
 .. _config-changelog-environment-variable-start-string:
 
 ``variable_start_string (str)``
 """""""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``"{{"``
 
+----
+
 .. _config-changelog-environment-variable-end-string:
 
 ``variable_end_string (str)``
 """""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``"}}"``
 
+----
+
 .. _config-changelog-environment-comment-start-string:
 
 ``comment_start_string (str)``
 """"""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``{#``
 
+----
+
 .. _config-changelog-environment-comment-end-string:
 
 ``comment_end_string (str)``
 """"""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``"#}"``
 
+----
+
 .. _config-changelog-environment-line-statement-prefix:
 
 ``line_statement_prefix (Optional[str])``
 """""""""""""""""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``None`` (not specified)
 
+----
+
 .. _config-changelog-environment-line-comment-prefix:
 
 ``line_comment_prefix (Optional[str])``
 """""""""""""""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``None`` (not specified)
 
+----
+
 .. _config-changelog-environment-trim-blocks:
 
 ``trim_blocks (bool)``
 """"""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``false``
 
+----
+
 .. _config-changelog-environment-lstrip-blocks:
 
 ``lstrip_blocks (bool)``
 """"""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``false``
 
+----
+
 .. _config-changelog-environment-newline-sequence:
 
 ``newline_sequence (Literal["\n", "\r", "\r\n"])``
 """"""""""""""""""""""""""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``"\n"``
 
+----
+
 .. _config-changelog-environment-keep-trailing-newline:
 
 ``keep_trailing_newline (bool)``
 """"""""""""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``false``
 
+----
+
 .. _config-changelog-environment-extensions:
 
 ``extensions (List[str])``
 """"""""""""""""""""""""""
 
 This setting is passed directly to the `jinja2.Environment`_ constructor.
 
 **Default:** ``[]``
 
+----
 
 .. _config-changelog-environment-autoescape:
 
 ``autoescape (Union[str, bool])``
 """"""""""""""""""""""""""""""""""
 
 If this setting is a string, it should be given in ``module:attr`` form; Python
@@ -574,54 +639,194 @@
 constructor.
 
 If this setting is a boolean, it is passed directly to the `jinja2.Environment`_
 constructor.
 
 **Default:** ``true``
 
+----
+
 .. _config-remote:
 
-``[tool.semantic_release.remote]``
-**********************************
+``remote``
+**********
 
-.. _config-remote-name:
+.. note::
+    The remote configuration is a group of settings that configure PSR's integration
+    with remote version control systems.
+
+    **pyproject.toml:** ``[tool.semantic_release.remote]``
 
-``name (str)``
+----
+
+.. _config-remote-api_domain:
+
+``api_domain``
 """"""""""""""
 
-Name of the remote to push to using ``git push -u $name <branch_name>``
+**Type:** ``Optional[str | Dict['env', str]]``
 
-**Default:** ``"origin"``
+The hosting domain for the API of your remote HVCS if different than the ``domain``.
+Generally, this will be used to specify a separate subdomain that is used for API
+calls rather than the primary domain (ex. ``api.github.com``).
 
-.. _config-remote-type:
+**Most on-premise HVCS installations will NOT use this setting!** Whether or not
+this value is used depends on the HVCS configured (and your server administration)
+in the :ref:`remote.type <config-remote-type>` setting and used in tadem with the
+:ref:`remote.domain <config-remote-domain>` setting.
 
-``type (str)``
-""""""""""""""
+When using a custom :ref:`remote.domain <config-remote-domain>` and a HVCS
+:ref:`remote.type <config-remote-type>` that is configured with a separate domain
+or sub-domain for API requests, this value is used to configure the location of API
+requests that are sent from PSR.
 
-The type of the remote VCS. Currently, Python Semantic Release supports ``"github"``,
-``"gitlab"``, ``"gitea"`` and ``"bitbucket"``. Not all functionality is available with all
-remote types, but we welcome pull requests to help improve this!
+Most on-premise or self-hosted HVCS environments will use a path prefix to handle inbound
+API requests, which means this value will ignored.
 
-**Default:** ``"github"``
+PSR knows the expected api domains for known cloud services and their associated
+api domains which means this value is not necessary to explicitly define for services
+as ``bitbucket.org``, and ``github.com``.
+
+Including the protocol schemes, such as ``https://``, for the API domain is optional.
+Secure ``HTTPS`` connections are assumed unless the setting of
+:ref:`remote.insecure <config-remote-insecure>` is ``True``.
+
+**Default:** ``None``
+
+----
+
+.. _config-remote-domain:
+
+``domain``
+""""""""""
+
+**Type:** ``Optional[str | Dict['env', str]]``
+
+The host domain for your HVCS server. This setting is used to support on-premise
+installations of HVCS providers with custom domain hosts.
+
+If you are using the official domain of the associated
+:ref:`remote.type <config-remote-type>`, this value is not required. PSR will use the
+default domain value for the :ref:`remote.type <config-remote-type>` when not specified.
+For example, when ``remote.type="github"`` is specified the default domain of
+``github.com`` is used.
+
+Including the protocol schemes, such as ``https://``, for the domain value is optional.
+Secure ``HTTPS`` connections are assumed unless the setting of
+:ref:`remote.insecure <config-remote-insecure>` is ``True``.
+
+This setting also supports reading from an environment variable for ease-of-use
+in CI pipelines. See :ref:`Environment Variable <config-environment-variables>` for
+more information. Depending on the :ref:`remote.type <config-remote-type>`, the default
+environment variable for the default domain's CI pipeline environment will automatically
+be checked so this value is not required in default environments.  For example, when
+``remote.type="gitlab"`` is specified, PSR will look to the ``CI_SERVER_URL`` environment
+variable when ``remote.domain`` is not specified.
+
+**Default:** ``None``
+
+.. seealso::
+   - :ref:`remote.api_domain <config-remote-api-domain>`
+
+----
 
 .. _config-remote-ignore-token-for-push:
 
-``ignore_token_for_push (bool)``
-""""""""""""""""""""""""""""""""
+``ignore_token_for_push``
+"""""""""""""""""""""""""
+
+**Type:** ``bool``
 
 If set to ``True``, ignore the authentication token when pushing changes to the remote.
 This is ideal, for example, if you already have SSH keys set up which can be used for
 pushing.
 
 **Default:** ``False``
 
+----
+
+.. _config-remote-insecure:
+
+``insecure``
+""""""""""""
+
+**Type:** ``bool``
+
+Insecure is used to allow non-secure ``HTTP`` connections to your HVCS server. If set to
+``True``, any domain value passed will assume ``http://`` if it is not specified and allow
+it. When set to ``False`` (implicitly or explicitly), it will force ``https://`` communications.
+
+When a custom ``domain`` or ``api_domain`` is provided as a configuration, this flag governs
+the protocol scheme used for those connections. If the protocol scheme is not provided in
+the field value, then this ``insecure`` option defines whether ``HTTP`` or ``HTTPS`` is
+used for the connection. If the protocol scheme is provided in the field value, it must
+match this setting or it will throw an error.
+
+The purpose of this flag is to prevent any typos in provided ``domain`` and ``api_domain``
+values that accidently specify an insecure connection but allow users to toggle the protection
+scheme off when desired.
+
+**Default:** ``False``
+
+----
+
+.. _config-remote-name:
+
+``name``
+""""""""
+
+**Type:** ``str``
+
+Name of the remote to push to using ``git push -u $name <branch_name>``
+
+**Default:** ``"origin"``
+
+----
+
+.. _config-remote-url:
+
+``url``
+"""""""
+
+**Type:** ``Optional[str | Dict['env', str]]``
+
+An override setting used to specify the remote upstream location of ``git push``.
+
+**Not commonly used!** This is used to override the derived upstream location when
+the desired push location is different than the location the repository was cloned
+from.
+
+This setting will override the upstream location url that would normally be derived
+from the :ref:`remote.name <config-remote-name>` location of your git repository.
+
+**Default:** ``None``
+
+----
+
+.. _config-remote-type:
+
+``type``
+""""""""
+
+**Type:** ``Literal["bitbucket", "gitea", "github", "gitlab"]``
+
+The type of the remote VCS. Currently, Python Semantic Release supports ``"github"``,
+``"gitlab"``, ``"gitea"`` and ``"bitbucket"``. Not all functionality is available with all
+remote types, but we welcome pull requests to help improve this!
+
+**Default:** ``"github"``
+
+----
+
 .. _config-remote-token:
 
-``token (Dict['env': str])``
-""""""""""""""""""""""""""""
+``token``
+"""""""""
+
+**Type:** ``Optional[str | Dict['env', str]]``
 
 :ref:`Environment Variable <config-environment-variables>` from which to source the
 authentication token for the remote VCS. Common examples include ``"GH_TOKEN"``,
 ``"GITLAB_TOKEN"`` or ``"GITEA_TOKEN"``, however, you may choose to use a custom
 environment variable if you wish.
 
 .. note::
@@ -650,30 +855,35 @@
 ``"gitea"``       ->  ``{ env = "GITEA_TOKEN" }``
 ``"bitbucket"``   ->  ``{ env = "BITBUCKET_TOKEN" }``
 ================  ==  ===============================
 
 **Default:** ``{ env = "<envvar name>" }``, where ``<envvar name>`` depends on
 :ref:`remote.type <config-remote-type>` as indicated above.
 
+----
 
 .. _config-publish:
 
 ``[tool.semantic_release.publish]``
 ***********************************
 
+----
+
 .. _config-publish-dist-glob-patterns:
 
 ``dist_glob_patterns (List[str])``
 """"""""""""""""""""""""""""""""""
 
 Upload any files matching any of these globs to your VCS release. Each item in this
 list should be a string containing a Unix-style glob pattern.
 
 **Default:** ``["dist/*"]``
 
+----
+
 .. _config-publish-upload-to-vcs-release:
 
 ``upload_to_vcs_release (bool)``
 """"""""""""""""""""""""""""""""
 
 If set to ``true``, upload any artifacts matched by the
 :ref:`dist_glob_patterns <config-publish-dist-glob-patterns>` to the release created
```

### Comparing `python-semantic-release-9.4.1/docs/github-action.rst` & `python_semantic_release-9.4.2/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/index.rst` & `python_semantic_release-9.4.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/make.bat` & `python_semantic_release-9.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/migrating_from_v7.rst` & `python_semantic_release-9.4.2/docs/migrating_from_v7.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/multibranch_releases.rst` & `python_semantic_release-9.4.2/docs/multibranch_releases.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/strict_mode.rst` & `python_semantic_release-9.4.2/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/docs/troubleshooting.rst` & `python_semantic_release-9.4.2/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/pyproject.toml` & `python_semantic_release-9.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.4.1"
+version = "9.4.2"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -28,15 +28,15 @@
   "requests ~= 2.25",
   "jinja2 ~= 3.1",
   "python-gitlab ~= 4.0",
   "tomlkit ~= 0.11",
   "dotty-dict ~= 1.3",
   "importlib-resources ~= 6.0",
   "pydantic ~= 2.0",
-  "rich ~= 12.5",
+  "rich ~= 13.0",
   "shellingham ~= 1.5",
 ]
 
 [project.scripts]
 semantic-release = "semantic_release.cli:main"
 psr = "semantic_release.cli:main"
 
@@ -48,15 +48,15 @@
 repository = "http://github.com/python-semantic-release/python-semantic-release.git"
 
 [project.optional-dependencies]
 docs = [
   "Sphinx ~= 6.0",
   "sphinxcontrib-apidoc == 0.5.0",
   "sphinx-autobuild == 2024.2.4",
-  "furo ~= 2023.3",
+  "furo ~= 2024.1",
 ]
 test = [
   "coverage[toml] ~= 7.0",
   "pytest ~= 7.0",
   "pytest-env ~= 1.0",
   "pytest-xdist ~= 3.0",
   "pytest-mock ~= 3.0",
```

### Comparing `python-semantic-release-9.4.1/python_semantic_release.egg-info/PKG-INFO` & `python_semantic_release-9.4.2/python_semantic_release.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.4.1
+Version: 9.4.2
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -26,21 +26,21 @@
 Requires-Dist: requests~=2.25
 Requires-Dist: jinja2~=3.1
 Requires-Dist: python-gitlab~=4.0
 Requires-Dist: tomlkit~=0.11
 Requires-Dist: dotty-dict~=1.3
 Requires-Dist: importlib-resources~=6.0
 Requires-Dist: pydantic~=2.0
-Requires-Dist: rich~=12.5
+Requires-Dist: rich~=13.0
 Requires-Dist: shellingham~=1.5
 Provides-Extra: docs
 Requires-Dist: Sphinx~=6.0; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc==0.5.0; extra == "docs"
 Requires-Dist: sphinx-autobuild==2024.2.4; extra == "docs"
-Requires-Dist: furo~=2023.3; extra == "docs"
+Requires-Dist: furo~=2024.1; extra == "docs"
 Provides-Extra: test
 Requires-Dist: coverage[toml]~=7.0; extra == "test"
 Requires-Dist: pytest~=7.0; extra == "test"
 Requires-Dist: pytest-env~=1.0; extra == "test"
 Requires-Dist: pytest-xdist~=3.0; extra == "test"
 Requires-Dist: pytest-mock~=3.0; extra == "test"
 Requires-Dist: pytest-lazy-fixture~=0.6.3; extra == "test"
```

### Comparing `python-semantic-release-9.4.1/python_semantic_release.egg-info/SOURCES.txt` & `python_semantic_release-9.4.2/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/python_semantic_release.egg-info/requires.txt` & `python_semantic_release-9.4.2/python_semantic_release.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 requests~=2.25
 jinja2~=3.1
 python-gitlab~=4.0
 tomlkit~=0.11
 dotty-dict~=1.3
 importlib-resources~=6.0
 pydantic~=2.0
-rich~=12.5
+rich~=13.0
 shellingham~=1.5
 
 [dev]
 pre-commit~=3.5
 tox~=4.11
 ruff==0.3.5
 
 [docs]
 Sphinx~=6.0
 sphinxcontrib-apidoc==0.5.0
 sphinx-autobuild==2024.2.4
-furo~=2023.3
+furo~=2024.1
 
 [mypy]
 mypy==1.9.0
 types-requests~=2.31.0
 
 [test]
 coverage[toml]~=7.0
```

### Comparing `python-semantic-release-9.4.1/semantic_release/__init__.py` & `python_semantic_release-9.4.2/semantic_release/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.4.1"
+__version__ = "9.4.2"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-9.4.1/semantic_release/changelog/context.py` & `python_semantic_release-9.4.2/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/changelog/release_history.py` & `python_semantic_release-9.4.2/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/changelog/template.py` & `python_semantic_release-9.4.2/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/commands/changelog.py` & `python_semantic_release-9.4.2/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/commands/cli_context.py` & `python_semantic_release-9.4.2/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/commands/generate_config.py` & `python_semantic_release-9.4.2/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/commands/main.py` & `python_semantic_release-9.4.2/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/commands/publish.py` & `python_semantic_release-9.4.2/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/commands/version.py` & `python_semantic_release-9.4.2/semantic_release/cli/commands/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,26 +7,28 @@
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 import click
 import shellingham  # type: ignore[import]
 from click_option_group import MutuallyExclusiveOptionGroup, optgroup
 from git.exc import GitCommandError
+from requests import HTTPError
 
 from semantic_release.changelog import ReleaseHistory, environment, recursive_render
 from semantic_release.changelog.context import make_changelog_context
 from semantic_release.cli.common import (
     get_release_notes_template,
     render_default_changelog_file,
     render_release_notes,
 )
 from semantic_release.cli.github_actions_output import VersionGitHubActionsOutput
 from semantic_release.cli.util import indented, noop_report, rprint
 from semantic_release.const import DEFAULT_SHELL, DEFAULT_VERSION
 from semantic_release.enums import LevelBump
+from semantic_release.errors import UnexpectedResponse
 from semantic_release.version import Version, next_version, tags_and_versions
 
 log = logging.getLogger(__name__)
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing import ContextManager, Iterable
 
@@ -629,20 +631,38 @@
         else:
             try:
                 release_id = hvcs_client.create_or_update_release(
                     tag=new_version.as_tag(),
                     release_notes=release_notes,
                     prerelease=new_version.is_prerelease,
                 )
+            except HTTPError as err:
+                log.exception(err)
+                ctx.fail(str.join("\n", [str(err), "Failed to create release!"]))
+            except UnexpectedResponse as err:
+                log.exception(err)
+                ctx.fail(
+                    str.join(
+                        "\n",
+                        [
+                            str(err),
+                            "Unexpected response from remote VCS!",
+                            "Before re-running, make sure to clean up any artifacts on the hvcs that may have already been created.",
+                        ],
+                    )
+                )
             except Exception as e:
                 log.exception(e)
                 ctx.fail(str(e))
 
             for asset in assets:
                 log.info("Uploading asset %s", asset)
                 try:
                     hvcs_client.upload_asset(release_id, asset)
+                except HTTPError as err:
+                    log.exception(err)
+                    ctx.fail(str.join("\n", [str(err), "Failed to upload asset!"]))
                 except Exception as e:
                     log.exception(e)
                     ctx.fail(str(e))
 
     return str(new_version)
```

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/common.py` & `python_semantic_release-9.4.2/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/config.py` & `python_semantic_release-9.4.2/semantic_release/cli/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,26 @@
 from enum import Enum
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Literal, Optional, Tuple, Type, Union
 
 from git import Actor, InvalidGitRepositoryError
 from git.repo.base import Repo
 from jinja2 import Environment
-from pydantic import BaseModel, Field, RootModel, ValidationError, model_validator
+from pydantic import (
+    BaseModel,
+    Field,
+    RootModel,
+    ValidationError,
+    field_validator,
+    model_validator,
+)
 
-# For Python 3.8, 3.9, 3.10 compatibility
+# typing_extensions is for Python 3.8, 3.9, 3.10 compatibility
 from typing_extensions import Annotated, Self
+from urllib3.util.url import parse_url
 
 from semantic_release import hvcs
 from semantic_release.changelog import environment
 from semantic_release.cli.const import DEFAULT_CONFIG_FILE
 from semantic_release.cli.masking_filter import MaskingFilter
 from semantic_release.commit_parser import (
     AngularCommitParser,
@@ -107,30 +115,83 @@
     match: str = "(main|master)"
     prerelease_token: str = "rc"  # noqa: S105
     prerelease: bool = False
 
 
 class RemoteConfig(BaseModel):
     name: str = "origin"
-    token: MaybeFromEnv = ""
-    url: Optional[MaybeFromEnv] = None
+    token: Optional[str] = None
+    url: Optional[str] = None
     type: HvcsClient = HvcsClient.GITHUB
     domain: Optional[str] = None
     api_domain: Optional[str] = None
     ignore_token_for_push: bool = False
+    insecure: bool = False
+
+    @field_validator("url", "domain", "api_domain", "token", mode="before")
+    @classmethod
+    def resolve_env_vars(cls, val: Any) -> str | None:
+        ret_val = (
+            val
+            if not isinstance(val, dict)
+            else (EnvConfigVar.model_validate(val).getvalue())
+        )
+        return ret_val or None
 
     @model_validator(mode="after")
     def set_default_token(self) -> Self:
         # Set the default token name for the given VCS when no user input is given
         if not self.token and self.type in _known_hvcs:
             default_token_name = _known_hvcs[self.type].DEFAULT_ENV_TOKEN_NAME
             if default_token_name:
-                self.token = EnvConfigVar(env=default_token_name)
+                env_token = EnvConfigVar(env=default_token_name).getvalue()
+                if env_token:
+                    self.token = env_token
         return self
 
+    @model_validator(mode="after")
+    def check_url_scheme(self) -> Self:
+        if self.url and isinstance(self.url, str):
+            self.check_insecure_flag(self.url, "url")
+
+        if self.domain and isinstance(self.domain, str):
+            self.check_insecure_flag(self.domain, "domain")
+
+        if self.api_domain and isinstance(self.api_domain, str):
+            self.check_insecure_flag(self.api_domain, "api_domain")
+
+        return self
+
+    def check_insecure_flag(self, url_str: str, field_name: str) -> None:
+        if not url_str:
+            return
+
+        scheme = parse_url(url_str).scheme
+        if scheme == "http" and not self.insecure:
+            raise ValueError(
+                str.join(
+                    "\n",
+                    [
+                        "Insecure 'HTTP' URL detected and disabled by default.",
+                        "Set the 'insecure' flag to 'True' to enable insecure connections.",
+                    ],
+                )
+            )
+
+        if scheme == "https" and self.insecure:
+            log.warning(
+                str.join(
+                    "\n",
+                    [
+                        f"'{field_name}' starts with 'https://' but the 'insecure' flag is set.",
+                        "This flag is only necessary for 'http://' URLs.",
+                    ],
+                )
+            )
+
 
 class PublishConfig(BaseModel):
     dist_glob_patterns: Tuple[str, ...] = ("dist/*",)
     upload_to_vcs_release: bool = True
 
 
 class RawConfig(BaseModel):
@@ -366,43 +427,32 @@
                 log.exception("Invalid variable declaration %r", decl)
                 raise InvalidConfiguration(
                     f"Invalid variable declaration {decl!r}"
                 ) from exc
 
             version_declarations.append(pd)
 
-        # hvcs_client
-        hvcs_client_cls = _known_hvcs[raw.remote.type]
-        raw_remote_url = raw.remote.url
-        resolved_remote_url = cls.resolve_from_env(raw_remote_url)
-        remote_url = (
-            resolved_remote_url
-            if resolved_remote_url is not None
-            else repo.remote(raw.remote.name).url
-        )
-
-        token = cls.resolve_from_env(raw.remote.token)
-        if (
-            isinstance(raw.remote.token, EnvConfigVar)
-            and not raw.remote.ignore_token_for_push
-            and not token
-        ):
-            log.warning(
-                "the token for the remote VCS is configured as stored in the %s "
-                "environment variable, but it is empty",
-                raw.remote.token.env,
-            )
-        elif not token:
+        # Provide warnings if the token is missing
+        if not raw.remote.token:
             log.debug("hvcs token is not set")
 
+            if not raw.remote.ignore_token_for_push:
+                log.warning("Token value is missing!")
+
+        # retrieve remote url
+        remote_url = raw.remote.url or repo.remote(raw.remote.name).url
+
+        # hvcs_client
+        hvcs_client_cls = _known_hvcs[raw.remote.type]
         hvcs_client = hvcs_client_cls(
             remote_url=remote_url,
-            hvcs_domain=cls.resolve_from_env(raw.remote.domain),
-            hvcs_api_domain=cls.resolve_from_env(raw.remote.api_domain),
-            token=token,
+            hvcs_domain=raw.remote.domain,
+            hvcs_api_domain=raw.remote.api_domain,
+            token=raw.remote.token,
+            allow_insecure=raw.remote.insecure,
         )
 
         # changelog_file
         changelog_file = Path(raw.changelog.changelog_file).resolve()
 
         template_dir = Path(repo.working_tree_dir or ".") / raw.changelog.template_dir
```

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/github_actions_output.py` & `python_semantic_release-9.4.2/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/masking_filter.py` & `python_semantic_release-9.4.2/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/cli/util.py` & `python_semantic_release-9.4.2/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/__init__.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/_base.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/angular.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/emoji.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/scipy.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/tag.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/token.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/commit_parser/util.py` & `python_semantic_release-9.4.2/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/const.py` & `python_semantic_release-9.4.2/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/data/templates/CHANGELOG.md.j2` & `python_semantic_release-9.4.2/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/enums.py` & `python_semantic_release-9.4.2/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/errors.py` & `python_semantic_release-9.4.2/semantic_release/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,7 +34,14 @@
 
 
 class MissingMergeBaseError(SemanticReleaseBaseError):
     """
     Raised when the merge base cannot be found with the current history. Generally
     because of a shallow git clone.
     """
+
+
+class UnexpectedResponse(Exception):
+    """
+    Raised when an HTTP response cannot be parsed properly or the expected structure
+    is not found.
+    """
```

### Comparing `python-semantic-release-9.4.1/semantic_release/helpers.py` & `python_semantic_release-9.4.2/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/hvcs/_base.py` & `python_semantic_release-9.4.2/semantic_release/hvcs/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Common functionality and interface for interacting with Git remote VCS"""
 
 from __future__ import annotations
 
 import logging
 import warnings
 from functools import lru_cache
+from typing import TYPE_CHECKING
 
 from semantic_release.helpers import parse_git_url
-from semantic_release.hvcs.token_auth import TokenAuth
-from semantic_release.hvcs.util import build_requests_session
 
+if TYPE_CHECKING:
+    from typing import Any
+
+
+# Globals
 logger = logging.getLogger(__name__)
 
 
 # This would be nice as a decorator but it obscured the method's call signature
 # which makes mypy unhappy
 def _not_supported(self: HvcsBase, method_name: str) -> None:
     warnings.warn(
@@ -28,31 +32,21 @@
 
     Methods which have a base implementation are implemented here
 
     Methods which aren't mandatory but should indicate a lack of support gracefully
     (i.e. without raising an exception) return _not_supported, and can be overridden
     to provide an implementation in subclasses. This is more straightforward than
     checking for NotImplemented around every method call.
+
     """
 
     DEFAULT_ENV_TOKEN_NAME = "HVCS_TOKEN"  # noqa: S105
 
-    def __init__(
-        self,
-        remote_url: str,
-        hvcs_domain: str | None = None,
-        hvcs_api_domain: str | None = None,
-        token: str | None = None,
-    ) -> None:
-        self.hvcs_domain = hvcs_domain
-        self.hvcs_api_domain = hvcs_api_domain
-        self.token = token
-        auth = None if not self.token else TokenAuth(self.token)
+    def __init__(self, remote_url: str, *args: Any, **kwargs: Any) -> None:
         self._remote_url = remote_url
-        self.session = build_requests_session(auth=auth)
 
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         """
         Parse the repository's remote url to identify the repository
         owner and name
         """
@@ -68,18 +62,21 @@
     def owner(self) -> str:
         _owner, _ = self._get_repository_owner_and_name()
         return _owner
 
     def compare_url(self, from_rev: str, to_rev: str) -> str:
         """
         Get the comparison link between two version tags.
+
         :param from_rev: The older version to compare. Can be a commit sha, tag or
-                        branch name.
+        branch name.
+
         :param to_rev: The newer version to compare. Can be a commit sha, tag or
-                       branch name.
+        branch name.
+
         :return: Link to view a comparison between the two versions.
         """
         _not_supported(self, "compare_url")
         return ""
 
     def upload_dists(self, tag: str, dist_glob: str) -> int:
         """
```

### Comparing `python-semantic-release-9.4.1/semantic_release/hvcs/gitea.py` & `python_semantic_release-9.4.2/semantic_release/hvcs/gitea.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,186 @@
 """Helper code for interacting with a Gitea remote VCS"""
 
 from __future__ import annotations
 
 import glob
 import logging
-import mimetypes
 import os
+from pathlib import PurePosixPath
+from typing import TYPE_CHECKING
 
-from requests import HTTPError
+from requests import HTTPError, JSONDecodeError
 from urllib3.util.url import Url, parse_url
 
+from semantic_release.errors import UnexpectedResponse
 from semantic_release.helpers import logged_function
 from semantic_release.hvcs._base import HvcsBase
 from semantic_release.hvcs.token_auth import TokenAuth
 from semantic_release.hvcs.util import build_requests_session, suppress_not_found
 
-log = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from typing import Any
+
 
-# Add a mime type for wheels
-# Fix incorrect entries in the `mimetypes` registry.
-# On Windows, the Python standard library's `mimetypes` reads in
-# mappings from file extension to MIME type from the Windows
-# registry. Other applications can and do write incorrect values
-# to this registry, which causes `mimetypes.guess_type` to return
-# incorrect values, which causes TensorBoard to fail to render on
-# the frontend.
-# This method hard-codes the correct mappings for certain MIME
-# types that are known to be either used by python-semantic-release or
-# problematic in general.
-mimetypes.add_type("application/octet-stream", ".whl")
-mimetypes.add_type("text/markdown", ".md")
+# Globals
+log = logging.getLogger(__name__)
 
 
 class Gitea(HvcsBase):
     """Gitea helper class"""
 
     DEFAULT_DOMAIN = "gitea.com"
     DEFAULT_API_PATH = "/api/v1"
-    DEFAULT_API_DOMAIN = f"{DEFAULT_DOMAIN}{DEFAULT_API_PATH}"
     DEFAULT_ENV_TOKEN_NAME = "GITEA_TOKEN"  # noqa: S105
 
-    # pylint: disable=super-init-not-called
     def __init__(
         self,
         remote_url: str,
+        *,
         hvcs_domain: str | None = None,
-        hvcs_api_domain: str | None = None,
         token: str | None = None,
+        allow_insecure: bool = False,
+        **kwargs: Any,
     ) -> None:
-        self._remote_url = remote_url
+        super().__init__(remote_url)
+        self.token = token
+        auth = None if not self.token else TokenAuth(self.token)
+        self.session = build_requests_session(auth=auth)
 
         domain_url = parse_url(
-            hvcs_domain or os.getenv("GITEA_SERVER_URL", "") or self.DEFAULT_DOMAIN
+            hvcs_domain
+            or os.getenv("GITEA_SERVER_URL", "")
+            or f"https://{self.DEFAULT_DOMAIN}"
         )
 
-        # Strip any scheme, query or fragment from the domain
-        self.hvcs_domain = Url(
-            host=domain_url.host, port=domain_url.port, path=domain_url.path
-        ).url.rstrip("/")
+        if domain_url.scheme == "http" and not allow_insecure:
+            raise ValueError("Insecure connections are currently disabled.")
+
+        if not domain_url.scheme:
+            new_scheme = "http" if allow_insecure else "https"
+            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
+
+        if domain_url.scheme not in ["http", "https"]:
+            raise ValueError(
+                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
+                "Only http and https are supported."
+            )
+
+        # Strip any auth, query or fragment from the domain
+        self.hvcs_domain = parse_url(
+            Url(
+                scheme=domain_url.scheme,
+                host=domain_url.host,
+                port=domain_url.port,
+                path=str(PurePosixPath(domain_url.path or "/")),
+            ).url.rstrip("/")
+        )
 
-        api_domain_parts = parse_url(
-            hvcs_api_domain
-            or os.getenv("GITEA_API_URL", "")
+        self.api_url = parse_url(
+            os.getenv("GITEA_API_URL", "").rstrip("/")
             or Url(
                 # infer from Domain url and append the default api path
-                scheme=domain_url.scheme,
-                host=self.hvcs_domain,
-                path=self.DEFAULT_API_PATH,
+                **{
+                    **self.hvcs_domain._asdict(),
+                    "path": f"{self.hvcs_domain.path or ''}{self.DEFAULT_API_PATH}",
+                }
             ).url
         )
 
-        # Strip any scheme, query or fragment from the api domain
-        self.hvcs_api_domain = Url(
-            host=api_domain_parts.host,
-            port=api_domain_parts.port,
-            path=api_domain_parts.path,
-        ).url.rstrip("/")
-
-        self.api_url = f"https://{self.hvcs_api_domain}"
-
-        self.token = token
-        auth = None if not self.token else TokenAuth(self.token)
-        self.session = build_requests_session(auth=auth)
-
     @logged_function(log)
     def create_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """
         Create a new release
-        https://gitea.com/api/swagger#/repository/repoCreateRelease
+
+        Ref: https://gitea.com/api/swagger#/repository/repoCreateRelease
+
         :param tag: Tag to create release for
+
         :param release_notes: The release notes for this version
+
         :param prerelease: Whether or not this release should be specified as a
-                           prerelease
+        prerelease
+
         :return: Whether the request succeeded
         """
         log.info("Creating release for tag %s", tag)
-        resp = self.session.post(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases",
+        releases_endpoint = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases",
+        )
+        response = self.session.post(
+            releases_endpoint,
             json={
                 "tag_name": tag,
                 "name": tag,
                 "body": release_notes,
                 "draft": False,
                 "prerelease": prerelease,
             },
         )
-        return resp.json()["id"]
+
+        # Raise an error if the request was not successful
+        response.raise_for_status()
+
+        try:
+            data = response.json()
+            return data["id"]
+        except JSONDecodeError as err:
+            raise UnexpectedResponse("Unreadable json response") from err
+        except KeyError as err:
+            raise UnexpectedResponse("JSON response is missing an id") from err
 
     @logged_function(log)
     @suppress_not_found
     def get_release_id_by_tag(self, tag: str) -> int | None:
         """
         Get a release by its tag name
         https://gitea.com/api/swagger#/repository/repoGetReleaseByTag
         :param tag: Tag to get release for
         :return: ID of found release
         """
-        response = self.session.get(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/tags/{tag}"
+        tag_endpoint = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/tags/{tag}",
         )
-        return response.json().get("id")
+        response = self.session.get(tag_endpoint)
+
+        # Raise an error if the request was not successful
+        response.raise_for_status()
+
+        try:
+            data = response.json()
+            return data["id"]
+        except JSONDecodeError as err:
+            raise UnexpectedResponse("Unreadable json response") from err
+        except KeyError as err:
+            raise UnexpectedResponse("JSON response is missing an id") from err
 
     @logged_function(log)
     def edit_release_notes(self, release_id: int, release_notes: str) -> int:
         """
         Edit a release with updated change notes
         https://gitea.com/api/swagger#/repository/repoEditRelease
         :param id: ID of release to update
         :param release_notes: The release notes for this version
         :return: The ID of the release that was edited
         """
         log.info("Updating release %s", release_id)
-        self.session.patch(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/{release_id}",
+        release_endpoint = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/{release_id}",
+        )
+
+        response = self.session.patch(
+            release_endpoint,
             json={"body": release_notes},
         )
+
+        # Raise an error if the request was not successful
+        response.raise_for_status()
+
         return release_id
 
     @logged_function(log)
     def create_or_update_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """
@@ -157,26 +197,29 @@
             log.debug("looking for an existing release to update")
 
         release_id = self.get_release_id_by_tag(tag)
         if release_id is None:
             raise ValueError(
                 f"release id for tag {tag} not found, and could not be created"
             )
-        log.debug("Found existing release %s, updating", release_id)
+
         # If this errors we let it die
+        log.debug("Found existing release %s, updating", release_id)
         return self.edit_release_notes(release_id, release_notes)
 
     @logged_function(log)
     def asset_upload_url(self, release_id: str) -> str:
         """
         Get the correct upload url for a release
         https://gitea.com/api/swagger#/repository/repoCreateReleaseAttachment
         :param release_id: ID of the release to upload to
         """
-        return f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/{release_id}/assets"  # noqa: E501
+        return self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/{release_id}/assets",
+        )
 
     @logged_function(log)
     def upload_asset(
         self,
         release_id: int,
         file: str,
         label: str | None = None,  # noqa: ARG002
@@ -203,14 +246,17 @@
                         name,
                         attachment,
                         content_type,
                     ),
                 },
             )
 
+            # Raise an error if the request was not successful
+            response.raise_for_status()
+
         log.info(
             "Successfully uploaded %s to Gitea, url: %s, status code: %s",
             file,
             response.url,
             response.status_code,
         )
 
@@ -240,18 +286,65 @@
                 n_succeeded += 1
             except HTTPError:  # noqa: PERF203
                 log.exception("error uploading asset %s", file_path)
 
         return n_succeeded
 
     def remote_url(self, use_token: bool = True) -> str:
+        """Get the remote url including the token for authentication if requested"""
         if not (self.token and use_token):
             return self._remote_url
-        return (
-            f"https://{self.token}@{self.hvcs_domain}/{self.owner}/{self.repo_name}.git"
+
+        return self.create_server_url(
+            auth=self.token,
+            path=f"{self.owner}/{self.repo_name}.git",
         )
 
     def commit_hash_url(self, commit_hash: str) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/commit/{commit_hash}"
+        return self.create_server_url(
+            path=f"/{self.owner}/{self.repo_name}/commit/{commit_hash}"
+        )
 
     def pull_request_url(self, pr_number: str | int) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/pulls/{pr_number}"
+        return self.create_server_url(
+            path=f"/{self.owner}/{self.repo_name}/pulls/{pr_number}"
+        )
+
+    def create_server_url(
+        self,
+        path: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        overrides = dict(
+            filter(
+                lambda x: x[1] is not None,
+                {
+                    "auth": auth,
+                    "path": str(PurePosixPath(path or "/")),
+                    "query": query,
+                    "fragment": fragment,
+                }.items(),
+            )
+        )
+        return Url(
+            **{
+                **self.hvcs_domain._asdict(),
+                **overrides,
+            }
+        ).url.rstrip("/")
+
+    def create_api_url(
+        self,
+        endpoint: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        api_path = self.api_url.url.replace(self.hvcs_domain.url, "")
+        return self.create_server_url(
+            path=f"{api_path}/{endpoint.lstrip(api_path)}",
+            auth=auth,
+            query=query,
+            fragment=fragment,
+        )
```

### Comparing `python-semantic-release-9.4.1/semantic_release/hvcs/github.py` & `python_semantic_release-9.4.2/semantic_release/hvcs/github.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,98 +3,174 @@
 from __future__ import annotations
 
 import glob
 import logging
 import mimetypes
 import os
 from functools import lru_cache
+from pathlib import PurePosixPath
+from typing import TYPE_CHECKING
 
-from requests import HTTPError
+from requests import HTTPError, JSONDecodeError
+from urllib3.util.url import Url, parse_url
 
+from semantic_release.errors import UnexpectedResponse
 from semantic_release.helpers import logged_function
 from semantic_release.hvcs._base import HvcsBase
 from semantic_release.hvcs.token_auth import TokenAuth
 from semantic_release.hvcs.util import build_requests_session, suppress_not_found
 
+if TYPE_CHECKING:
+    from typing import Any
+
+
+# Globals
 log = logging.getLogger(__name__)
 
+
 # Add a mime type for wheels
 # Fix incorrect entries in the `mimetypes` registry.
 # On Windows, the Python standard library's `mimetypes` reads in
 # mappings from file extension to MIME type from the Windows
 # registry. Other applications can and do write incorrect values
 # to this registry, which causes `mimetypes.guess_type` to return
 # incorrect values, which causes TensorBoard to fail to render on
 # the frontend.
 # This method hard-codes the correct mappings for certain MIME
 # types that are known to be either used by python-semantic-release or
 # problematic in general.
-mimetypes.add_type("application/octet-stream", ".whl")
-mimetypes.add_type("text/markdown", ".md")
+if mimetypes.guess_type("test.whl")[0] != "application/octet-stream":
+    mimetypes.add_type("application/octet-stream", ".whl")
+
+if mimetypes.guess_type("test.md")[0] != "text/markdown":
+    mimetypes.add_type("text/markdown", ".md")
 
 
 class Github(HvcsBase):
-    """Github helper class"""
+    """
+    GitHub HVCS interface for interacting with GitHub repositories
 
+    This class supports the following products:
+        - GitHub Free, Pro, & Team
+        - GitHub Enterprise Cloud
+
+    This class does not support the following products:
+        - GitHub Enterprise Server (on-premises installations)
+    """
+
+    # TODO: Add support for GitHub Enterprise Server (on-premises installations)
+    #       DEFAULT_ONPREM_API_PATH = "/api/v3"
     DEFAULT_DOMAIN = "github.com"
-    DEFAULT_API_DOMAIN = "api.github.com"
-    DEFAULT_UPLOAD_DOMAIN = "uploads.github.com"
+    DEFAULT_API_SUBDOMAIN_PREFIX = "api"
+    DEFAULT_API_DOMAIN = f"{DEFAULT_API_SUBDOMAIN_PREFIX}.{DEFAULT_DOMAIN}"
     DEFAULT_ENV_TOKEN_NAME = "GH_TOKEN"  # noqa: S105
 
     def __init__(
         self,
         remote_url: str,
+        *,
         hvcs_domain: str | None = None,
         hvcs_api_domain: str | None = None,
         token: str | None = None,
+        allow_insecure: bool = False,
+        **kwargs: Any,
     ) -> None:
-        self._remote_url = remote_url
+        super().__init__(remote_url)
+        self.token = token
+        auth = None if not self.token else TokenAuth(self.token)
+        self.session = build_requests_session(auth=auth)
 
         # ref: https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables
-        self.hvcs_domain = hvcs_domain or os.getenv(
-            "GITHUB_SERVER_URL", self.DEFAULT_DOMAIN
-        ).replace("https://", "")
+        domain_url = parse_url(
+            hvcs_domain
+            or os.getenv("GITHUB_SERVER_URL", "")
+            or f"https://{self.DEFAULT_DOMAIN}"
+        )
+
+        if domain_url.scheme == "http" and not allow_insecure:
+            raise ValueError("Insecure connections are currently disabled.")
+
+        if not domain_url.scheme:
+            new_scheme = "http" if allow_insecure else "https"
+            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
+
+        if domain_url.scheme not in ["http", "https"]:
+            raise ValueError(
+                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
+                "Only http and https are supported."
+            )
+
+        # Strip any auth, query or fragment from the domain
+        self.hvcs_domain = parse_url(
+            Url(
+                scheme=domain_url.scheme,
+                host=domain_url.host,
+                port=domain_url.port,
+                path=str(PurePosixPath(domain_url.path or "/")),
+            ).url.rstrip("/")
+        )
 
-        # not necessarily prefixed with "api." in the case of a custom domain, so
-        # can't just default to "api.github.com"
         # ref: https://docs.github.com/en/actions/reference/environment-variables#default-environment-variables
-        self.hvcs_api_domain = hvcs_api_domain or os.getenv(
-            "GITHUB_API_URL", self.DEFAULT_API_DOMAIN
-        ).replace("https://", "")
+        api_domain_parts = parse_url(
+            hvcs_api_domain
+            or os.getenv("GITHUB_API_URL", "")
+            or Url(
+                # infer from Domain url and prepend the default api subdomain
+                **{
+                    **self.hvcs_domain._asdict(),
+                    "host": f"{self.DEFAULT_API_SUBDOMAIN_PREFIX}.{self.hvcs_domain.host}",
+                    "path": "",
+                }
+            ).url
+        )
 
-        self.api_url = f"https://{self.hvcs_api_domain}"
-        self.upload_url = f"https://{self.DEFAULT_UPLOAD_DOMAIN}"
+        if api_domain_parts.scheme == "http" and not allow_insecure:
+            raise ValueError("Insecure connections are currently disabled.")
 
-        self.token = token
-        auth = None if not self.token else TokenAuth(self.token)
-        self.session = build_requests_session(auth=auth)
+        if not api_domain_parts.scheme:
+            new_scheme = "http" if allow_insecure else "https"
+            api_domain_parts = Url(
+                **{**api_domain_parts._asdict(), "scheme": new_scheme}
+            )
+
+        if api_domain_parts.scheme not in ["http", "https"]:
+            raise ValueError(
+                f"Invalid scheme {api_domain_parts.scheme} for api domain {api_domain_parts.host}. "
+                "Only http and https are supported."
+            )
+
+        # Strip any auth, query or fragment from the domain
+        self.api_url = parse_url(
+            Url(
+                scheme=api_domain_parts.scheme,
+                host=api_domain_parts.host,
+                port=api_domain_parts.port,
+                path=str(PurePosixPath(api_domain_parts.path or "/")),
+            ).url.rstrip("/")
+        )
 
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         # Github actions context
         if "GITHUB_REPOSITORY" in os.environ:
             log.debug("getting repository owner and name from environment variables")
             owner, name = os.environ["GITHUB_REPOSITORY"].rsplit("/", 1)
             return owner, name
+
         return super()._get_repository_owner_and_name()
 
-    def compare_url(
-        self,
-        from_rev: str,
-        to_rev: str,
-    ) -> str:
+    def compare_url(self, from_rev: str, to_rev: str) -> str:
         """
         Get the GitHub comparison link between two version tags.
         :param from_rev: The older version to compare.
         :param to_rev: The newer version to compare.
         :return: Link to view a comparison between the two versions.
         """
-        return (
-            f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/compare/"
-            f"{from_rev}...{to_rev}"
+        return self.create_server_url(
+            path=f"/{self.owner}/{self.repo_name}/compare/{from_rev}...{to_rev}"
         )
 
     @logged_function(log)
     def create_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """
@@ -102,61 +178,87 @@
         https://docs.github.com/rest/reference/repos#create-a-release
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
         :param prerelease: Whether or not this release should be created as a prerelease
         :return: the ID of the release
         """
         log.info("Creating release for tag %s", tag)
-        resp = self.session.post(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases",
+        releases_endpoint = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases",
+        )
+        response = self.session.post(
+            releases_endpoint,
             json={
                 "tag_name": tag,
                 "name": tag,
                 "body": release_notes,
                 "draft": False,
                 "prerelease": prerelease,
             },
         )
 
-        release_id: int = resp.json()["id"]
-        log.info("Successfully created release with ID: %s", release_id)
-        return release_id
+        # Raise an error if the request was not successful
+        response.raise_for_status()
+
+        try:
+            release_id: int = response.json()["id"]
+            log.info("Successfully created release with ID: %s", release_id)
+            return release_id
+        except JSONDecodeError as err:
+            raise UnexpectedResponse("Unreadable json response") from err
+        except KeyError as err:
+            raise UnexpectedResponse("JSON response is missing an id") from err
 
     @logged_function(log)
     @suppress_not_found
     def get_release_id_by_tag(self, tag: str) -> int | None:
         """
         Get a release by its tag name
         https://docs.github.com/rest/reference/repos#get-a-release-by-tag-name
         :param tag: Tag to get release for
         :return: ID of release, if found, else None
         """
-        response = self.session.get(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/tags/{tag}"
+        tag_endpoint = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/tags/{tag}",
         )
-        return response.json().get("id")
+        response = self.session.get(tag_endpoint)
+
+        # Raise an error if the request was not successful
+        response.raise_for_status()
+
+        try:
+            data = response.json()
+            return data["id"]
+        except JSONDecodeError as err:
+            raise UnexpectedResponse("Unreadable json response") from err
+        except KeyError as err:
+            raise UnexpectedResponse("JSON response is missing an id") from err
 
     @logged_function(log)
-    def edit_release_notes(
-        self,
-        release_id: int,
-        release_notes: str,
-    ) -> int:
+    def edit_release_notes(self, release_id: int, release_notes: str) -> int:
         """
         Edit a release with updated change notes
         https://docs.github.com/rest/reference/repos#update-a-release
         :param id: ID of release to update
         :param release_notes: The release notes for this version
         :return: The ID of the release that was edited
         """
         log.info("Updating release %s", release_id)
-        self.session.post(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/{release_id}",
+        release_endpoint = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/{release_id}",
+        )
+
+        response = self.session.post(
+            release_endpoint,
             json={"body": release_notes},
         )
+
+        # Raise an error if the update was unsuccessful
+        response.raise_for_status()
+
         return release_id
 
     @logged_function(log)
     def create_or_update_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """
@@ -188,18 +290,30 @@
         """
         Get the correct upload url for a release
         https://docs.github.com/en/enterprise-server@3.5/rest/releases/releases#get-a-release
         :param release_id: ID of the release to upload to
         :return: URL to upload for a release if found, else None
         """
         # https://docs.github.com/en/enterprise-server@3.5/rest/releases/assets#upload-a-release-asset
-        response = self.session.get(
-            f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/{release_id}",
+        release_url = self.create_api_url(
+            endpoint=f"/repos/{self.owner}/{self.repo_name}/releases/{release_id}"
         )
-        return response.json().get("upload_url").replace("{?name,label}", "")
+
+        response = self.session.get(release_url)
+        response.raise_for_status()
+
+        try:
+            upload_url: str = response.json()["upload_url"]
+            return upload_url.replace("{?name,label}", "")
+        except JSONDecodeError as err:
+            raise UnexpectedResponse("Unreadable json response") from err
+        except KeyError as err:
+            raise UnexpectedResponse(
+                "JSON response is missing a key 'upload_url'"
+            ) from err
 
     @logged_function(log)
     def upload_asset(
         self, release_id: int, file: str, label: str | None = None
     ) -> bool:
         """
         Upload an asset to an existing release
@@ -212,28 +326,32 @@
         url = self.asset_upload_url(release_id)
         if url is None:
             raise ValueError(
                 "There is no associated url for uploading asset for release "
                 f"{release_id}. Release url: "
                 f"{self.api_url}/repos/{self.owner}/{self.repo_name}/releases/{release_id}"
             )
+
         content_type = (
             mimetypes.guess_type(file, strict=False)[0] or "application/octet-stream"
         )
 
         with open(file, "rb") as data:
             response = self.session.post(
                 url,
                 params={"name": os.path.basename(file), "label": label},
                 headers={
                     "Content-Type": content_type,
                 },
                 data=data.read(),
             )
 
+            # Raise an error if the upload was unsuccessful
+            response.raise_for_status()
+
         log.debug(
             "Successfully uploaded %s to Github, url: %s, status code: %s",
             file,
             response.url,
             response.status_code,
         )
 
@@ -263,22 +381,71 @@
                 n_succeeded += 1
             except HTTPError:  # noqa: PERF203
                 log.exception("error uploading asset %s", file_path)
 
         return n_succeeded
 
     def remote_url(self, use_token: bool = True) -> str:
+        """Get the remote url including the token for authentication if requested"""
         if not (self.token and use_token):
             log.info("requested to use token for push but no token set, ignoring...")
             return self._remote_url
-        actor = os.getenv("GITHUB_ACTOR")
-        return (
-            f"https://{actor}:{self.token}@{self.hvcs_domain}/{self.owner}/{self.repo_name}.git"
-            if actor
-            else f"https://{self.token}@{self.hvcs_domain}/{self.owner}/{self.repo_name}.git"
+
+        actor = os.getenv("GITHUB_ACTOR", None)
+        return self.create_server_url(
+            auth=f"{actor}:{self.token}" if actor else self.token,
+            path=f"/{self.owner}/{self.repo_name}.git",
         )
 
     def commit_hash_url(self, commit_hash: str) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/commit/{commit_hash}"
+        return self.create_server_url(
+            path=f"/{self.owner}/{self.repo_name}/commit/{commit_hash}"
+        )
 
     def pull_request_url(self, pr_number: str | int) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/issues/{pr_number}"
+        return self.create_server_url(
+            path=f"/{self.owner}/{self.repo_name}/issues/{pr_number}"
+        )
+
+    def _derive_url(
+        self,
+        base_url: Url,
+        path: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        overrides = dict(
+            filter(
+                lambda x: x[1] is not None,
+                {
+                    "auth": auth,
+                    "path": str(PurePosixPath("/", path)),
+                    "query": query,
+                    "fragment": fragment,
+                }.items(),
+            )
+        )
+        return Url(
+            **{
+                **base_url._asdict(),
+                **overrides,
+            }
+        ).url.rstrip("/")
+
+    def create_server_url(
+        self,
+        path: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        return self._derive_url(self.hvcs_domain, path, auth, query, fragment)
+
+    def create_api_url(
+        self,
+        endpoint: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        return self._derive_url(self.api_url, endpoint, auth, query, fragment)
```

### Comparing `python-semantic-release-9.4.1/semantic_release/hvcs/gitlab.py` & `python_semantic_release-9.4.2/semantic_release/hvcs/gitlab.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 """Helper code for interacting with a Gitlab remote VCS"""
 
 from __future__ import annotations
 
 import logging
-import mimetypes
 import os
 from functools import lru_cache
-from urllib.parse import urlsplit
+from pathlib import PurePosixPath
+from typing import TYPE_CHECKING
 
 import gitlab
+from urllib3.util.url import Url, parse_url
 
 from semantic_release.helpers import logged_function
 from semantic_release.hvcs._base import HvcsBase
-from semantic_release.hvcs.token_auth import TokenAuth
-from semantic_release.hvcs.util import build_requests_session
 
-log = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from typing import Any
+
 
-# Add a mime type for wheels
-# Fix incorrect entries in the `mimetypes` registry.
-# On Windows, the Python standard library's `mimetypes` reads in
-# mappings from file extension to MIME type from the Windows
-# registry. Other applications can and do write incorrect values
-# to this registry, which causes `mimetypes.guess_type` to return
-# incorrect values, which causes TensorBoard to fail to render on
-# the frontend.
-# This method hard-codes the correct mappings for certain MIME
-# types that are known to be either used by python-semantic-release or
-# problematic in general.
-mimetypes.add_type("application/octet-stream", ".whl")
-mimetypes.add_type("text/markdown", ".md")
+# Globals
+log = logging.getLogger(__name__)
 
 
 class Gitlab(HvcsBase):
     """
     Gitlab helper class
     Note Gitlab doesn't really have the concept of a separate
     API domain
@@ -44,48 +34,65 @@
     # It is missing the permission to push to the repository, but has all others (releases, packages, etc.)
 
     DEFAULT_DOMAIN = "gitlab.com"
 
     def __init__(
         self,
         remote_url: str,
+        *,
         hvcs_domain: str | None = None,
-        hvcs_api_domain: str | None = None,
         token: str | None = None,
+        allow_insecure: bool = False,
+        **kwargs: Any,
     ) -> None:
+        super().__init__(remote_url)
         self._remote_url = remote_url
-        self.hvcs_domain = (
-            hvcs_domain or self._domain_from_environment() or self.DEFAULT_DOMAIN
-        )
-        self.hvcs_api_domain = hvcs_api_domain or self.hvcs_domain.replace(
-            "https://", ""
+        self.token = token
+
+        domain_url = parse_url(
+            hvcs_domain
+            or os.getenv("CI_SERVER_URL", "")
+            or f"https://{self.DEFAULT_DOMAIN}"
         )
-        self.api_url = os.getenv("CI_SERVER_URL", f"https://{self.hvcs_api_domain}")
 
-        self.token = token
-        auth = None if not self.token else TokenAuth(self.token)
-        self.session = build_requests_session(auth=auth)
+        if domain_url.scheme == "http" and not allow_insecure:
+            raise ValueError("Insecure connections are currently disabled.")
 
-    @staticmethod
-    def _domain_from_environment() -> str | None:
-        """Use Gitlab-CI environment variable to get the server domain, if available"""
-        if "CI_SERVER_URL" in os.environ:
-            url = urlsplit(os.environ["CI_SERVER_URL"])
-            return f"{url.netloc}{url.path}".rstrip("/")
-        return os.getenv("CI_SERVER_HOST")
+        if not domain_url.scheme:
+            new_scheme = "http" if allow_insecure else "https"
+            domain_url = Url(**{**domain_url._asdict(), "scheme": new_scheme})
+
+        if domain_url.scheme not in ["http", "https"]:
+            raise ValueError(
+                f"Invalid scheme {domain_url.scheme} for domain {domain_url.host}. "
+                "Only http and https are supported."
+            )
+
+        # Strip any auth, query or fragment from the domain
+        self.hvcs_domain = parse_url(
+            Url(
+                scheme=domain_url.scheme,
+                host=domain_url.host,
+                port=domain_url.port,
+                path=str(PurePosixPath(domain_url.path or "/")),
+            ).url.rstrip("/")
+        )
+
+        self._client = gitlab.Gitlab(self.hvcs_domain.url)
 
     @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         """
         Get the repository owner and name from GitLab CI environment variables, if
         available, otherwise from parsing the remote url
         """
         if "CI_PROJECT_NAMESPACE" in os.environ and "CI_PROJECT_NAME" in os.environ:
             log.debug("getting repository owner and name from environment variables")
             return os.environ["CI_PROJECT_NAMESPACE"], os.environ["CI_PROJECT_NAME"]
+
         return super()._get_repository_owner_and_name()
 
     @logged_function(log)
     def create_release(
         self,
         tag: str,
         release_notes: str,
@@ -94,15 +101,15 @@
         """
         Post release changelog
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
         :param prerelease: This parameter has no effect
         :return: The tag of the release
         """
-        client = gitlab.Gitlab(self.api_url, private_token=self.token)
+        client = gitlab.Gitlab(self.hvcs_domain.url, private_token=self.token)
         client.auth()
         log.info("Creating release for %s", tag)
         # ref: https://docs.gitlab.com/ee/api/releases/index.html#create-a-release
         client.projects.get(self.owner + "/" + self.repo_name).releases.create(
             {
                 "name": "Release " + tag,
                 "tag_name": tag,
@@ -115,15 +122,15 @@
     # TODO: make str types accepted here
     @logged_function(log)
     def edit_release_notes(  # type: ignore[override]
         self,
         release_id: str,
         release_notes: str,
     ) -> str:
-        client = gitlab.Gitlab(self.api_url, private_token=self.token)
+        client = gitlab.Gitlab(self.hvcs_domain.url, private_token=self.token)
         client.auth()
         log.info("Updating release %s", release_id)
 
         client.projects.get(self.owner + "/" + self.repo_name).releases.update(
             release_id,
             {
                 "description": release_notes,
@@ -145,20 +152,78 @@
                 tag,
                 self.owner,
                 self.repo_name,
             )
             return self.edit_release_notes(release_id=tag, release_notes=release_notes)
 
     def compare_url(self, from_rev: str, to_rev: str) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/-/compare/{from_rev}...{to_rev}"
+        return self.create_server_url(
+            path=f"{self.owner}/{self.repo_name}/-/compare/{from_rev}...{to_rev}"
+        )
 
     def remote_url(self, use_token: bool = True) -> str:
         """Get the remote url including the token for authentication if requested"""
         if not (self.token and use_token):
             return self._remote_url
-        return f"https://gitlab-ci-token:{self.token}@{self.hvcs_domain}/{self.owner}/{self.repo_name}.git"
+
+        return self.create_server_url(
+            auth=f"gitlab-ci-token:{self.token}",
+            path=f"{self.owner}/{self.repo_name}.git",
+        )
 
     def commit_hash_url(self, commit_hash: str) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/-/commit/{commit_hash}"
+        return self.create_server_url(
+            path=f"{self.owner}/{self.repo_name}/-/commit/{commit_hash}"
+        )
+
+    def issue_url(self, issue_number: str | int) -> str:
+        return self.create_server_url(
+            path=f"{self.owner}/{self.repo_name}/-/issues/{issue_number}"
+        )
+
+    def merge_request_url(self, mr_number: str | int) -> str:
+        return self.create_server_url(
+            path=f"{self.owner}/{self.repo_name}/-/merge_requests/{mr_number}"
+        )
 
     def pull_request_url(self, pr_number: str | int) -> str:
-        return f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/-/issues/{pr_number}"
+        return self.merge_request_url(mr_number=pr_number)
+
+    def create_server_url(
+        self,
+        path: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        overrides = dict(
+            filter(
+                lambda x: x[1] is not None,
+                {
+                    "auth": auth,
+                    "path": str(PurePosixPath(path or "/")),
+                    "query": query,
+                    "fragment": fragment,
+                }.items(),
+            )
+        )
+        return Url(
+            **{
+                **self.hvcs_domain._asdict(),
+                **overrides,
+            }
+        ).url.rstrip("/")
+
+    def create_api_url(
+        self,
+        endpoint: str,
+        auth: str | None = None,
+        query: str | None = None,
+        fragment: str | None = None,
+    ) -> str:
+        api_path = self._client.api_url.replace(self.hvcs_domain.url, "")
+        return self.create_server_url(
+            path=f"{api_path}/{endpoint.lstrip(api_path)}",
+            auth=auth,
+            query=query,
+            fragment=fragment,
+        )
```

### Comparing `python-semantic-release-9.4.1/semantic_release/hvcs/token_auth.py` & `python_semantic_release-9.4.2/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/hvcs/util.py` & `python_semantic_release-9.4.2/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/version/algorithm.py` & `python_semantic_release-9.4.2/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/version/declaration.py` & `python_semantic_release-9.4.2/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/version/translator.py` & `python_semantic_release-9.4.2/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/semantic_release/version/version.py` & `python_semantic_release-9.4.2/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/command_line/conftest.py` & `python_semantic_release-9.4.2/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/command_line/test_changelog.py` & `python_semantic_release-9.4.2/tests/command_line/test_changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 import pytest
 import requests_mock
 from pytest_lazyfixture import lazy_fixture
 from requests import Session
 
 from semantic_release.cli import changelog, main
-from semantic_release.hvcs import Github
 
 from tests.const import (
+    EXAMPLE_HVCS_DOMAIN,
     EXAMPLE_RELEASE_NOTES_TEMPLATE,
     EXAMPLE_REPO_NAME,
     EXAMPLE_REPO_OWNER,
     SUCCESS_EXIT_CODE,
 )
 from tests.fixtures.repos import (
     repo_w_github_flow_w_feature_release_channel_angular_commits,
@@ -237,30 +237,28 @@
     mock_adapter = requests_mock.Adapter()
     mock_adapter.register_uri(
         method=requests_mock.ANY, url=requests_mock.ANY, json={"id": 10001}
     )
     session.mount("http://", mock_adapter)
     session.mount("https://", mock_adapter)
 
-    expected_request_url = (
-        "https://{api_url}/repos/{owner}/{repo_name}/releases".format(
-            api_url=Github.DEFAULT_API_DOMAIN,
-            owner=EXAMPLE_REPO_OWNER,
-            repo_name=EXAMPLE_REPO_NAME,
-        )
+    expected_request_url = "{api_url}/repos/{owner}/{repo_name}/releases".format(
+        # TODO: Fix as this is likely not correct given a custom domain and the
+        # use of GitHub which would be GitHub Enterprise Server which we don't yet support
+        api_url=f"https://api.{EXAMPLE_HVCS_DOMAIN}",  # GitHub API URL
+        owner=EXAMPLE_REPO_OWNER,
+        repo_name=EXAMPLE_REPO_NAME,
     )
 
     # Patch out env vars that affect changelog URLs but only get set in e.g.
     # Github actions
     with mock.patch(
         "semantic_release.hvcs.github.build_requests_session",
         return_value=session,
-    ) as mocker, monkeypatch.context() as m:
-        m.delenv("GITHUB_REPOSITORY", raising=False)
-        m.delenv("CI_PROJECT_NAMESPACE", raising=False)
+    ) as mocker, mock.patch.dict("os.environ", {}, clear=True):
         result = cli_runner.invoke(main, [changelog_subcmd, *args])
 
     assert SUCCESS_EXIT_CODE == result.exit_code  # noqa: SIM300
 
     assert mocker.called
     assert mock_adapter.called
     assert mock_adapter.last_request is not None
```

### Comparing `python-semantic-release-9.4.1/tests/command_line/test_generate_config.py` & `python_semantic_release-9.4.2/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/command_line/test_help.py` & `python_semantic_release-9.4.2/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/command_line/test_main.py` & `python_semantic_release-9.4.2/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/command_line/test_publish.py` & `python_semantic_release-9.4.2/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/command_line/test_version.py` & `python_semantic_release-9.4.2/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/const.py` & `python_semantic_release-9.4.2/tests/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/commit_parsers.py` & `python_semantic_release-9.4.2/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/example_project.py` & `python_semantic_release-9.4.2/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/git_repo.py` & `python_semantic_release-9.4.2/tests/fixtures/git_repo.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                 hvcs_class = use_gitea_hvcs(hvcs_domain)
             elif hvcs_client_name == "bitbucket":
                 hvcs_class = use_bitbucket_hvcs(hvcs_domain)
             else:
                 raise ValueError(f"Unknown HVCS client name: {hvcs_client_name}")
 
             # Create HVCS Client instance
-            hvcs = hvcs_class(example_git_https_url, hvcs_domain)
+            hvcs = hvcs_class(example_git_https_url, hvcs_domain=hvcs_domain)
 
             # Set tag format in configuration
             if tag_format_str is not None:
                 update_pyproject_toml(
                     "tool.semantic_release.tag_format", tag_format_str
                 )
```

### Comparing `python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python_semantic_release-9.4.2/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python_semantic_release-9.4.2/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python_semantic_release-9.4.2/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/fixtures/scipy.py` & `python_semantic_release-9.4.2/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/scenario/test_next_version.py` & `python_semantic_release-9.4.2/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/scenario/test_release_history.py` & `python_semantic_release-9.4.2/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/scenario/test_template_render.py` & `python_semantic_release-9.4.2/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         unreleased={
             "feature": [feat_commit_parsed],
         },
         released={
             version: Release(
                 tagger=commit_author,
                 committer=commit_author,
-                tagged_date=datetime.utcnow(),
+                tagged_date=datetime.now(),
                 elements={
                     "feature": [feat_commit_parsed],
                     "fix": [fix_commit_parsed],
                 },
             )
         },
     )
```

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_release_notes.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     return ReleaseHistory(
         unreleased={},
         released={
             version: Release(
                 tagger=commit_author,
                 committer=commit_author,
-                tagged_date=datetime.utcnow(),
+                tagged_date=datetime.now(),
                 elements={
                     "fix": [fix_commit_parsed],
                 },
             )
         },
     )
```

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_template.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_config.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from unittest import mock
 
 import pytest
 import tomlkit
 from pydantic import RootModel, ValidationError
 
 from semantic_release.cli.config import (
-    EnvConfigVar,
     GlobalCommandLineOptions,
     HvcsClient,
     RawConfig,
     RuntimeContext,
 )
 from semantic_release.commit_parser.angular import AngularParserOptions
 from semantic_release.commit_parser.emoji import EmojiParserOptions
@@ -28,34 +27,56 @@
     from pathlib import Path
     from typing import Any
 
     from tests.fixtures.example_project import ExProjectDir
 
 
 @pytest.mark.parametrize(
-    "remote_config, expected_token",
+    "patched_os_environ, remote_config, expected_token",
     [
-        ({"type": HvcsClient.GITHUB.value}, EnvConfigVar(env="GH_TOKEN")),
-        ({"type": HvcsClient.GITLAB.value}, EnvConfigVar(env="GITLAB_TOKEN")),
-        ({"type": HvcsClient.GITEA.value}, EnvConfigVar(env="GITEA_TOKEN")),
-        ({}, EnvConfigVar(env="GH_TOKEN")),  # default not provided -> means Github
         (
+            {"GH_TOKEN": "mytoken"},
+            {"type": HvcsClient.GITHUB.value},
+            "mytoken",
+        ),
+        (
+            {"GITLAB_TOKEN": "mytoken"},
+            {"type": HvcsClient.GITLAB.value},
+            "mytoken",
+        ),
+        (
+            {"GITEA_TOKEN": "mytoken"},
+            {"type": HvcsClient.GITEA.value},
+            "mytoken",
+        ),
+        (
+            # default not provided -> means Github
+            {"GH_TOKEN": "mytoken"},
+            {},
+            "mytoken",
+        ),
+        (
+            {"CUSTOM_TOKEN": "mytoken"},
             {"type": HvcsClient.GITHUB.value, "token": {"env": "CUSTOM_TOKEN"}},
-            EnvConfigVar(env="CUSTOM_TOKEN"),
+            "mytoken",
         ),
     ],
 )
 def test_load_hvcs_default_token(
-    remote_config: dict[str, Any], expected_token: EnvConfigVar
+    patched_os_environ: dict[str, str],
+    remote_config: dict[str, Any],
+    expected_token: str,
 ):
-    raw_config = RawConfig.model_validate(
-        {
-            "remote": remote_config,
-        }
-    )
+    with mock.patch.dict("os.environ", patched_os_environ, clear=True):
+        raw_config = RawConfig.model_validate(
+            {
+                "remote": remote_config,
+            }
+        )
+
     assert expected_token == raw_config.remote.token
 
 
 @pytest.mark.parametrize("remote_config", [{"type": "nonexistent"}])
 def test_invalid_hvcs_type(remote_config: dict[str, Any]):
     with pytest.raises(ValidationError) as excinfo:
         RawConfig.model_validate(
```

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_masking_filter.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_util.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_version.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_angular.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_tag.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_token.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_util.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test__base.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_github.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import base64
+import fnmatch
 import glob
 import mimetypes
 import os
 import re
 from typing import TYPE_CHECKING
 from unittest import mock
 from urllib.parse import urlencode
@@ -12,724 +13,995 @@
 import pytest
 import requests_mock
 from requests import HTTPError, Response, Session
 
 from semantic_release.hvcs.github import Github
 from semantic_release.hvcs.token_auth import TokenAuth
 
-from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER, RELEASE_NOTES
-from tests.util import netrc_file
+from tests.const import (
+    EXAMPLE_HVCS_DOMAIN,
+    EXAMPLE_REPO_NAME,
+    EXAMPLE_REPO_OWNER,
+    RELEASE_NOTES,
+)
+from tests.fixtures.example_project import init_example_project
 
 if TYPE_CHECKING:
     from pathlib import Path
+    from typing import Generator
+
+    from tests.conftest import NetrcFileFn
 
 
 @pytest.fixture
-def default_gh_client():
-    remote_url = f"git@github.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
-    return Github(remote_url=remote_url)
+def default_gh_client() -> Generator[Github, None, None]:
+    remote_url = (
+        f"git@{Github.DEFAULT_DOMAIN}:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
+    )
+    with mock.patch.dict(os.environ, {}, clear=True):
+        yield Github(remote_url=remote_url)
 
 
 @pytest.mark.parametrize(
-    (
-        "patched_os_environ, hvcs_domain, hvcs_api_domain, "
-        "expected_hvcs_domain, expected_hvcs_api_domain"
+    str.join(
+        ", ",
+        [
+            "patched_os_environ",
+            "hvcs_domain",
+            "hvcs_api_domain",
+            "expected_hvcs_domain",
+            "expected_hvcs_api_url",
+            "insecure",
+        ],
     ),
     [
-        ({}, None, None, Github.DEFAULT_DOMAIN, Github.DEFAULT_API_DOMAIN),
         (
-            {"GITHUB_SERVER_URL": "https://special.custom.server/vcs/"},
+            # Default values
+            {},
+            None,
+            None,
+            f"https://{Github.DEFAULT_DOMAIN}",
+            f"https://{Github.DEFAULT_API_DOMAIN}",
+            False,
+        ),
+        (
+            # Gather domain from environment & imply api domain from server domain
+            {"GITHUB_SERVER_URL": "https://special.custom.server/"},
             None,
             None,
-            "special.custom.server/vcs/",
-            Github.DEFAULT_API_DOMAIN,
+            "https://special.custom.server",
+            "https://api.special.custom.server",
+            False,
         ),
         (
-            {"GITHUB_API_URL": "https://api.special.custom.server/"},
+            # Pull both locations from environment
+            {
+                "GITHUB_SERVER_URL": "https://special.custom.server/",
+                "GITHUB_API_URL": "https://api2.special.custom.server/",
+            },
             None,
             None,
-            Github.DEFAULT_DOMAIN,
-            "api.special.custom.server/",
+            "https://special.custom.server",
+            "https://api2.special.custom.server",
+            False,
         ),
         (
+            # Ignore environment & use provided parameter value (ie from user config)
+            # then infer api domain from the parameter value based on default GitHub configurations
             {"GITHUB_SERVER_URL": "https://special.custom.server/vcs/"},
-            "https://example.com",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
             None,
-            "https://example.com",
-            Github.DEFAULT_API_DOMAIN,
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            False,
         ),
         (
+            # Ignore environment & use provided parameter value (ie from user config)
             {"GITHUB_API_URL": "https://api.special.custom.server/"},
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://api.{EXAMPLE_HVCS_DOMAIN}",
+            False,
+        ),
+        (
+            # Allow insecure http connections explicitly
+            {},
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            True,
+        ),
+        (
+            # Allow insecure http connections explicitly & imply insecure api domain
+            {},
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
             None,
-            "https://api.example.com",
-            Github.DEFAULT_DOMAIN,
-            "https://api.example.com",
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            True,
+        ),
+        (
+            # Infer insecure connection from user configuration
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            f"api.{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            True,
+        ),
+        (
+            # Infer insecure connection from user configuration & imply insecure api domain
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            None,
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://api.{EXAMPLE_HVCS_DOMAIN}",
+            True,
         ),
     ],
 )
 @pytest.mark.parametrize(
     "remote_url",
     [
-        f"git@github.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
-        f"https://github.com/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
+        f"git@{Github.DEFAULT_DOMAIN}:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
+        f"https://{Github.DEFAULT_DOMAIN}/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
     ],
 )
 @pytest.mark.parametrize("token", ("abc123", None))
 def test_github_client_init(
-    patched_os_environ,
-    hvcs_domain,
-    hvcs_api_domain,
-    expected_hvcs_domain,
-    expected_hvcs_api_domain,
-    remote_url,
-    token,
+    patched_os_environ: dict[str, str],
+    hvcs_domain: str | None,
+    hvcs_api_domain: str | None,
+    expected_hvcs_domain: str,
+    expected_hvcs_api_url: str,
+    remote_url: str,
+    token: str | None,
+    insecure: bool,
 ):
     with mock.patch.dict(os.environ, patched_os_environ, clear=True):
         client = Github(
             remote_url=remote_url,
             hvcs_domain=hvcs_domain,
             hvcs_api_domain=hvcs_api_domain,
             token=token,
+            allow_insecure=insecure,
         )
 
-        assert client.hvcs_domain == expected_hvcs_domain
-        assert client.hvcs_api_domain == expected_hvcs_api_domain
-        assert client.api_url == f"https://{client.hvcs_api_domain}"
-        assert client.token == token
-        assert client._remote_url == remote_url
+        # Evaluate (expected -> actual)
+        assert expected_hvcs_domain == str(client.hvcs_domain)
+        assert expected_hvcs_api_url == str(client.api_url)
+        assert token == client.token
+        assert remote_url == client._remote_url
         assert hasattr(client, "session")
         assert isinstance(getattr(client, "session", None), Session)
 
 
 @pytest.mark.parametrize(
+    "hvcs_domain, hvcs_api_domain, insecure",
+    [
+        # Bad base domain schemes
+        (f"ftp://{EXAMPLE_HVCS_DOMAIN}", None, False),
+        (f"ftp://{EXAMPLE_HVCS_DOMAIN}", None, True),
+        # Unallowed insecure connections when base domain is insecure
+        (f"http://{EXAMPLE_HVCS_DOMAIN}", None, False),
+        # Bad API domain schemes
+        (None, f"ftp://api.{EXAMPLE_HVCS_DOMAIN}", False),
+        (None, f"ftp://api.{EXAMPLE_HVCS_DOMAIN}", True),
+        # Unallowed insecure connections when api domain is insecure
+        (None, f"http://{EXAMPLE_HVCS_DOMAIN}", False),
+    ],
+)
+def test_github_client_init_with_invalid_scheme(
+    hvcs_domain: str | None,
+    hvcs_api_domain: str | None,
+    insecure: bool,
+):
+    with pytest.raises(ValueError), mock.patch.dict(os.environ, {}, clear=True):
+        Github(
+            remote_url=f"https://{EXAMPLE_HVCS_DOMAIN}/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
+            hvcs_domain=hvcs_domain,
+            hvcs_api_domain=hvcs_api_domain,
+            allow_insecure=insecure,
+        )
+
+
+@pytest.mark.parametrize(
     "patched_os_environ, expected_owner, expected_name",
     [
         ({}, None, None),
         ({"GITHUB_REPOSITORY": "path/to/repo/foo"}, "path/to/repo", "foo"),
     ],
 )
 def test_github_get_repository_owner_and_name(
-    default_gh_client, patched_os_environ, expected_owner, expected_name
+    default_gh_client: Github,
+    patched_os_environ: dict[str, str],
+    expected_owner: str,
+    expected_name: str,
 ):
+    # expected results should be a tuple[namespace, repo_name]
+    # when None, the default values are used which matches default_gh_client's setup
+    expected_result = (
+        expected_owner or EXAMPLE_REPO_OWNER,
+        expected_name or EXAMPLE_REPO_NAME,
+    )
+
     with mock.patch.dict(os.environ, patched_os_environ, clear=True):
-        if expected_owner is None and expected_name is None:
-            assert (
-                default_gh_client._get_repository_owner_and_name()
-                == super(Github, default_gh_client)._get_repository_owner_and_name()
-            )
-        else:
-            assert default_gh_client._get_repository_owner_and_name() == (
-                expected_owner,
-                expected_name,
-            )
+        # Execute in mocked environment
+        result = default_gh_client._get_repository_owner_and_name()
+
+        # Evaluate (expected -> actual)
+        assert expected_result == result
 
 
-def test_compare_url(default_gh_client):
-    assert default_gh_client.compare_url(
-        from_rev="revA", to_rev="revB"
-    ) == "https://{domain}/{owner}/{repo}/compare/revA...revB".format(
-        domain=default_gh_client.hvcs_domain,
+def test_compare_url(default_gh_client: Github):
+    # Setup
+    start_rev = "revA"
+    end_rev = "revB"
+    expected_url = "{server}/{owner}/{repo}/compare/{from_rev}...{to_rev}".format(
+        server=default_gh_client.hvcs_domain,
         owner=default_gh_client.owner,
         repo=default_gh_client.repo_name,
+        from_rev=start_rev,
+        to_rev=end_rev,
     )
 
+    # Execute method under test
+    actual_url = default_gh_client.compare_url(from_rev=start_rev, to_rev=end_rev)
+
+    # Evaluate (expected -> actual)
+    assert expected_url == actual_url
+
 
 @pytest.mark.parametrize(
-    "patched_os_environ, use_token, token, _remote_url, expected",
+    "patched_os_environ, use_token, token, remote_url, expected_auth_url",
     [
         (
             {"GITHUB_ACTOR": "foo"},
             False,
             "",
-            "git@github.com:custom/example.git",
-            "git@github.com:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             {"GITHUB_ACTOR": "foo"},
             True,
             "",
-            "git@github.com:custom/example.git",
-            "git@github.com:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             {},
             False,
             "aabbcc",
-            "git@github.com:custom/example.git",
-            "git@github.com:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             {},
             True,
             "aabbcc",
-            "git@github.com:custom/example.git",
-            "https://aabbcc@github.com/custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
+            f"https://aabbcc@{Github.DEFAULT_DOMAIN}/custom/example.git",
         ),
         (
             {"GITHUB_ACTOR": "foo"},
             False,
             "aabbcc",
-            "git@github.com:custom/example.git",
-            "git@github.com:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             {"GITHUB_ACTOR": "foo"},
             True,
             "aabbcc",
-            "git@github.com:custom/example.git",
-            "https://foo:aabbcc@github.com/custom/example.git",
+            f"git@{Github.DEFAULT_DOMAIN}:custom/example.git",
+            f"https://foo:aabbcc@{Github.DEFAULT_DOMAIN}/custom/example.git",
         ),
     ],
 )
 def test_remote_url(
-    patched_os_environ,
-    use_token,
-    token,
-    # TODO: linter thinks this is a fixture not a param - why?
-    _remote_url,  # noqa: PT019
-    expected,
-    default_gh_client,
+    default_gh_client: Github,
+    patched_os_environ: dict[str, str],
+    use_token: bool,
+    token: str,
+    remote_url: str,
+    expected_auth_url: str,
 ):
     with mock.patch.dict(os.environ, patched_os_environ, clear=True):
-        default_gh_client._remote_url = _remote_url
+        default_gh_client._remote_url = remote_url
         default_gh_client.token = token
-        assert default_gh_client.remote_url(use_token=use_token) == expected
+
+        # Execute method under test & Evaluate (expected -> actual)
+        assert expected_auth_url == default_gh_client.remote_url(use_token=use_token)
 
 
-def test_commit_hash_url(default_gh_client):
+def test_commit_hash_url(default_gh_client: Github):
     sha = "hashashash"
-    assert default_gh_client.commit_hash_url(
-        sha
-    ) == "https://{domain}/{owner}/{repo}/commit/{sha}".format(
-        domain=default_gh_client.hvcs_domain,
+    expected_url = "{server}/{owner}/{repo}/commit/{sha}".format(
+        server=default_gh_client.hvcs_domain.url,
         owner=default_gh_client.owner,
         repo=default_gh_client.repo_name,
         sha=sha,
     )
+    assert expected_url == default_gh_client.commit_hash_url(sha)
 
 
 @pytest.mark.parametrize("pr_number", (420, "420"))
-def test_pull_request_url(default_gh_client, pr_number):
-    assert default_gh_client.pull_request_url(
-        pr_number=pr_number
-    ) == "https://{domain}/{owner}/{repo}/issues/{pr_number}".format(
-        domain=default_gh_client.hvcs_domain,
+def test_pull_request_url(default_gh_client: Github, pr_number: int | str):
+    expected_url = "{server}/{owner}/{repo}/issues/{pr_number}".format(
+        server=default_gh_client.hvcs_domain,
         owner=default_gh_client.owner,
         repo=default_gh_client.repo_name,
         pr_number=pr_number,
     )
+    actual_url = default_gh_client.pull_request_url(pr_number=pr_number)
+    assert expected_url == actual_url
 
 
 ############
 # Tests which need http response mocking
 ############
 
 
+github_upload_url = f"https://uploads.{Github.DEFAULT_DOMAIN}"
 github_matcher = re.compile(rf"^https://{Github.DEFAULT_DOMAIN}")
 github_api_matcher = re.compile(rf"^https://{Github.DEFAULT_API_DOMAIN}")
-github_upload_matcher = re.compile(rf"^https://{Github.DEFAULT_UPLOAD_DOMAIN}")
+github_upload_matcher = re.compile(rf"^{github_upload_url}")
 
 
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_succeeds(
-    default_gh_client, status_code, prerelease, mock_release_id
+    default_gh_client: Github,
+    mock_release_id: int,
+    prerelease: bool,
+    status_code: int,
 ):
     tag = "v1.0.0"
+    expected_num_requests = 1
+    expected_http_method = "POST"
+    expected_request_url = "{api_url}/repos/{owner}/{repo_name}/releases".format(
+        api_url=default_gh_client.api_url,
+        owner=default_gh_client.owner,
+        repo_name=default_gh_client.repo_name,
+    )
+    expected_request_body = {
+        "tag_name": tag,
+        "name": tag,
+        "body": RELEASE_NOTES,
+        "draft": False,
+        "prerelease": prerelease,
+    }
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the response
         m.register_uri(
             "POST",
             github_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
-        assert (
-            default_gh_client.create_release(tag, RELEASE_NOTES, prerelease)
-            == mock_release_id
+
+        # Execute method under test
+        actual_rtn_val = default_gh_client.create_release(
+            tag, RELEASE_NOTES, prerelease
         )
+
+        # Evaluate (expected -> actual)
+        assert mock_release_id == actual_rtn_val
         assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "POST"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-            )
-        )
-        assert m.last_request.json() == {
-            "tag_name": tag,
-            "name": tag,
-            "body": RELEASE_NOTES,
-            "draft": False,
-            "prerelease": prerelease,
-        }
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_request_url == m.last_request.url
+        assert expected_request_body == m.last_request.json()
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
+@pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
-def test_create_release_fails(default_gh_client, prerelease, status_code):
+def test_create_release_fails(
+    default_gh_client: Github,
+    mock_release_id: int,
+    prerelease: bool,
+    status_code: int,
+):
     tag = "v1.0.0"
+    expected_num_requests = 1
+    expected_http_method = "POST"
+    expected_request_url = "{api_url}/repos/{owner}/{repo_name}/releases".format(
+        api_url=default_gh_client.api_url,
+        owner=default_gh_client.owner,
+        repo_name=default_gh_client.repo_name,
+    )
+    expected_request_body = {
+        "tag_name": tag,
+        "name": tag,
+        "body": RELEASE_NOTES,
+        "draft": False,
+        "prerelease": prerelease,
+    }
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the response
         m.register_uri(
-            "POST", github_api_matcher, json={"id": 1}, status_code=status_code
+            "POST",
+            github_api_matcher,
+            json={"id": mock_release_id},
+            status_code=status_code,
         )
 
+        # Execute method under test expecting an exeception to be raised
         with pytest.raises(HTTPError):
             default_gh_client.create_release(tag, RELEASE_NOTES, prerelease)
 
+        # Evaluate (expected -> actual)
         assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "POST"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-            )
-        )
-        assert m.last_request.json() == {
-            "tag_name": tag,
-            "name": tag,
-            "body": RELEASE_NOTES,
-            "draft": False,
-            "prerelease": prerelease,
-        }
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_request_url == m.last_request.url
+        assert expected_request_body == m.last_request.json()
 
 
 @pytest.mark.parametrize("token", (None, "super-token"))
-def test_should_create_release_using_token_or_netrc(default_gh_client, token):
+def test_should_create_release_using_token_or_netrc(
+    default_gh_client: Github,
+    token: str | None,
+    default_netrc_username: str,
+    default_netrc_password: str,
+    netrc_file: NetrcFileFn,
+):
+    # Setup
     default_gh_client.token = token
     default_gh_client.session.auth = None if not token else TokenAuth(token)
     tag = "v1.0.0"
-    with requests_mock.Mocker(session=default_gh_client.session) as m, netrc_file(
-        machine=default_gh_client.DEFAULT_API_DOMAIN
-    ) as netrc, mock.patch.dict(os.environ, {"NETRC": netrc.name}, clear=True):
-        m.register_uri("POST", github_api_matcher, json={"id": 1}, status_code=201)
-        assert default_gh_client.create_release(tag, RELEASE_NOTES) == 1
-        assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "POST"
-        if not token:
-            assert {
-                "Authorization": "Basic "
-                + base64.encodebytes(
-                    f"{netrc.login_username}:{netrc.login_password}".encode()
-                )
-                .decode("ascii")
-                .strip()
-            }.items() <= m.last_request.headers.items()
-        else:
-            assert {
-                "Authorization": f"token {token}"
-            }.items() <= m.last_request.headers.items()
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-            )
+    expected_release_id = 1
+    expected_num_requests = 1
+    expected_http_method = "POST"
+    expected_request_url = "{api_url}/repos/{owner}/{repo_name}/releases".format(
+        api_url=default_gh_client.api_url,
+        owner=default_gh_client.owner,
+        repo_name=default_gh_client.repo_name,
+    )
+    expected_request_body = {
+        "tag_name": tag,
+        "name": tag,
+        "body": RELEASE_NOTES,
+        "draft": False,
+        "prerelease": False,
+    }
+
+    encoded_auth = (
+        base64.encodebytes(
+            f"{default_netrc_username}:{default_netrc_password}".encode()
+        )
+        .decode("ascii")
+        .strip()
+    )
+
+    expected_request_headers = (
+        {"Authorization": f"token {token}"}
+        if token
+        else {"Authorization": f"Basic {encoded_auth}"}
+    ).items()
+
+    # create netrc file
+    netrc = netrc_file(machine=default_gh_client.DEFAULT_API_DOMAIN)
+
+    # Monkeypatch to create the Mocked environment
+    with requests_mock.Mocker(session=default_gh_client.session) as m, mock.patch.dict(
+        os.environ, {"NETRC": netrc.name}, clear=True
+    ):
+        # mock the response
+        m.register_uri(
+            "POST",
+            github_api_matcher,
+            json={"id": expected_release_id},
+            status_code=201,
         )
-        assert m.last_request.json() == {
-            "tag_name": tag,
-            "name": tag,
-            "body": RELEASE_NOTES,
-            "draft": False,
-            "prerelease": False,
-        }
+
+        # Execute method under test
+        ret_val = default_gh_client.create_release(tag, RELEASE_NOTES)
+
+        # Evaluate (expected -> actual)
+        assert expected_release_id == ret_val
+        assert m.called
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_request_url == m.last_request.url
+        assert expected_request_headers <= m.last_request.headers.items()
+        assert expected_request_body == m.last_request.json()
 
 
 def test_request_has_no_auth_header_if_no_token_or_netrc():
+    tag = "v1.0.0"
+    expected_release_id = 1
+    expected_num_requests = 1
+    expected_http_method = "POST"
+
     with mock.patch.dict(os.environ, {}, clear=True):
-        client = Github(remote_url="git@github.com:something/somewhere.git")
+        client = Github(
+            remote_url=f"git@{Github.DEFAULT_DOMAIN}:something/somewhere.git"
+        )
+
+        expected_request_url = "{api_url}/repos/{owner}/{repo_name}/releases".format(
+            api_url=client.api_url,
+            owner=client.owner,
+            repo_name=client.repo_name,
+        )
 
         with requests_mock.Mocker(session=client.session) as m:
+            # mock the response
             m.register_uri("POST", github_api_matcher, json={"id": 1}, status_code=201)
-            assert client.create_release("v1.0.0", RELEASE_NOTES) == 1
+
+            # Execute method under test
+            rtn_val = client.create_release(tag, RELEASE_NOTES)
+
+            # Evaluate (expected -> actual)
+            assert expected_release_id == rtn_val
             assert m.called
-            assert len(m.request_history) == 1
-            assert m.last_request.method == "POST"
-            assert (
-                m.last_request.url
-                == f"{client.api_url}/repos/{client.owner}/{client.repo_name}/releases"
-            )
+            assert expected_num_requests == len(m.request_history)
+            assert expected_http_method == m.last_request.method
+            assert expected_request_url == m.last_request.url
             assert "Authorization" not in m.last_request.headers
 
 
 @pytest.mark.parametrize("status_code", [201])
 @pytest.mark.parametrize("mock_release_id", range(3))
-def test_edit_release_notes_succeeds(default_gh_client, status_code, mock_release_id):
+def test_edit_release_notes_succeeds(
+    default_gh_client: Github,
+    status_code: int,
+    mock_release_id: int,
+):
+    # Setup
+    expected_num_requests = 1
+    expected_http_method = "POST"
+    expected_request_url = (
+        "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
+            api_url=default_gh_client.api_url,
+            owner=default_gh_client.owner,
+            repo_name=default_gh_client.repo_name,
+            release_id=mock_release_id,
+        )
+    )
+    expected_request_body = {"body": RELEASE_NOTES}
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the response
         m.register_uri(
             "POST",
             github_api_matcher,
             json={"id": mock_release_id},
             status_code=status_code,
         )
-        assert (
-            default_gh_client.edit_release_notes(mock_release_id, RELEASE_NOTES)
-            == mock_release_id
-        )
+
+        # Execute method under test
+        rtn_val = default_gh_client.edit_release_notes(mock_release_id, RELEASE_NOTES)
+
+        # Evaluate (expected -> actual)
+        assert mock_release_id == rtn_val
         assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "POST"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-                release_id=mock_release_id,
-            )
-        )
-        assert m.last_request.json() == {"body": RELEASE_NOTES}
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_request_url == m.last_request.url
+        assert expected_request_body == m.last_request.json()
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
-def test_edit_release_notes_fails(default_gh_client, status_code):
-    release_id = 420
+@pytest.mark.parametrize("mock_release_id", range(3))
+def test_edit_release_notes_fails(
+    default_gh_client: Github, status_code: int, mock_release_id: int
+):
+    # Setup
+    expected_num_requests = 1
+    expected_http_method = "POST"
+    expected_request_url = (
+        "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
+            api_url=default_gh_client.api_url,
+            owner=default_gh_client.owner,
+            repo_name=default_gh_client.repo_name,
+            release_id=mock_release_id,
+        )
+    )
+    expected_request_body = {"body": RELEASE_NOTES}
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the response
         m.register_uri(
-            "POST", github_api_matcher, json={"id": release_id}, status_code=status_code
+            "POST",
+            github_api_matcher,
+            json={"id": mock_release_id},
+            status_code=status_code,
         )
 
+        # Execute method under test expecting an exception to be raised
         with pytest.raises(HTTPError):
-            default_gh_client.edit_release_notes(release_id, RELEASE_NOTES)
+            default_gh_client.edit_release_notes(mock_release_id, RELEASE_NOTES)
 
+        # Evaluate (expected -> actual)
         assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "POST"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-                release_id=release_id,
-            )
-        )
-        assert m.last_request.json() == {"body": RELEASE_NOTES}
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_request_url == m.last_request.url
+        assert expected_request_body == m.last_request.json()
 
 
 @pytest.mark.parametrize(
-    "resp_payload, status_code, expected",
+    "resp_payload, status_code, expected_result",
     [
         ({"id": 420, "status": "success"}, 200, 420),
         ({"error": "not found"}, 404, None),
         ({"error": "too many requests"}, 429, None),
         ({"error": "internal error"}, 500, None),
         ({"error": "temporarily unavailable"}, 503, None),
     ],
 )
-def test_get_release_id_by_tag(default_gh_client, resp_payload, status_code, expected):
+def test_get_release_id_by_tag(
+    default_gh_client: Github,
+    resp_payload: dict[str, int],
+    status_code: int,
+    expected_result: int | None,
+):
+    # Setup
     tag = "v1.0.0"
+    expected_num_requests = 1
+    expected_http_method = "GET"
+    expected_request_url = (
+        "{api_url}/repos/{owner}/{repo_name}/releases/tags/{tag}".format(
+            api_url=default_gh_client.api_url,
+            owner=default_gh_client.owner,
+            repo_name=default_gh_client.repo_name,
+            tag=tag,
+        )
+    )
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the response
         m.register_uri(
             "GET", github_api_matcher, json=resp_payload, status_code=status_code
         )
-        assert default_gh_client.get_release_id_by_tag(tag) == expected
+
+        # Execute method under test
+        rtn_val = default_gh_client.get_release_id_by_tag(tag)
+
+        # Evaluate (expected -> actual)
+        assert expected_result == rtn_val
         assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "GET"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases/tags/{tag}".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-                tag=tag,
-            )
-        )
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_request_url == m.last_request.url
 
 
 # Note - mocking as the logic for the create/update of a release
 # is covered by testing above, no point re-testing.
 
 
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_succeeds(
-    default_gh_client,
-    mock_release_id,
-    prerelease,
+    default_gh_client: Github,
+    mock_release_id: int,
+    prerelease: bool,
 ):
     tag = "v1.0.0"
     with mock.patch.object(
-        default_gh_client, "create_release"
+        default_gh_client, "create_release", return_value=mock_release_id
     ) as mock_create_release, mock.patch.object(
-        default_gh_client, "get_release_id_by_tag"
+        default_gh_client, "get_release_id_by_tag", return_value=mock_release_id
     ) as mock_get_release_id_by_tag, mock.patch.object(
-        default_gh_client, "edit_release_notes"
+        default_gh_client, "edit_release_notes", return_value=mock_release_id
     ) as mock_edit_release_notes:
-        mock_create_release.return_value = mock_release_id
-        mock_get_release_id_by_tag.return_value = mock_release_id
-        mock_edit_release_notes.return_value = mock_release_id
-        assert (
-            default_gh_client.create_or_update_release(tag, RELEASE_NOTES, prerelease)
-            == mock_release_id
+        # Execute in mock environment
+        result = default_gh_client.create_or_update_release(
+            tag, RELEASE_NOTES, prerelease
         )
+
+        # Evaluate (expected -> actual)
+        assert mock_release_id == result
         mock_create_release.assert_called_once_with(tag, RELEASE_NOTES, prerelease)
         mock_get_release_id_by_tag.assert_not_called()
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_update_succeeds(
-    default_gh_client,
-    mock_release_id,
-    prerelease,
+    default_gh_client: Github,
+    mock_release_id: int,
+    prerelease: bool,
 ):
     tag = "v1.0.0"
-    not_found = HTTPError("404 Not Found", response=Response())
+    not_found = HTTPError("404 Not Found")
+    not_found.response = Response()
     not_found.response.status_code = 404
+
     with mock.patch.object(
-        default_gh_client, "create_release"
+        default_gh_client,
+        "create_release",
+        side_effect=not_found,
     ) as mock_create_release, mock.patch.object(
-        default_gh_client, "get_release_id_by_tag"
+        default_gh_client,
+        "get_release_id_by_tag",
+        return_value=mock_release_id,
     ) as mock_get_release_id_by_tag, mock.patch.object(
-        default_gh_client, "edit_release_notes"
+        default_gh_client,
+        "edit_release_notes",
+        return_value=mock_release_id,
     ) as mock_edit_release_notes:
-        mock_create_release.side_effect = not_found
-        mock_get_release_id_by_tag.return_value = mock_release_id
-        mock_edit_release_notes.return_value = mock_release_id
-        assert (
-            default_gh_client.create_or_update_release(tag, RELEASE_NOTES, prerelease)
-            == mock_release_id
+        # Execute in mock environment
+        result = default_gh_client.create_or_update_release(
+            tag, RELEASE_NOTES, prerelease
         )
+
+        # Evaluate (expected -> actual)
+        assert mock_release_id == result
+        mock_create_release.assert_called_once()
         mock_get_release_id_by_tag.assert_called_once_with(tag)
         mock_edit_release_notes.assert_called_once_with(mock_release_id, RELEASE_NOTES)
 
 
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_no_release_for_tag(
-    default_gh_client, prerelease
+    default_gh_client: Github,
+    prerelease: bool,
 ):
     tag = "v1.0.0"
-    not_found = HTTPError("404 Not Found", response=Response())
+    not_found = HTTPError("404 Not Found")
+    not_found.response = Response()
     not_found.response.status_code = 404
+
     with mock.patch.object(
-        default_gh_client, "create_release"
+        default_gh_client, "create_release", side_effect=not_found
     ) as mock_create_release, mock.patch.object(
-        default_gh_client, "get_release_id_by_tag"
+        default_gh_client, "get_release_id_by_tag", return_value=None
     ) as mock_get_release_id_by_tag, mock.patch.object(
-        default_gh_client, "edit_release_notes"
+        default_gh_client, "edit_release_notes", return_value=None
     ) as mock_edit_release_notes:
-        mock_create_release.side_effect = not_found
-        mock_get_release_id_by_tag.return_value = None
-        mock_edit_release_notes.return_value = None
-
+        # Execute in mock environment expecting an exception to be raised
         with pytest.raises(ValueError):
             default_gh_client.create_or_update_release(tag, RELEASE_NOTES, prerelease)
 
+        mock_create_release.assert_called_once()
         mock_get_release_id_by_tag.assert_called_once_with(tag)
         mock_edit_release_notes.assert_not_called()
 
 
-def test_asset_upload_url(default_gh_client):
+def test_asset_upload_url(default_gh_client: Github):
     release_id = 1
+    expected_num_requests = 1
+    expected_http_method = "GET"
+    expected_asset_upload_request_url = (
+        "{api_url}/repos/{owner}/{repo}/releases/{release_id}".format(
+            api_url=default_gh_client.api_url,
+            owner=default_gh_client.owner,
+            repo=default_gh_client.repo_name,
+            release_id=release_id,
+        )
+    )
+    mocked_upload_url = (
+        "{upload_domain}/repos/{owner}/{repo}/releases/{release_id}/assets".format(
+            upload_domain=github_upload_url,
+            owner=default_gh_client.owner,
+            repo=default_gh_client.repo_name,
+            release_id=release_id,
+        )
+    )
     # '{?name,label}' are added by github.com at least, maybe custom too
     # https://docs.github.com/en/rest/releases/releases?apiVersion=2022-11-28#get-a-release
     resp_payload = {
-        "upload_url": (
-            f"{default_gh_client.upload_url}/repos/"
-            f"{default_gh_client.owner}/{default_gh_client.repo_name}/"
-            f"releases/{release_id}/"
-            "assets{?name,label}"
-        ),
+        "upload_url": mocked_upload_url + "{?name,label}",
         "status": "success",
     }
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the response
         m.register_uri("GET", github_api_matcher, json=resp_payload, status_code=200)
-        assert (
-            default_gh_client.asset_upload_url(release_id)
-            == "https://{domain}/repos/{owner}/{repo}/releases/{release_id}/assets".format(
-                domain=default_gh_client.DEFAULT_UPLOAD_DOMAIN,
-                owner=default_gh_client.owner,
-                repo=default_gh_client.repo_name,
-                release_id=release_id,
-            )
-        )
+
+        # Execute method under test
+        result = default_gh_client.asset_upload_url(release_id)
+
+        # Evaluate (expected -> actual)
+        assert mocked_upload_url == result
         assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "GET"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-                release_id=1,
-            )
-        )
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_asset_upload_request_url == m.last_request.url
 
 
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
+@pytest.mark.usefixtures(init_example_project.__name__)
 def test_upload_asset_succeeds(
-    init_example_project: None,
     default_gh_client: Github,
     example_changelog_md: Path,
     status_code: int,
     mock_release_id: int,
 ):
+    # Setup
     label = "abc123"
     urlparams = {"name": example_changelog_md.name, "label": label}
-    expected_upload_url = (
-        f"{default_gh_client.upload_url}/repos/{default_gh_client.owner}/"
-        f"{default_gh_client.repo_name}/releases/{mock_release_id}/"
-        r"assets{?name,label}"
+    release_upload_url = (
+        "{upload_domain}/repos/{owner}/{repo}/releases/{release_id}/assets".format(
+            upload_domain=github_upload_url,
+            owner=default_gh_client.owner,
+            repo=default_gh_client.repo_name,
+            release_id=mock_release_id,
+        )
     )
-    json_get_up_url = {"status": "ok", "upload_url": expected_upload_url}
+    expected_num_requests = 2
+    expected_retrieve_upload_url_method = "GET"
+    expected_upload_http_method = "POST"
+    expected_upload_url = "{url}?{params}".format(
+        url=release_upload_url,
+        params=urlencode(urlparams),
+    )
+    expected_changelog = example_changelog_md.read_bytes()
+    json_get_up_url = {
+        "status": "ok",
+        "upload_url": release_upload_url + "{?name,label}",
+    }
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the responses
         m.register_uri(
             "POST",
             github_upload_matcher,
             json={"status": "ok"},
             status_code=status_code,
         )
         m.register_uri(
             "GET", github_api_matcher, json=json_get_up_url, status_code=status_code
         )
-        assert (
-            default_gh_client.upload_asset(
-                release_id=mock_release_id,
-                file=example_changelog_md.resolve(),
-                label=label,
-            )
-            is True
+
+        # Execute method under test
+        result = default_gh_client.upload_asset(
+            release_id=mock_release_id,
+            file=example_changelog_md.resolve(),
+            label=label,
         )
+
+        # Evaluate (expected -> actual)
+        assert result is True
         assert m.called
-        assert len(m.request_history) == 2
+        assert expected_num_requests == len(m.request_history)
+
         get_req, post_req = m.request_history
-        assert isinstance(get_req, requests_mock.request._RequestObjectProxy)
-        assert isinstance(post_req, requests_mock.request._RequestObjectProxy)
-        assert get_req.method == "GET"
-
-        assert post_req.method == "POST"
-        assert post_req.url == "{url}?{params}".format(
-            url=expected_upload_url.replace(r"{?name,label}", ""),
-            params=urlencode(urlparams),
-        )
-        # Check if content-type header was correctly set according to
-        # mimetypes - not retesting guessing functionality
-        assert {
-            "Content-Type": mimetypes.guess_type(
-                example_changelog_md.resolve(), strict=False
-            )[0]
-            or "application/octet-stream"
-        }.items() <= post_req.headers.items()
-        assert post_req.body == example_changelog_md.read_bytes()
+
+        assert expected_retrieve_upload_url_method == get_req.method
+        assert expected_upload_http_method == post_req.method
+        assert expected_upload_url == post_req.url
+        assert expected_changelog == post_req.body
 
 
 @pytest.mark.parametrize("status_code", (400, 404, 429, 500, 503))
 @pytest.mark.parametrize("mock_release_id", range(3))
+@pytest.mark.usefixtures(init_example_project.__name__)
 def test_upload_asset_fails(
-    init_example_project: None,
     default_gh_client: Github,
     example_changelog_md: Path,
     status_code: int,
     mock_release_id: int,
 ):
+    # Setup
     label = "abc123"
     urlparams = {"name": example_changelog_md.name, "label": label}
+    upload_url = "{up_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
+        up_url=github_upload_url,
+        owner=default_gh_client.owner,
+        repo_name=default_gh_client.repo_name,
+        release_id=mock_release_id,
+    )
     json_get_up_url = {
         "status": "ok",
-        "upload_url": "{up_url}/repos/{owner}/{repo_name}/releases/{release_id}".format(
-            up_url=default_gh_client.upload_url,
-            owner=default_gh_client.owner,
-            repo_name=default_gh_client.repo_name,
-            release_id=mock_release_id,
-        ),
+        "upload_url": upload_url,
     }
+    changelog_data_mime_type = (
+        mimetypes.guess_type(example_changelog_md.resolve(), strict=False)[0]
+        or "application/octet-stream"
+    )
+    expected_num_requests = 2
+    expected_http_method = "POST"
+    expected_upload_request_url = "{url}?{params}".format(
+        url=upload_url,
+        params=urlencode(urlparams),
+    )
+    expected_upload_request_headers = {"Content-Type": changelog_data_mime_type}.items()
+    expected_changelog = example_changelog_md.read_bytes()
+
     with requests_mock.Mocker(session=default_gh_client.session) as m:
+        # mock the responses
         m.register_uri(
             "POST",
             github_upload_matcher,
             json={"message": "error"},
             status_code=status_code,
         )
         m.register_uri("GET", github_api_matcher, json=json_get_up_url, status_code=200)
+
+        # Execute method under test expecting an exception to be raised
         with pytest.raises(HTTPError):
             default_gh_client.upload_asset(
                 release_id=mock_release_id,
                 file=example_changelog_md.resolve(),
                 label=label,
             )
 
+        # Evaluate (expected -> actual)
         assert m.called
-        assert len(m.request_history) == 2
-        post_req = m.last_request.copy()
-        assert post_req.method == "POST"
-        assert post_req.url == "{url}?{params}".format(
-            url=default_gh_client.asset_upload_url(mock_release_id),
-            params=urlencode(urlparams),
-        )
-
-        # Check if content-type header was correctly set according to
-        # mimetypes - not retesting guessing functionality
-        assert {
-            "Content-Type": mimetypes.guess_type(
-                example_changelog_md.resolve(), strict=False
-            )[0]
-            or "application/octet-stream"
-        }.items() <= post_req.headers.items()
-        assert post_req.body == example_changelog_md.read_bytes()
+        assert expected_num_requests == len(m.request_history)
+        assert expected_http_method == m.last_request.method
+        assert expected_upload_request_url == m.last_request.url
+        assert expected_upload_request_headers <= m.last_request.headers.items()
+        assert expected_changelog == m.last_request.body
 
 
 # Note - mocking as the logic for uploading an asset
 # is covered by testing above, no point re-testing.
 def test_upload_dists_when_release_id_not_found(default_gh_client):
     tag = "v1.0.0"
     path = "doesn't matter"
+    expected_num_uploads = 0
+
+    # Set up mock environment
     with mock.patch.object(
-        default_gh_client, "get_release_id_by_tag"
+        default_gh_client,
+        "get_release_id_by_tag",
+        return_value=None,
     ) as mock_get_release_id_by_tag, mock.patch.object(
         default_gh_client, "upload_asset"
     ) as mock_upload_asset:
-        mock_get_release_id_by_tag.return_value = None
-        assert not default_gh_client.upload_dists(tag, path)
+        # Execute method under test
+        result = default_gh_client.upload_dists(tag, path)
+
+        # Evaluate
+        assert expected_num_uploads == result
         mock_get_release_id_by_tag.assert_called_once_with(tag=tag)
         mock_upload_asset.assert_not_called()
 
 
 @pytest.mark.parametrize(
-    "files, glob_pattern, upload_statuses, expected",
+    "files, glob_pattern, upload_statuses, expected_num_uploads",
     [
         (["foo.zip", "bar.whl"], "*.zip", [True], 1),
         (["foo.whl", "foo.egg", "foo.tar.gz"], "foo.*", [True, True, True], 3),
         # What if not built?
         ([], "*", [], 0),
         # What if wrong directory/other stuff in output dir/subfolder?
         (["specialconfig.yaml", "something.whl", "desc.md"], "*.yaml", [True], 1),
         (["specialconfig.yaml", "something.whl", "desc.md"], "*.md", [True], 1),
     ],
 )
 def test_upload_dists_when_release_id_found(
-    default_gh_client, files, glob_pattern, upload_statuses, expected
+    default_gh_client: Github,
+    files: list[str],
+    glob_pattern: str,
+    upload_statuses: list[bool],
+    expected_num_uploads: int,
 ):
     release_id = 420
     tag = "doesn't matter"
-    with mock.patch.object(
-        default_gh_client, "get_release_id_by_tag"
+    matching_files = fnmatch.filter(files, glob_pattern)
+    expected_files_uploaded = [mock.call(release_id, fn) for fn in matching_files]
+
+    # Skip check as the files don't exist in filesystem
+    mocked_isfile = mock.patch.object(os.path, "isfile", return_value=True)
+    mocked_globber = mock.patch.object(glob, "glob", return_value=matching_files)
+
+    # Set up mock environment
+    with mocked_globber, mocked_isfile, mock.patch.object(
+        default_gh_client,
+        "get_release_id_by_tag",
+        return_value=release_id,
     ) as mock_get_release_id_by_tag, mock.patch.object(
-        default_gh_client, "upload_asset"
-    ) as mock_upload_asset, mock.patch.object(
-        glob, "glob"
-    ) as mock_glob_glob, mock.patch.object(os.path, "isfile") as mock_os_path_isfile:
-        # Skip check as the filenames deliberately don't exists for testing
-        mock_os_path_isfile.return_value = True
-
-        matching_files = glob.fnmatch.filter(files, glob_pattern)
-        mock_glob_glob.return_value = matching_files
-        mock_get_release_id_by_tag.return_value = release_id
+        default_gh_client,
+        "upload_asset",
+        side_effect=upload_statuses,
+    ) as mock_upload_asset:
+        # Execute method under test
+        num_uploads = default_gh_client.upload_dists(tag, glob_pattern)
 
-        mock_upload_asset.side_effect = upload_statuses
-        assert default_gh_client.upload_dists(tag, glob_pattern) == expected
+        # Evaluate (expected -> actual)
+        assert expected_num_uploads == num_uploads
         mock_get_release_id_by_tag.assert_called_once_with(tag=tag)
-        assert [
-            mock.call(release_id, fn) for fn in matching_files
-        ] == mock_upload_asset.call_args_list
+        assert expected_files_uploaded == mock_upload_asset.call_args_list
```

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+from __future__ import annotations
+
 import os
 from contextlib import contextmanager
+from typing import TYPE_CHECKING
 from unittest import mock
 
 import gitlab
 import pytest
-from requests import Session
 
 from semantic_release.hvcs.gitlab import Gitlab
 
-from tests.const import EXAMPLE_REPO_NAME, EXAMPLE_REPO_OWNER, RELEASE_NOTES
+from tests.const import (
+    EXAMPLE_HVCS_DOMAIN,
+    EXAMPLE_REPO_NAME,
+    EXAMPLE_REPO_OWNER,
+    RELEASE_NOTES,
+)
+
+if TYPE_CHECKING:
+    from typing import Generator
 
 gitlab.Gitlab("")  # instantiation necessary to discover gitlab ProjectManager
 
 # Note: there's nothing special about the value of these variables,
 # they're just constants for easier consistency with the faked objects
 A_GOOD_TAG = "v1.2.3"
 A_BAD_TAG = "v2.1.1-rc.1"
@@ -139,271 +149,318 @@
             f"{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}": _GitlabProject(status)
         },
     ):
         yield
 
 
 @pytest.fixture
-def default_gl_client():
-    remote_url = f"git@gitlab.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
-    return Gitlab(remote_url=remote_url)
+def default_gl_client() -> Generator[Gitlab, None, None]:
+    remote_url = (
+        f"git@{Gitlab.DEFAULT_DOMAIN}:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git"
+    )
+    with mock.patch.dict(os.environ, {}, clear=True):
+        yield Gitlab(remote_url=remote_url)
 
 
 @pytest.mark.parametrize(
-    (
-        "patched_os_environ, hvcs_domain, hvcs_api_domain, "
-        "expected_hvcs_domain, expected_hvcs_api_domain"
-    ),
+    "patched_os_environ, hvcs_domain, expected_hvcs_domain, insecure",
+    # NOTE: GitLab does not have a different api domain
     [
-        ({}, None, None, Gitlab.DEFAULT_DOMAIN, Gitlab.DEFAULT_DOMAIN),
+        # Default values
+        ({}, None, f"https://{Gitlab.DEFAULT_DOMAIN}", False),
         (
-            {"CI_SERVER_URL": "https://special.custom.server/vcs/"},
-            None,
+            # Gather domain from environment
+            {"CI_SERVER_URL": "https://special.custom.server/"},
             None,
-            "special.custom.server/vcs",
-            "special.custom.server/vcs",
+            "https://special.custom.server",
+            False,
         ),
         (
-            {"CI_SERVER_HOST": "api.special.custom.server/"},
-            None,
+            # Custom domain with path prefix (derives from environment)
+            {"CI_SERVER_URL": "https://special.custom.server/vcs/"},
             None,
-            "api.special.custom.server/",
-            "api.special.custom.server/",
+            "https://special.custom.server/vcs",
+            False,
         ),
         (
-            {"CI_SERVER_URL": "https://special.custom.server/vcs/"},
-            "example.com",
-            None,
-            "example.com",
-            "example.com",
+            # Ignore environment & use provided parameter value (ie from user config)
+            {
+                "CI_SERVER_URL": "https://special.custom.server/",
+                "CI_API_V4_URL": "https://special.custom.server/api/v3",
+            },
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            f"https://{EXAMPLE_HVCS_DOMAIN}",
+            False,
         ),
         (
-            {"CI_SERVER_URL": "https://api.special.custom.server/"},
-            None,
-            "api.example.com",
-            "api.special.custom.server",
-            "api.example.com",
+            # Allow insecure http connections explicitly
+            {},
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            True,
+        ),
+        (
+            # Infer insecure connection from user configuration
+            {},
+            EXAMPLE_HVCS_DOMAIN,
+            f"http://{EXAMPLE_HVCS_DOMAIN}",
+            True,
         ),
     ],
 )
 @pytest.mark.parametrize(
     "remote_url",
     [
-        f"git@gitlab.com:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
-        f"https://gitlab.com/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
+        f"git@{Gitlab.DEFAULT_DOMAIN}:{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
+        f"https://{Gitlab.DEFAULT_DOMAIN}/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
     ],
 )
 @pytest.mark.parametrize("token", ("abc123", None))
 def test_gitlab_client_init(
-    patched_os_environ,
-    hvcs_domain,
-    hvcs_api_domain,
-    expected_hvcs_domain,
-    expected_hvcs_api_domain,
-    remote_url,
-    token,
+    patched_os_environ: dict[str, str],
+    hvcs_domain: str | None,
+    expected_hvcs_domain: str,
+    remote_url: str,
+    token: str | None,
+    insecure: bool,
 ):
     with mock.patch.dict(os.environ, patched_os_environ, clear=True):
         client = Gitlab(
             remote_url=remote_url,
             hvcs_domain=hvcs_domain,
-            hvcs_api_domain=hvcs_api_domain,
             token=token,
+            allow_insecure=insecure,
         )
 
-        assert client.hvcs_domain == expected_hvcs_domain
-        assert client.hvcs_api_domain == expected_hvcs_api_domain
-        assert client.api_url == patched_os_environ.get(
-            "CI_SERVER_URL", f"https://{client.hvcs_api_domain}"
+        # Evaluate (expected -> actual)
+        assert expected_hvcs_domain == client.hvcs_domain.url
+        assert token == client.token
+        assert remote_url == client._remote_url
+
+
+@pytest.mark.parametrize(
+    "hvcs_domain, insecure",
+    [
+        (f"ftp://{EXAMPLE_HVCS_DOMAIN}", False),
+        (f"ftp://{EXAMPLE_HVCS_DOMAIN}", True),
+        (f"http://{EXAMPLE_HVCS_DOMAIN}", False),
+    ],
+)
+def test_gitlab_client_init_with_invalid_scheme(
+    hvcs_domain: str,
+    insecure: bool,
+):
+    with pytest.raises(ValueError), mock.patch.dict(os.environ, {}, clear=True):
+        Gitlab(
+            remote_url=f"https://{EXAMPLE_HVCS_DOMAIN}/{EXAMPLE_REPO_OWNER}/{EXAMPLE_REPO_NAME}.git",
+            hvcs_domain=hvcs_domain,
+            allow_insecure=insecure,
         )
-        assert client.token == token
-        assert client._remote_url == remote_url
-        assert hasattr(client, "session")
-        assert isinstance(getattr(client, "session", None), Session)
 
 
 @pytest.mark.parametrize(
     "patched_os_environ, expected_owner, expected_name",
     [
         ({}, None, None),
         (
             {"CI_PROJECT_NAMESPACE": "path/to/repo", "CI_PROJECT_NAME": "foo"},
             "path/to/repo",
             "foo",
         ),
     ],
 )
 def test_gitlab_get_repository_owner_and_name(
-    default_gl_client, patched_os_environ, expected_owner, expected_name
+    default_gl_client: Gitlab,
+    patched_os_environ: dict[str, str],
+    expected_owner: str | None,
+    expected_name: str | None,
 ):
+    # expected results should be a tuple[namespace, repo_name] and if both are None,
+    # then the default value from GitLab class should be used
+    expected_result = (expected_owner, expected_name)
+    if expected_owner is None and expected_name is None:
+        expected_result = super(
+            Gitlab, default_gl_client
+        )._get_repository_owner_and_name()
+
     with mock.patch.dict(os.environ, patched_os_environ, clear=True):
-        if expected_owner is None and expected_name is None:
-            assert (
-                default_gl_client._get_repository_owner_and_name()
-                == super(Gitlab, default_gl_client)._get_repository_owner_and_name()
-            )
-        else:
-            assert default_gl_client._get_repository_owner_and_name() == (
-                expected_owner,
-                expected_name,
-            )
+        # Execute in mocked environment
+        result = default_gl_client._get_repository_owner_and_name()
+
+        # Evaluate (expected -> actual)
+        assert expected_result == result
 
 
 @pytest.mark.parametrize(
-    "use_token, token, _remote_url, expected",
+    "use_token, token, remote_url, expected_auth_url",
     [
         (
             False,
             "",
-            "git@gitlab.com:custom/example.git",
-            "git@gitlab.com:custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             True,
             "",
-            "git@gitlab.com:custom/example.git",
-            "git@gitlab.com:custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             False,
             "aabbcc",
-            "git@gitlab.com:custom/example.git",
-            "git@gitlab.com:custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
         ),
         (
             True,
             "aabbcc",
-            "git@gitlab.com:custom/example.git",
-            "https://gitlab-ci-token:aabbcc@gitlab.com/custom/example.git",
+            f"git@{Gitlab.DEFAULT_DOMAIN}:custom/example.git",
+            f"https://gitlab-ci-token:aabbcc@{Gitlab.DEFAULT_DOMAIN}/custom/example.git",
         ),
     ],
 )
 def test_remote_url(
-    default_gl_client,
-    use_token,
-    token,
-    # TODO: linter thinks this is a fixture not a param - why?
-    _remote_url,  # noqa: PT019
-    expected,
+    default_gl_client: Gitlab,
+    use_token: bool,
+    token: str,
+    remote_url: str,
+    expected_auth_url: str,
 ):
-    default_gl_client._remote_url = _remote_url
+    default_gl_client._remote_url = remote_url
     default_gl_client.token = token
-    assert default_gl_client.remote_url(use_token=use_token) == expected
+    assert expected_auth_url == default_gl_client.remote_url(use_token=use_token)
 
 
-def test_compare_url(default_gl_client):
-    assert default_gl_client.compare_url(
-        from_rev="revA", to_rev="revB"
-    ) == "https://{domain}/{owner}/{repo}/-/compare/revA...revB".format(
-        domain=default_gl_client.hvcs_domain,
+def test_compare_url(default_gl_client: Gitlab):
+    start_rev = "revA"
+    end_rev = "revB"
+    expected_url = "{server}/{owner}/{repo}/-/compare/{from_rev}...{to_rev}".format(
+        server=default_gl_client.hvcs_domain.url,
         owner=default_gl_client.owner,
         repo=default_gl_client.repo_name,
+        from_rev=start_rev,
+        to_rev=end_rev,
     )
+    actual_url = default_gl_client.compare_url(from_rev=start_rev, to_rev=end_rev)
+    assert expected_url == actual_url
 
 
-def test_commit_hash_url(default_gl_client):
-    assert default_gl_client.commit_hash_url(
-        REF
-    ) == "https://{domain}/{owner}/{repo}/-/commit/{sha}".format(
-        domain=default_gl_client.hvcs_domain,
+def test_commit_hash_url(default_gl_client: Gitlab):
+    expected_url = "{server}/{owner}/{repo}/-/commit/{sha}".format(
+        server=default_gl_client.hvcs_domain.url,
         owner=default_gl_client.owner,
         repo=default_gl_client.repo_name,
         sha=REF,
     )
+    assert expected_url == default_gl_client.commit_hash_url(REF)
+
+
+@pytest.mark.parametrize("issue_number", (420, "420"))
+def test_issue_url(default_gl_client: Gitlab, issue_number: int | str):
+    expected_url = "{server}/{owner}/{repo}/-/issues/{issue_num}".format(
+        server=default_gl_client.hvcs_domain.url,
+        owner=default_gl_client.owner,
+        repo=default_gl_client.repo_name,
+        issue_num=issue_number,
+    )
+    actual_url = default_gl_client.issue_url(issue_number=issue_number)
+    assert expected_url == actual_url
 
 
 @pytest.mark.parametrize("pr_number", (420, "420"))
-def test_pull_request_url(default_gl_client, pr_number):
-    assert default_gl_client.pull_request_url(
-        pr_number=pr_number
-    ) == "https://{domain}/{owner}/{repo}/-/issues/{pr_number}".format(
-        domain=default_gl_client.hvcs_domain,
+def test_pull_request_url(default_gl_client: Gitlab, pr_number: int | str):
+    expected_url = "{server}/{owner}/{repo}/-/merge_requests/{pr_number}".format(
+        server=default_gl_client.hvcs_domain.url,
         owner=default_gl_client.owner,
         repo=default_gl_client.repo_name,
         pr_number=pr_number,
     )
+    actual_url = default_gl_client.pull_request_url(pr_number=pr_number)
+    assert expected_url == actual_url
 
 
 @pytest.mark.parametrize("tag", (A_GOOD_TAG, A_LOCKED_TAG))
-def test_create_release_succeeds(default_gl_client, tag):
+def test_create_release_succeeds(default_gl_client: Gitlab, tag):
     with mock_gitlab():
-        assert default_gl_client.create_release(tag, RELEASE_NOTES) == tag
+        assert tag == default_gl_client.create_release(tag, RELEASE_NOTES)
 
 
-def test_create_release_fails_with_bad_tag(default_gl_client):
+def test_create_release_fails_with_bad_tag(default_gl_client: Gitlab):
     with mock_gitlab(), pytest.raises(gitlab.GitlabCreateError):
         default_gl_client.create_release(A_BAD_TAG, RELEASE_NOTES)
 
 
 @pytest.mark.parametrize("tag", (A_GOOD_TAG, A_LOCKED_TAG))
-def test_update_release_succeeds(default_gl_client, tag):
+def test_update_release_succeeds(default_gl_client: Gitlab, tag: str):
     with mock_gitlab():
-        assert default_gl_client.edit_release_notes(tag, RELEASE_NOTES) == tag
+        assert tag == default_gl_client.edit_release_notes(tag, RELEASE_NOTES)
 
 
-def test_update_release_fails_with_missing_tag(default_gl_client):
+def test_update_release_fails_with_missing_tag(default_gl_client: Gitlab):
     with mock_gitlab(), pytest.raises(gitlab.GitlabUpdateError):
         default_gl_client.edit_release_notes(A_MISSING_TAG, RELEASE_NOTES)
 
 
 @pytest.mark.parametrize("prerelease", (True, False))
-def test_create_or_update_release_when_create_succeeds(default_gl_client, prerelease):
+def test_create_or_update_release_when_create_succeeds(
+    default_gl_client: Gitlab, prerelease: bool
+):
     with mock.patch.object(
-        default_gl_client, "create_release"
+        default_gl_client, "create_release", return_value=A_GOOD_TAG
     ) as mock_create_release, mock.patch.object(
-        default_gl_client, "edit_release_notes"
+        default_gl_client, "edit_release_notes", return_value=A_GOOD_TAG
     ) as mock_edit_release_notes:
-        mock_create_release.return_value = A_GOOD_TAG
-        mock_edit_release_notes.return_value = A_GOOD_TAG
-        assert (
-            default_gl_client.create_or_update_release(
-                A_GOOD_TAG, RELEASE_NOTES, prerelease
-            )
-            == A_GOOD_TAG
+        # Execute in mock environment
+        result = default_gl_client.create_or_update_release(
+            A_GOOD_TAG, RELEASE_NOTES, prerelease
         )
+
+        # Evaluate (expected -> actual)
+        assert A_GOOD_TAG == result  # noqa: SIM300
         mock_create_release.assert_called_once_with(
             tag=A_GOOD_TAG, release_notes=RELEASE_NOTES, prerelease=prerelease
         )
         mock_edit_release_notes.assert_not_called()
 
 
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_update_succeeds(
-    default_gl_client, prerelease
+    default_gl_client: Gitlab, prerelease: bool
 ):
     bad_request = gitlab.GitlabCreateError("400 Bad Request")
     with mock.patch.object(
-        default_gl_client, "create_release"
-    ) as mock_create_release, mock.patch.object(
-        default_gl_client, "edit_release_notes"
+        default_gl_client, "create_release", side_effect=bad_request
+    ), mock.patch.object(
+        default_gl_client, "edit_release_notes", return_value=A_GOOD_TAG
     ) as mock_edit_release_notes:
-        mock_create_release.side_effect = bad_request
-        mock_edit_release_notes.return_value = A_GOOD_TAG
-        assert (
-            default_gl_client.create_or_update_release(
-                A_GOOD_TAG, RELEASE_NOTES, prerelease
-            )
-            == A_GOOD_TAG
+        # Execute in mock environment
+        result = default_gl_client.create_or_update_release(
+            A_GOOD_TAG, RELEASE_NOTES, prerelease
         )
+
+        # Evaluate (expected -> actual)
+        assert A_GOOD_TAG == result  # noqa: SIM300
         mock_edit_release_notes.assert_called_once_with(
             release_id=A_GOOD_TAG, release_notes=RELEASE_NOTES
         )
 
 
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_or_update_release_when_create_fails_and_update_fails(
-    default_gl_client, prerelease
+    default_gl_client: Gitlab, prerelease: bool
 ):
     bad_request = gitlab.GitlabCreateError("400 Bad Request")
     not_found = gitlab.GitlabUpdateError("404 Not Found")
-    with mock.patch.object(
-        default_gl_client, "create_release"
-    ) as mock_create_release, mock.patch.object(
-        default_gl_client, "edit_release_notes"
-    ) as mock_edit_release_notes:
-        mock_create_release.side_effect = bad_request
-        mock_edit_release_notes.side_effect = not_found
+    create_release_patch = mock.patch.object(
+        default_gl_client, "create_release", side_effect=bad_request
+    )
+    edit_release_notes_patch = mock.patch.object(
+        default_gl_client, "edit_release_notes", side_effect=not_found
+    )
 
+    # Execute in mocked environment expecting a GitlabUpdateError to be raised
+    with create_release_patch, edit_release_notes_patch:
         with pytest.raises(gitlab.GitlabUpdateError):
             default_gl_client.create_or_update_release(
                 A_GOOD_TAG, RELEASE_NOTES, prerelease
             )
```

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/test_helpers.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_algorithm.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_declaration.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_translator.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_version.py` & `python_semantic_release-9.4.2/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.1/tests/util.py` & `python_semantic_release-9.4.2/tests/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 import secrets
 import shutil
 import stat
 import string
 from contextlib import contextmanager, suppress
-from tempfile import NamedTemporaryFile
 from typing import TYPE_CHECKING, Tuple
 
 from pydantic.dataclasses import dataclass
 
 from semantic_release.changelog.context import make_changelog_context
 from semantic_release.changelog.release_history import ReleaseHistory
 from semantic_release.cli import config as cliConfigModule
@@ -86,29 +85,14 @@
     with open(f"{repo.working_tree_dir}/{filename}", "a+") as f:
         f.write(text or f"default text {shortuid(12)}")
         f.write("\n")
 
     repo.index.add(filename)
 
 
-@contextmanager
-def netrc_file(machine: str) -> NamedTemporaryFile:
-    with NamedTemporaryFile("w") as netrc:
-        # Add these attributes to use in tests as source of truth
-        netrc.login_username = "username"
-        netrc.login_password = "password"
-
-        netrc.write(f"machine {machine}" + "\n")
-        netrc.write(f"login {netrc.login_username}" + "\n")
-        netrc.write(f"password {netrc.login_password}" + "\n")
-        netrc.flush()
-
-        yield netrc
-
-
 def flatten_dircmp(dcmp: filecmp.dircmp) -> list[str]:
     return (
         dcmp.diff_files
         + dcmp.left_only
         + dcmp.right_only
         + [
             os.sep.join((directory, file))
```

