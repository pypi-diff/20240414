# Comparing `tmp/pertpy-0.6.0.tar.gz` & `tmp/pertpy-0.7.0.tar.gz`

## Comparing `pertpy-0.6.0.tar` & `pertpy-0.7.0.tar`

### file list

```diff
@@ -1,126 +1,158 @@
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pertpy-0.6.0/.editorconfig
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pertpy-0.6.0/.gitattributes
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pertpy-0.6.0/.gitmodules
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 pertpy-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pertpy-0.6.0/.prettierignore
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pertpy-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 pertpy-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pertpy-0.6.0/codecov.yml
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/labels.yml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/pull_request_template.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/release-drafter.yml
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/workflows/labeler.yml
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/workflows/release_drafter.yml
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 pertpy-0.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/Makefile
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/authors.md
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/code_of_conduct.md
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/conf.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/contributing.md
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/index.md
--rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/installation.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/make.bat
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/utils.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_ext/edit_on_github.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_ext/typed_returns.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/SCVI_LICENSE
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/placeholder.png
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/css/overwrite.css
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/css/sphinx_gallery.css
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/icons/code-24px.svg
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/icons/computer-24px.svg
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/icons/library_books-24px.svg
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/icons/play_circle_outline-24px.svg
--rw-r--r--   0        0        0    22782 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/augur.png
--rw-r--r--   0        0        0    28114 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/dialogue.png
--rw-r--r--   0        0        0    82238 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/distances.png
--rw-r--r--   0        0        0    88998 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/distances_tests.png
--rw-r--r--   0        0        0    52088 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/guide_rna_assignment.png
--rw-r--r--   0        0        0    25340 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/milo.png
--rw-r--r--   0        0        0  2687817 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/mixscape.png
--rw-r--r--   0        0        0    33037 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/ontology.png
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/placeholder.png
--rw-r--r--   0        0        0    50106 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/sccoda.png
--rw-r--r--   0        0        0    39935 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/sccoda_extended.png
--rw-r--r--   0        0        0    83788 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/scgen_batch_removal.png
--rw-r--r--   0        0        0    83788 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/scgen_perturbation_prediction.png
--rw-r--r--   0        0        0    41952 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_static/tutorials/tasccoda.png
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_templates/class_no_inherited.rst
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/tutorials/index.md
--rw-r--r--   0        0        0    15700 2020-02-02 00:00:00.000000 pertpy-0.6.0/docs/usage/usage.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/py.typed
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/data/__init__.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/data/_dataloader.py
--rw-r--r--   0        0        0    59496 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/data/_datasets.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/__init__.py
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_augur.py
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_cinemaot.py
--rw-r--r--   0        0        0    43650 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_coda.py
--rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_dialogue.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_guide_rna.py
--rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_milopy.py
--rw-r--r--   0        0        0    27903 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_mixscape.py
--rw-r--r--   0        0        0    15125 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/plot/_scgen.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/preprocessing/__init__.py
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/preprocessing/_guide_rna.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/__init__.py
--rw-r--r--   0        0        0    45193 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_augur.py
--rw-r--r--   0        0        0    33374 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_cinemaot.py
--rw-r--r--   0        0        0    48116 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_dialogue.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_differential_gene_expression.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_kernel_pca.py
--rw-r--r--   0        0        0    30737 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_milo.py
--rw-r--r--   0        0        0    23559 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_mixscape.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/transferlearning_MMD_LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_coda/__init__.py
--rw-r--r--   0        0        0    66859 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_coda/_base_coda.py
--rw-r--r--   0        0        0    21616 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_coda/_sccoda.py
--rw-r--r--   0        0        0    30721 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_coda/_tasccoda.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_distances/__init__.py
--rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_distances/_distance_tests.py
--rw-r--r--   0        0        0    29780 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_distances/_distances.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_metadata/__init__.py
--rw-r--r--   0        0        0    33830 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_metadata/_cell_line.py
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_metadata/_look_up.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_perturbation_space/__init__.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_perturbation_space/_clustering.py
--rw-r--r--   0        0        0    13861 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_perturbation_space/_discriminator_classifier.py
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_perturbation_space/_metrics.py
--rw-r--r--   0        0        0    14169 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_perturbation_space/_perturbation_space.py
--rw-r--r--   0        0        0    10367 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_perturbation_space/_simple.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_scgen/__init__.py
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_scgen/_base_components.py
--rw-r--r--   0        0        0    15368 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_scgen/_jax_scgen.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_scgen/_jax_scgenvae.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 pertpy-0.6.0/pertpy/tools/_scgen/_utils.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/preprocessing/test_grna_assignment.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/haber_data.csv
--rw-r--r--   0        0        0   476779 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/r_result.csv
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/test_augur.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/test_cinemaot.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/test_jax_scgen.py
--rw-r--r--   0        0        0    11434 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/test_milo.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/test_mixscape.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_coda/test_sccoda.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_coda/test_tasccoda.py
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_distances/test_distance_tests.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_distances/test_distances.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_metadata/test_cell_line.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_perturbation_space/test_discriminator_classifier.py
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_perturbation_space/test_simple_cluster_space.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 pertpy-0.6.0/tests/tools/_perturbation_space/test_simple_perturbation_space.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pertpy-0.6.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pertpy-0.6.0/LICENSE
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 pertpy-0.6.0/README.md
--rw-r--r--   0        0        0     4577 2020-02-02 00:00:00.000000 pertpy-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 pertpy-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pertpy-0.7.0/.editorconfig
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pertpy-0.7.0/.gitattributes
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pertpy-0.7.0/.gitmodules
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pertpy-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pertpy-0.7.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 pertpy-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pertpy-0.7.0/codecov.yml
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/labels.yml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/workflows/labeler.yml
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/workflows/release_drafter.yml
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pertpy-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/Makefile
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/code_of_conduct.md
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/conf.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/contributing.md
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/index.md
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/installation.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/make.bat
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/utils.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_ext/edit_on_github.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_ext/typed_returns.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/SCVI_LICENSE
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/placeholder.png
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/css/overwrite.css
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/css/sphinx_gallery.css
+-rw-r--r--   0        0        0    36668 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/augur_dp_scatter.png
+-rw-r--r--   0        0        0    27935 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/augur_important_features.png
+-rw-r--r--   0        0        0    13426 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/augur_lollipop.png
+-rw-r--r--   0        0        0    28058 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/augur_scatterplot.png
+-rw-r--r--   0        0        0    73412 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/dialogue_pairplot.png
+-rw-r--r--   0        0        0    42224 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/dialogue_violin.png
+-rw-r--r--   0        0        0    69787 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/enrichment_dotplot.png
+-rw-r--r--   0        0        0    34796 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/enrichment_gsea.png
+-rw-r--r--   0        0        0    60973 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/milo_da_beeswarm.png
+-rw-r--r--   0        0        0    97338 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/milo_nhood.png
+-rw-r--r--   0        0        0    82093 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/milo_nhood_graph.png
+-rw-r--r--   0        0        0    70863 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/mixscape_barplot.png
+-rw-r--r--   0        0        0    69099 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/mixscape_heatmap.png
+-rw-r--r--   0        0        0   136335 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/mixscape_lda.png
+-rw-r--r--   0        0        0    76909 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/mixscape_perturbscore.png
+-rw-r--r--   0        0        0    30951 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/mixscape_violin.png
+-rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/sccoda_boxplots.png
+-rw-r--r--   0        0        0    22896 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/sccoda_effects_barplot.png
+-rw-r--r--   0        0        0    23960 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/sccoda_rel_abundance_dispersion_plot.png
+-rw-r--r--   0        0        0    24450 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/sccoda_stacked_barplot.png
+-rw-r--r--   0        0        0    33174 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/scgen_reg_mean.png
+-rw-r--r--   0        0        0    56666 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/tasccoda_draw_effects.png
+-rw-r--r--   0        0        0   104791 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/tasccoda_draw_tree.png
+-rw-r--r--   0        0        0   479226 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/docstring_previews/tasccoda_effects_umap.png
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/icons/code-24px.svg
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/icons/computer-24px.svg
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/icons/library_books-24px.svg
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/icons/play_circle_outline-24px.svg
+-rw-r--r--   0        0        0    35584 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/augur.png
+-rw-r--r--   0        0        0    22288 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/cinemaot.png
+-rw-r--r--   0        0        0    86973 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/dialogue.png
+-rw-r--r--   0        0        0    82238 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/distances.png
+-rw-r--r--   0        0        0    88998 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/distances_tests.png
+-rw-r--r--   0        0        0    27038 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/enrichment.png
+-rw-r--r--   0        0        0    52088 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/guide_rna_assignment.png
+-rw-r--r--   0        0        0    87099 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/milo.png
+-rw-r--r--   0        0        0    79422 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/mixscape.png
+-rw-r--r--   0        0        0    33037 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/ontology.png
+-rw-r--r--   0        0        0    61766 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/perturbation_space.png
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/placeholder.png
+-rw-r--r--   0        0        0    50106 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/sccoda.png
+-rw-r--r--   0        0        0    39935 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/sccoda_extended.png
+-rw-r--r--   0        0        0    83788 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/scgen_perturbation_prediction.png
+-rw-r--r--   0        0        0    41952 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_static/tutorials/tasccoda.png
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_templates/class_no_inherited.rst
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/tutorials/index.md
+-rw-r--r--   0        0        0    21208 2020-02-02 00:00:00.000000 pertpy-0.7.0/docs/usage/usage.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/py.typed
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/data/__init__.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/data/_dataloader.py
+-rw-r--r--   0        0        0    63179 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/data/_datasets.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/__init__.py
+-rw-r--r--   0        0        0    40644 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/_cell_line.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/_compound.py
+-rw-r--r--   0        0        0     9357 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/_drug.py
+-rw-r--r--   0        0        0    29476 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/_look_up.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/_metadata.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/metadata/_moa.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/plot/__init__.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/plot/_augur.py
+-rw-r--r--   0        0        0    26891 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/plot/_coda.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/plot/_guide_rna.py
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/plot/_milopy.py
+-rw-r--r--   0        0        0    14862 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/plot/_mixscape.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/preprocessing/__init__.py
+-rw-r--r--   0        0        0     7713 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/preprocessing/_guide_rna.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/__init__.py
+-rw-r--r--   0        0        0    55797 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_augur.py
+-rw-r--r--   0        0        0    39501 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_cinemaot.py
+-rw-r--r--   0        0        0    52143 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_dialogue.py
+-rw-r--r--   0        0        0    14360 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_differential_gene_expression.py
+-rw-r--r--   0        0        0    21922 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_enrichment.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_kernel_pca.py
+-rw-r--r--   0        0        0    43388 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_milo.py
+-rw-r--r--   0        0        0    52500 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_mixscape.py
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/decoupler_LICENSE
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/transferlearning_MMD_LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_coda/__init__.py
+-rw-r--r--   0        0        0   115262 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_coda/_base_coda.py
+-rw-r--r--   0        0        0    22849 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_coda/_sccoda.py
+-rw-r--r--   0        0        0    31033 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_coda/_tasccoda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_distances/__init__.py
+-rw-r--r--   0        0        0    13604 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_distances/_distance_tests.py
+-rw-r--r--   0        0        0    35619 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_distances/_distances.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_perturbation_space/__init__.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_perturbation_space/_clustering.py
+-rw-r--r--   0        0        0    22080 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_perturbation_space/_discriminator_classifiers.py
+-rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_perturbation_space/_metrics.py
+-rw-r--r--   0        0        0    18868 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_perturbation_space/_perturbation_space.py
+-rw-r--r--   0        0        0    12681 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_perturbation_space/_simple.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_scgen/__init__.py
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_scgen/_base_components.py
+-rw-r--r--   0        0        0    30705 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_scgen/_scgen.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_scgen/_scgenvae.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 pertpy-0.7.0/pertpy/tools/_scgen/_utils.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/metadata/test_cell_line.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/metadata/test_compound.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/metadata/test_drug.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/metadata/test_moa.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/preprocessing/test_grna_assignment.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/haber_data.csv
+-rw-r--r--   0        0        0   476779 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/r_result.csv
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_augur.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_cinemaot.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_differential_gene_expression.py
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_enrichment.py
+-rw-r--r--   0        0        0    11437 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_milo.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_mixscape.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/test_scgen.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_coda/test_sccoda.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_coda/test_tasccoda.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_distances/test_distance_tests.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_distances/test_distances.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_perturbation_space/test_discriminator_classifiers.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_perturbation_space/test_simple_cluster_space.py
+-rw-r--r--   0        0        0     7507 2020-02-02 00:00:00.000000 pertpy-0.7.0/tests/tools/_perturbation_space/test_simple_perturbation_space.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 pertpy-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pertpy-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 pertpy-0.7.0/README.md
+-rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 pertpy-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 pertpy-0.7.0/PKG-INFO
```

### Comparing `pertpy-0.6.0/CODE_OF_CONDUCT.md` & `pertpy-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/.github/labels.yml` & `pertpy-0.7.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/.github/pull_request_template.md` & `pertpy-0.7.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/.github/ISSUE_TEMPLATE/bug_report.yml` & `pertpy-0.7.0/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/.github/workflows/build.yml` & `pertpy-0.7.0/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     group: ${{ github.workflow }}-${{ github.ref }}
     cancel-in-progress: true
 
 jobs:
     package:
         runs-on: ubuntu-latest
         steps:
-            - uses: actions/checkout@v3
+            - uses: actions/checkout@v4
 
             - name: Set up Python 3.11
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v5
               with:
                   python-version: "3.11"
                   cache: "pip"
                   cache-dependency-path: "**/pyproject.toml"
 
             - name: Install build dependencies
               run: python -m pip install --upgrade pip wheel twine build
```

### Comparing `pertpy-0.6.0/.github/workflows/release.yml` & `pertpy-0.7.0/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 jobs:
     release:
         name: Release
         runs-on: ubuntu-latest
         steps:
             - name: Checkout code
-              uses: actions/checkout@v3
+              uses: actions/checkout@v4
 
             - name: Set up Python 3.11
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v5
               with:
                   python-version: "3.11"
 
             - name: Install hatch
               run: pip install hatch
 
             - name: Build project for distribution
```

### Comparing `pertpy-0.6.0/.github/workflows/test.yml` & `pertpy-0.7.0/.github/workflows/test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,41 +18,47 @@
                 shell: bash -e {0} # -e to fail on error
 
         strategy:
             fail-fast: false
             matrix:
                 include:
                     - os: ubuntu-latest
-                      python: "3.9"
+                      python: "3.10"
                     - os: ubuntu-latest
                       python: "3.11"
                     - os: ubuntu-latest
                       python: "3.11"
                       pip-flags: "--pre"
 
         env:
             OS: ${{ matrix.os }}
             PYTHON: ${{ matrix.python }}
 
         steps:
-            - uses: actions/checkout@v3
+            - uses: actions/checkout@v4
             - name: Set up Python ${{ matrix.python }}
-              uses: actions/setup-python@v4
+              uses: actions/setup-python@v5
               with:
                   python-version: ${{ matrix.python }}
                   cache: "pip"
                   cache-dependency-path: "**/pyproject.toml"
 
             - name: Install test dependencies
-              run: python -m pip install --upgrade pip wheel
+              run: python -m pip install --upgrade uv wheel
             - name: Install dependencies
-              run: pip install ${{ matrix.pip-flags }} ".[dev,test,coda]"
+              run: uv pip install --system ${{ matrix.pip-flags }} ".[dev,test,coda]"
 
             - name: Test
               env:
                   MPLBACKEND: agg
                   PLATFORM: ${{ matrix.os }}
                   DISPLAY: :42
-              run: pytest -v --cov --color=yes
+              run: coverage run -m pytest -v --color=yes
+
+            - name: Show coverage report
+              run: coverage report -m
 
             - name: Upload coverage
               uses: codecov/codecov-action@v3
+              with:
+                  fail_ci_if_error: true
+                  verbose: true
```

### Comparing `pertpy-0.6.0/docs/Makefile` & `pertpy-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/conf.py` & `pertpy-0.7.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 
 import sys
 from pathlib import Path
 
 HERE = Path(__file__).parent
 sys.path[:0] = [str(HERE.parent), str(HERE / "extensions")]
 
-needs_sphinx = "4.3"  # Nicer param docs
+needs_sphinx = "4.3"
 
-# General information about the project.
 project = "pertpy"
 copyright = "2021, Lukas Heumos, Theislab"
 author = "Lukas Heumos"
 github_repo = "pertpy"
 
-version = "0.6.0"
-release = "0.6.0"
+version = "0.7.0"
+release = "0.7.0"
 
 extensions = [
     "myst_parser",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "nbsphinx",
@@ -177,13 +176,15 @@
     "tutorials/notebooks/mixscape": "_static/tutorials/mixscape.png",
     "tutorials/notebooks/augur": "_static/tutorials/augur.png",
     "tutorials/notebooks/sccoda": "_static/tutorials/sccoda.png",
     "tutorials/notebooks/sccoda_extended": "_static/tutorials/sccoda_extended.png",
     "tutorials/notebooks/tasccoda": "_static/tutorials/tasccoda.png",
     "tutorials/notebooks/milo": "_static/tutorials/milo.png",
     "tutorials/notebooks/dialogue": "_static/tutorials/dialogue.png",
+    "tutorials/notebooks/enrichment": "_static/tutorials/enrichment.png",
     "tutorials/notebooks/distances": "_static/tutorials/distances.png",
     "tutorials/notebooks/distance_tests": "_static/tutorials/distances_tests.png",
+    "tutorials/notebooks/cinemaot": "_static/tutorials/cinemaot.png",
     "tutorials/notebooks/scgen_perturbation_prediction": "_static/tutorials/scgen_perturbation_prediction.png",
-    "tutorials/notebooks/scgen_batch_removal": "_static/tutorials/scgen_batch_removal.png",
     "tutorials/notebooks/ontology_mapping": "_static/tutorials/ontology.png",
+    "tutorials/notebooks/perturbation_space": "_static/tutorials/perturbation_space.png",
 }
```

### Comparing `pertpy-0.6.0/docs/contributing.md` & `pertpy-0.7.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/index.md` & `pertpy-0.7.0/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -21,23 +21,14 @@
     :link: tutorials/index
     :link-type: doc
 
     The tutorials walk you through real-world applications of pertpy.
 ```
 
 ```{eval-rst}
-.. card:: Use cases :octicon:`info;1em;`
-    :link: user_guide/index
-    :link-type: doc
-
-    pertpy has been applied to many use-cases. We highlight some of them here.
-    Interested in adding your use-case? Please talk to us.
-```
-
-```{eval-rst}
 .. card:: Discussion :octicon:`megaphone;1em;`
     :link: https://discourse.scverse.org/
 
     Need help? Reach out on our forum to get your questions answered!
 
 ```
 
@@ -56,15 +47,14 @@
 
 installation
 usage/usage
 tutorials/index
 contributing
 code_of_conduct
 Discussions <https://github.com/theislab/pertpy/discussions>
-authors
 references
 ```
 
 -   Consider citing [scanpy Genome Biology (2018)] along with original {doc}`references <references>`.
 -   A paper for pertpy is in the works.
 
 # Indices and tables
```

### Comparing `pertpy-0.6.0/docs/installation.md` & `pertpy-0.7.0/docs/installation.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,16 +10,25 @@
 
 ```console
 $ pip install pertpy
 ```
 
 This is the preferred method to install pertpy, as it will always install the most recent stable release.
 
-If you don't have [pip] installed, this [Python installation guide] can guide
-you through the process.
+If you don't have [pip] installed, this [Python installation guide] can guide you through the process.
+
+## Google Colab and TascCODA support
+
+TascCODA requires an additional set of dependencies (ete3 and pyqt5) that can be installed using
+
+```console
+$ pip install pertpy[coda]
+```
+
+this also solves any "AttributeError: module 'pertpy.plot' has no attribute 'coda'" issues.
 
 ## From sources
 
 The sources for pertpy can be downloaded from the [Github repo].
 Please note that you require [poetry] to be installed.
 
 You can either clone the public repository:
@@ -30,20 +39,14 @@
 
 Or download the [tarball]:
 
 ```console
 $ curl -OJL https://github.com/theislab/pertpy/tarball/master
 ```
 
-Once you have a copy of the source, you can install it with:
-
-```console
-$ make install
-```
-
 ## Apple Silicon
 
 If you want to install and use pertpy on a machine with macOS and M-Chip, the installation is slightly more complex.
 This is because pertpy depends on [scvi-tools], which can currently only run on Apple Silicon machines when installed
 using a native python version (due to a dependency on jax, which cannot be run via Rosetta).
 
 Follow these steps to install pertpy on an Apple Silicon machine (tested on a MacBook Pro with M1 chip and macOS 14.0):
@@ -56,15 +59,15 @@
     ```console
     $ brew install --cask mambaforge
     ```
 
 3. Create a new environment using mamba (here with python 3.10) and activate it
 
     ```console
-    $ mamba create -n pertpy-env python=3.10
+    $ mamba create -n pertpy-env python=3.11
     $ mamba activate pertpy-env
     ```
 
 4. Clone the GitHub Repository
 
     ```console
     $ git clone https://github.com/theislab/pertpy.git
```

### Comparing `pertpy-0.6.0/docs/make.bat` & `pertpy-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/references.bib` & `pertpy-0.7.0/docs/references.bib`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_ext/edit_on_github.py` & `pertpy-0.7.0/docs/_ext/edit_on_github.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Based on gist.github.com/MantasVaitkunas/7c16de233812adcb7028."""
+
 import os
 from typing import Any
 
 from sphinx.application import Sphinx
 
 __licence__ = "BSD (3 clause)"
```

### Comparing `pertpy-0.6.0/docs/_ext/typed_returns.py` & `pertpy-0.7.0/docs/_ext/typed_returns.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/SCVI_LICENSE` & `pertpy-0.7.0/docs/_static/SCVI_LICENSE`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/placeholder.png` & `pertpy-0.7.0/docs/_static/placeholder.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/css/overwrite.css` & `pertpy-0.7.0/docs/_static/css/overwrite.css`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/css/sphinx_gallery.css` & `pertpy-0.7.0/docs/_static/css/sphinx_gallery.css`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/distances.png` & `pertpy-0.7.0/docs/_static/tutorials/distances.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/distances_tests.png` & `pertpy-0.7.0/docs/_static/tutorials/distances_tests.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/guide_rna_assignment.png` & `pertpy-0.7.0/docs/_static/tutorials/guide_rna_assignment.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/ontology.png` & `pertpy-0.7.0/docs/_static/tutorials/ontology.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/placeholder.png` & `pertpy-0.7.0/docs/_static/tutorials/placeholder.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/sccoda.png` & `pertpy-0.7.0/docs/_static/tutorials/sccoda.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/sccoda_extended.png` & `pertpy-0.7.0/docs/_static/tutorials/sccoda_extended.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/scgen_batch_removal.png` & `pertpy-0.7.0/docs/_static/tutorials/scgen_perturbation_prediction.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_static/tutorials/tasccoda.png` & `pertpy-0.7.0/docs/_static/tutorials/tasccoda.png`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_templates/class_no_inherited.rst` & `pertpy-0.7.0/docs/_templates/class_no_inherited.rst`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/docs/_templates/autosummary/class.rst` & `pertpy-0.7.0/docs/_templates/autosummary/class.rst`

 * *Files 21% similar despite different names*

```diff
@@ -20,19 +20,33 @@
 
 {% block methods %}
 {% if methods %}
 Methods table
 ~~~~~~~~~~~~~
 
 .. autosummary::
+
+{% set plotting_methods = [] %}
+{% set other_methods = [] %}
+
 {% for item in methods %}
-    {%- if item != '__init__' %}
+    {%- if item.startswith('plot_') %}
+        {%- set _ = plotting_methods.append(item) %}
+    {% elif item != '__init__' %}
+        {%- set _ = other_methods.append(item) %}
+    {%- endif %}
+{% endfor %}
+
+{% for item in other_methods %}
+    ~{{ fullname }}.{{ item }}
+{% endfor %}
+
+{% for item in plotting_methods %}
     ~{{ fullname }}.{{ item }}
-    {%- endif -%}
-{%- endfor %}
+{% endfor %}
 {% endif %}
 {% endblock %}
 
 {% block attributes_documentation %}
 {% if attributes %}
 Attributes
 ~~~~~~~~~~~
```

### Comparing `pertpy-0.6.0/pertpy/__init__.py` & `pertpy-0.7.0/pertpy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Top-level package for pertpy."""
 
 __author__ = "Lukas Heumos"
 __email__ = "lukas.heumos@posteo.net"
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 import warnings
 
 from matplotlib import MatplotlibDeprecationWarning
 from numba import NumbaDeprecationWarning
 
 warnings.filterwarnings("ignore", category=NumbaDeprecationWarning)
 warnings.filterwarnings("ignore", category=MatplotlibDeprecationWarning)
-warnings.filterwarnings("ignore", category=UserWarning)
+warnings.filterwarnings("ignore", category=UserWarning, module="scvi._settings")
 
 from . import data as dt
+from . import metadata as md
 from . import plot as pl
 from . import preprocessing as pp
 from . import tools as tl
```

### Comparing `pertpy-0.6.0/pertpy/data/__init__.py` & `pertpy-0.7.0/pertpy/data/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,22 @@
     adamson_2016_upr_epistasis,
     adamson_2016_upr_perturb_seq,
     aissa_2021,
     bhattacherjee,
     burczynski_crohn,
     chang_2021,
     cinemaot_example,
+    combosciplex,
     datlinger_2017,
     datlinger_2021,
     dialogue_example,
     distance_example,
     dixit_2016,
     dixit_2016_raw,
+    dong_2023,
     frangieh_2021,
     frangieh_2021_protein,
     frangieh_2021_raw,
     frangieh_2021_rna,
     gasperini_2019_atscale,
     gasperini_2019_highmoi,
     gasperini_2019_lowmoi,
@@ -32,20 +34,22 @@
     replogle_2022_rpe1,
     sc_sim_augur,
     schiebinger_2019_16day,
     schiebinger_2019_18day,
     schraivogel_2020_tap_screen_chr8,
     schraivogel_2020_tap_screen_chr11,
     sciplex3_raw,
+    sciplex_gxe1,
     shifrut_2018,
-    smillie,
+    smillie_2019,
     srivatsan_2020_sciplex2,
     srivatsan_2020_sciplex3,
     srivatsan_2020_sciplex4,
     stephenson_2021_subsampled,
+    tasccoda_example,
     tian_2019_day7neuron,
     tian_2019_ipsc,
     tian_2021_crispra,
     tian_2021_crispri,
     weinreb_2020,
     xie_2017,
     zhao_2021,
```

### Comparing `pertpy-0.6.0/pertpy/data/_dataloader.py` & `pertpy-0.7.0/pertpy/data/_dataloader.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import tempfile
 from pathlib import Path
 from random import choice
 from string import ascii_lowercase
-from typing import Union
 from zipfile import ZipFile
 
 import requests
 from rich import print
 from rich.progress import Progress
 
 
 def _download(  # pragma: no cover
     url: str,
     output_file_name: str = None,
-    output_path: Union[str, Path] = None,
+    output_path: str | Path = None,
     block_size: int = 1024,
     overwrite: bool = False,
     is_zip: bool = False,
 ) -> None:
     """Downloads a dataset irrespective of the format.
 
     Args:
@@ -60,9 +59,8 @@
         # force the progress bar to 100% at the end
         progress.update(task, completed=total, refresh=True)
 
     if is_zip:
         output_path = output_path or tempfile.gettempdir()
         with ZipFile(download_to_path, "r") as zip_obj:
             zip_obj.extractall(path=output_path)
-            extracted = zip_obj.namelist()
-            print(extracted)
+            zip_obj.namelist()
```

### Comparing `pertpy-0.6.0/pertpy/data/_datasets.py` & `pertpy-0.7.0/pertpy/data/_datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     Returns:
         :class:`~mudata.MuData` object of the ECCITE-seq dataset
     """
     import muon as mu
 
     output_file_name = "papalexi_2021.h5mu"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/36509460",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -59,15 +59,15 @@
     References:
         Obtained from https://github.com/neurorestore/Augur
 
     Returns:
         :class:`~anndata.AnnData` object of a simulated single-cell RNA seq dataset
     """
     output_file_name = "sc_sim_augur.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/31645886",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -89,15 +89,15 @@
         adolescence and addiction. Nat Commun. 2019 Sep 13;10(1):4169.
         doi: 10.1038/s41467-019-12054-3. PMID: 31519873; PMCID: PMC6744514.
 
     Returns:
         :class:`~anndata.AnnData` object of a single-cell RNA seq dataset
     """
     output_file_name = "bhattacherjee_rna.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34526528",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -106,49 +106,51 @@
     return adata
 
 
 def sciplex3_raw() -> AnnData:  # pragma: no cover
     """Raw sciplex3 perturbation dataset curated for perturbation modeling.
 
     References:
-        Srivatsan SR, McFaline-Figueroa JL, Ramani V, Saunders L, Cao J, Packer J,
-        Pliner HA, Jackson DL, Daza RM, Christiansen L, Zhang F, Steemers F,
-        Shendure J, Trapnell C. Massively multiplex chemical transcriptomics at
+        Srivatsan SR et al., Trapnell C. Massively multiplex chemical transcriptomics at
         single-cell resolution. Science. 2020 Jan 3;367(6473):45-51.
         doi: 10.1126/science.aax6234. Epub 2019 Dec 5. PMID: 31806696; PMCID: PMC7289078.
 
     Returns:
         :class:`~anndata.AnnData` object of a single-cell RNA seq dataset
     """
     output_file_name = "sciplex3.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/33979517",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
-def smillie() -> AnnData:  # pragma: no cover
-    """scRNA-seq data of the small intestine of mice under Ulcerative Colitis.
+def tasccoda_example() -> AnnData:  # pragma: no cover
+    """Example for the coda part of a mudata object.
+
+    Resulting AnnData object (mudata['coda']) when preparing a dataset for processing with tascCODA.
+    Created using the smillie dataset, which comprises scRNA-seq data of the small intestine of mice under Ulcerative Colitis.
+    The full dataset containing the actual count data can be obtained via smillie_2019().
 
     References:
         Smillie, Christopher S et al. “Intra- and Inter-cellular Rewiring of the Human Colon during Ulcerative Colitis.”
         Cell vol. 178,3 (2019): 714-730.e22. doi:10.1016/j.cell.2019.06.029
 
     Returns:
         :class:`~anndata.AnnData` object of the dataset.
     """
-    output_file_name = "smillie.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_name = "tasccoda_smillie.h5ad"
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/38648585",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -169,15 +171,15 @@
         screens in patient models define mechanisms of cancer immune evasion.
         Nat Genet 53, 332–341 (2021). https://doi.org/10.1038/s41588-021-00779-1
 
     Returns:
         :class:`~anndata.AnnData` object of the Perturb-CITE-seq data.
     """
     output_file_name = "frangieh_2021.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34013717",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -198,15 +200,15 @@
         screens in patient models define mechanisms of cancer immune evasion.
         Nat Genet 53, 332–341 (2021). https://doi.org/10.1038/s41588-021-00779-1
 
     Returns:
         :class:`~anndata.AnnData` object of raw Perturb-CITE-seq data.
     """
     output_file_name = "frangieh_2021_raw.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34012565",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -227,15 +229,15 @@
         Scalable Single-Cell RNA Profiling of Pooled Genetic Screens.
         Cell 2016 Dec 15;167(7):1853-1866.e17. DOI:https://doi.org/10.1016/j.cell.2016.11.038
 
     Returns:
         :class:`~anndata.AnnData` object of raw Perturb-seq data.
     """
     output_file_name = "dixit_2016_raw.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34012565",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -256,15 +258,15 @@
         Scalable Single-Cell RNA Profiling of Pooled Genetic Screens.
         Cell 2016 Dec 15;167(7):1853-1866.e17. DOI:https://doi.org/10.1016/j.cell.2016.11.038
 
     Returns:
         :class:`~anndata.AnnData` object of Perturb-seq data
     """
     output_file_name = "dixit_2016.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34014608",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -284,15 +286,15 @@
         single-cell phenotypes.” Science (New York, N.Y.) vol. 365,6455 (2019): 786-793.
         doi:10.1126/science.aax4438
 
     Returns:
         :class:`~anndata.AnnData` object of single-cell pooled CRISPR screening.
     """
     output_file_name = "norman_2019.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34027562",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -312,15 +314,15 @@
         single-cell phenotypes.” Science (New York, N.Y.) vol. 365,6455 (2019): 786-793.
         doi:10.1126/science.aax4438
 
     Returns:
         :class:`~anndata.AnnData` object of raw single-cell pooled CRISPR screening
     """
     output_file_name = "norman_2019_raw.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34002548",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -335,18 +337,18 @@
     References:
         https://github.com/livnatje/DIALOGUE/wiki/Example
 
     Returns:
         :class:`~anndata.AnnData` object
     """
     output_file_name = "dialogue_example.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://figshare.com/ndownloader/files/34490714",
+            url="https://figshare.com/ndownloader/files/43462662",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -357,15 +359,15 @@
 
     Processed and subsetted version of original Perturb-seq dataset by Dixit et al.
 
     Returns:
         :class:`~anndata.AnnData` object
     """
     output_file_name = "distances_example_data.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/39561379",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -388,15 +390,15 @@
         using natural genetic variation.
         Nat Biotechnol 36, 89–94 (2018). https://doi.org/10.1038/nbt.4042
 
     Returns:
         :class:`~anndata.AnnData` object of droplet-based single cell RNA-sequencing
     """
     output_file_name = "kang_2018.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/34464122",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -417,15 +419,15 @@
         Single-cell multi-omics analysis of the immune response in COVID-19.
         Nature Medicine, 27(5). https://doi.org/10.1038/s41591-021-01329-2
 
     Returns:
         :class:`~anndata.AnnData` object of scRNA-seq profiles
     """
     output_file_name = "stephenson_2021_subsampled.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/38171703",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -444,15 +446,15 @@
         Haber, Adam L. et al. “A single-cell survey of the small intestinal epithelium” Nature vol. 551 (2017): 333-339
         doi:10.1038/nature24489
 
     Returns:
         :class:`~anndata.AnnData` object
     """
     output_file_name = "haber_2017_regions.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/38169900",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
@@ -471,18 +473,18 @@
         Publication: https://www.sciencedirect.com/science/article/pii/S0092867416316609?via%3Dihub \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "adamson_2016_pilot.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/AdamsonWeissman2016_GSM2406675_10X001.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/AdamsonWeissman2016_GSM2406675_10X001.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -502,18 +504,18 @@
         Publication: https://www.sciencedirect.com/science/article/pii/S0092867416316609?via%3Dihub \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb preparedsingle-cell perturbation data
     """
     output_file_name = "adamson_2016_upr_epistasis.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/AdamsonWeissman2016_GSM2406677_10X005.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/AdamsonWeissman2016_GSM2406677_10X005.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -531,18 +533,18 @@
         Publication: https://www.sciencedirect.com/science/article/pii/S0092867416316609?via%3Dihub \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "adamson_2016_upr_perturb_seq.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/AdamsonWeissman2016_GSM2406681_10X010.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/AdamsonWeissman2016_GSM2406681_10X010.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -558,18 +560,18 @@
         Publication: https://www.nature.com/articles/s41467-021-21884-z \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "aissa_2021.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/AissaBenevolenskaya2021.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/AissaBenevolenskaya2021.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -587,18 +589,18 @@
     References:
         https://www.nature.com/articles/s41587-021-01005-3
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "chang_2021.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/ChangYe2021.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/ChangYe2021.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -618,18 +620,18 @@
         Publication: https://www.nature.com/articles/nmeth.4177 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "datlinger_2017.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/DatlingerBock2017.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/DatlingerBock2017.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -648,18 +650,18 @@
         Publication: https://doi.org/10.1038/s41592-021-01153-z \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
      Returns:
          :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "datlinger_2021.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/DatlingerBock2021.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/DatlingerBock2021.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -679,18 +681,18 @@
         Publication: https://doi.org/10.1038/s41588-021-00779-1 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "frangieh_2021_protein.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/FrangiehIzar2021_protein.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/FrangiehIzar2021_protein.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -710,18 +712,18 @@
         Publication: https://doi.org/10.1038/s41588-021-00779-1 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "frangieh_2021_rna.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/FrangiehIzar2021_RNA.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/FrangiehIzar2021_RNA.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -738,18 +740,18 @@
         Publication: https://doi.org/10.1016/j.cell.2018.11.029 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "gasperini_2019_atscale.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/GasperiniShendure2019_atscale.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/GasperiniShendure2019_atscale.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -767,18 +769,18 @@
         Publication: https://doi.org/10.1016/j.cell.2018.11.029 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "gasperini_2019_highmoi.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/GasperiniShendure2019_highMOI.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/GasperiniShendure2019_highMOI.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -796,18 +798,18 @@
         Publication: https://doi.org/10.1016/j.cell.2018.11.029 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "gasperini_2019_lowmoi.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/GasperiniShendure2019_lowMOI.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/GasperiniShendure2019_lowMOI.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -824,18 +826,18 @@
         Publication: https://doi.org/10.1038/s41587-019-0372-z \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of a scPerturb prepared single-cell dataset
     """
     output_file_name = "gehring_2019.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/GehringPachter2019.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/GehringPachter2019.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -853,18 +855,18 @@
         Publication: https://doi.org/10.1038/s41467-020-17440-w \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "mcfarland_2020.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/McFarlandTsherniak2020.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/McFarlandTsherniak2020.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -882,29 +884,29 @@
         Publication: https://doi.org/10.1016/j.cell.2022.05.013 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "replogle_2022_k562_essential.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/ReplogleWeissman2022_K562_essential.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/ReplogleWeissman2022_K562_essential.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def replogle_2022_k562_gwps() -> AnnData:  # pragma: no cover
-    """K562 cells transduced with CRISPRi (day 8 after transcduction).
+    """K562 cells transduced with CRISPRi (day 8 after transduction).
 
     Here, the authors used a compact, multiplexed CRISPR interference (CRISPRi) library
     to assay thousands of loss-of-function genetic perturbations with single-cell RNA sequencing
     in chronic myeloid leukemia (CML) (K562) cell lines. For the K562 day 8 genome-scale
     Perturb-seq experiment, library lentivirus was packaged into lentivirus in 293T cells and
     empirically measured in K562 cells to obtain viral titers. CRISPRi K562 cells were transduced
     and all expressed genes were targeted at day 8 after transduction
@@ -913,29 +915,29 @@
         Publication: https://doi.org/10.1016/j.cell.2022.05.013 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "replogle_2022_k562_gwps.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/ReplogleWeissman2022_K562_gwps.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/ReplogleWeissman2022_K562_gwps.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def replogle_2022_rpe1() -> AnnData:  # pragma: no cover
-    """RPE1 cells transduced with CRISPRi (day 7 after transcduction).
+    """RPE1 cells transduced with CRISPRi (day 7 after transduction).
 
     For day 7 essential-scale Perturb-seq experiment in retinal pigment epithelial (RPE1)
     cell lines, library lentivirus was packaged into lentivirus in 293T cells and
     empirically measured in RPE1 cells to obtain viral titers. CRISPRi RPE1 cells expressing
     ZIM3 KRAB-dCas9-P2A-BFP were transduced. 20Q1 Cancer Dependency Map common essential
     genes were targeted at day 7 after transduction.
 
@@ -943,18 +945,18 @@
         Publication: https://doi.org/10.1016/j.cell.2022.05.013 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "replogle_2022_rpe1.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/ReplogleWeissman2022_rpe1.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/ReplogleWeissman2022_rpe1.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -974,18 +976,18 @@
         Publication: https://doi.org/10.1016/j.cell.2019.01.006 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "schiebinger_2019_16day.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SchiebingerLander2019_GSE106340.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/SchiebingerLander2019_GSE106340.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1003,18 +1005,18 @@
         Publication: https://doi.org/10.1016/j.cell.2019.01.006 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "Schiebinger_2019_18day.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SchiebingerLander2019_GSE115943.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/SchiebingerLander2019_GSE115943.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1032,18 +1034,18 @@
         Publication: https://doi.org/10.1038/s41592-020-0837-5 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "schraivogel_2020_tap_screen_chr11.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SchraivogelSteinmetz2020_TAP_SCREEN__chromosome_11_screen.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/SchraivogelSteinmetz2020_TAP_SCREEN__chromosome_11_screen.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1061,18 +1063,18 @@
         Publication: https://doi.org/10.1038/s41592-020-0837-5 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "schraivogel_2020_tap_screen_chr8.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SchraivogelSteinmetz2020_TAP_SCREEN__chromosome_8_screen.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/SchraivogelSteinmetz2020_TAP_SCREEN__chromosome_8_screen.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1091,18 +1093,18 @@
         Publication: https://doi.org/10.1016/j.cell.2018.10.024 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "shifrut_2018.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/ShifrutMarson2018.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/ShifrutMarson2018.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1122,18 +1124,18 @@
         Publication: https://doi.org/10.1126/science.aax6234 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "srivatsan_2020_sciplex2.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SrivatsanTrapnell2020_sciplex2.h5ad?download=1",
+            url="https://zenodo.org/record/10044268/files/SrivatsanTrapnell2020_sciplex2.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1151,18 +1153,18 @@
         Publication: https://doi.org/10.1126/science.aax6234 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "srivatsan_2020_sciplex3.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SrivatsanTrapnell2020_sciplex3.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/SrivatsanTrapnell2020_sciplex3.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1183,18 +1185,18 @@
         Publication: https://doi.org/10.1126/science.aax6234 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "srivatsan_2020_sciplex4.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/SrivatsanTrapnell2020_sciplex4.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/SrivatsanTrapnell2020_sciplex4.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1215,18 +1217,18 @@
         Publication: https://doi.org/10.1016/j.neuron.2019.07.014 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "tian_2019_day7neuron.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/TianKampmann2019_day7neuron.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/TianKampmann2019_day7neuron.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1247,18 +1249,18 @@
         Publication: https://doi.org/10.1016/j.neuron.2019.07.014 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "tian_2019_iPSC.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/TianKampmann2019_iPSC.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/TianKampmann2019_iPSC.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1277,18 +1279,18 @@
         Publication: https://doi.org/10.1038/s41593-021-00862-0 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "tian_2021_crispra.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/TianKampmann2021_CRISPRa.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/TianKampmann2021_CRISPRa.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1307,18 +1309,18 @@
         Publication: https://doi.org/10.1038/s41593-021-00862-0 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "tian_2021_crispri.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/TianKampmann2021_CRISPRi.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/TianKampmann2021_CRISPRi.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1334,18 +1336,18 @@
         Publication: https://www.science.org/doi/10.1126/science.aaw3381 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "weinreb_2020.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/WeinrebKlein2020.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/WeinrebKlein2020.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1362,18 +1364,18 @@
         Publication: https://doi.org/10.1016/j.molcel.2017.03.007 \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "xie_2017.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/XieHon2017.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/XieHon2017.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
@@ -1392,40 +1394,149 @@
         Publication: https://doi.org/10.1186/s13073-021-00894-y \
         Obtained from scperturb: http://projects.sanderlab.org/scperturb/
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "zhaoSims2021.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
-            url="https://zenodo.org/record/7278143/files/ZhaoSims2021.h5ad?download=1",
+            url="https://zenodo.org/records/10044268/files/ZhaoSims2021.h5ad?download=1",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def cinemaot_example() -> AnnData:  # pragma: no cover:
-    """CINEMA-OT Example dataset.
+    """Subsampled CINEMA-OT example dataset.
+
+    Ex vivo stimulation of human peripheral blood mononuclear cells (PBMC) with interferon. This is a subsampled
+    dataset containing 1000 cells, either without stimulation or stimulated with IFNb. The full dataset is available
+    via the cinemaot_full() function.
 
-    Ex vivo stimulation of human peripheral blood mononuclear cells (PBMC) with interferon.
 
     Returns:
         :class:`~anndata.AnnData` object of PBMCs stimulated with interferon.
     """
     output_file_name = "cinemaot_example.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    output_file_path = settings.datasetdir / output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/42362796?private_link=270b0d2c7f1ea57c366d",
             output_file_name=output_file_name,
             output_path=settings.datasetdir,
             is_zip=False,
         )
     adata = sc.read_h5ad(output_file_path)
 
     return adata
+
+
+def dong_2023() -> AnnData:  # pragma: no cover
+    """Complete CINEMA-OT dataset.
+
+    Ex vivo stimulation of human peripheral blood mononuclear cells (PBMC) with interferon. This is the full dataset
+    containing 9209 cells that were stimulated with IFNb, IFNg, IFNb+IFNg, or left unstimulated. A subsampled version
+    of the dataset is available via cinemaot_example().
+
+    References:
+        Preprint: https://doi.org/10.1101/2022.07.31.502173
+        Dataset available here: https://datadryad.org/stash/dataset/doi:10.5061/dryad.4xgxd25g1
+
+    Returns:
+        :class:`~anndata.AnnData` object of PBMCs stimulated with interferon.
+    """
+    output_file_name = "dong_2023.h5ad"
+    output_file_path = settings.datasetdir / output_file_name
+    if not Path(output_file_path).exists():
+        _download(
+            url="https://figshare.com/ndownloader/files/43068190",
+            output_file_name=output_file_name,
+            output_path=settings.datasetdir,
+            is_zip=False,
+        )
+    adata = sc.read_h5ad(output_file_path)
+
+    return adata
+
+
+def smillie_2019() -> AnnData:  # pragma: no cover
+    """scRNA-seq data of the small intestine of mice under Ulcerative Colitis.
+
+    The resulting AnnData when preparing this dataset for processing with tascCODA is available via tasccoda_example().
+
+    References:
+        Smillie, Christopher S et al. “Intra- and Inter-cellular Rewiring of the Human Colon during Ulcerative Colitis.”
+        Cell vol. 178,3 (2019): 714-730.e22. doi:10.1016/j.cell.2019.06.029
+
+    Returns:
+        :class:`~anndata.AnnData` object of the dataset.
+    """
+    output_file_name = "smillie_2019.h5ad.zip"
+    output_file_path = settings.datasetdir / Path(output_file_name).with_suffix("")
+    if not Path(output_file_path).exists():
+        _download(
+            url="https://figshare.com/ndownloader/files/43317285",
+            output_file_name=output_file_name,
+            output_path=settings.datasetdir,
+            is_zip=True,
+        )
+    adata = sc.read_h5ad(output_file_path)
+
+    return adata
+
+
+def combosciplex() -> AnnData:  # pragma: no cover
+    """scRNA-seq subset of the combinatorial experiment of sciplex3.
+
+    References:
+        Srivatsan SR et al., Trapnell C. Massively multiplex chemical transcriptomics at
+        single-cell resolution. Science. 2020 Jan 3;367(6473):45-51.
+        doi: 10.1126/science.aax6234. Epub 2019 Dec 5. PMID: 31806696; PMCID: PMC7289078.
+
+    Returns:
+        :class:`~anndata.AnnData` object of the dataset.
+    """
+    output_file_name = "combosciplex.h5ad"
+    output_file_path = settings.datasetdir / output_file_name
+    if not Path(output_file_path).exists():
+        _download(
+            url="https://figshare.com/ndownloader/files/44229635",
+            output_file_name=output_file_name,
+            output_path=settings.datasetdir,
+            is_zip=False,
+        )
+    adata = sc.read_h5ad(output_file_path)
+
+    return adata
+
+
+def sciplex_gxe1() -> AnnData:  # pragma: no cover
+    """sci-Plex-GxE combined chemical and genetic profiling of A172 dCas9-KRAB cells
+    genetically perturbed for HPRT1 or mismtach repair genes exposed to 6-thioguanine and temozolomide,
+    respectively, and A172 dCas9-SunTag cells genetically perturbed for HPRT1 exposed to 6-thioguanine.
+
+    References:
+        McFaline-Figueroa JL et al., Trapnell C. Multiplex single-cell chemical genomics reveals
+        the kinase dependence of the response to targeted therapy. Cell Genomics. 2024 Volume 4, Issue 2.
+        doi: 10.1016/j.xgen.2023.100487
+
+    Returns:
+        :class:`~anndata.AnnData` object of the dataset.
+    """
+    output_file_name = "sciPlexGxE_1_GSM7056148.h5ad"
+    output_file_path = settings.datasetdir / output_file_name
+    if not Path(output_file_path).exists():
+        _download(
+            url="https://figshare.com/ndownloader/files/45372454",
+            output_file_name=output_file_name,
+            output_path=settings.datasetdir,
+            is_zip=False,
+        )
+    adata = sc.read_h5ad(output_file_path)
+
+    return adata
```

### Comparing `pertpy-0.6.0/pertpy/plot/_guide_rna.py` & `pertpy-0.7.0/pertpy/plot/_guide_rna.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from __future__ import annotations
 
+import warnings
 from typing import TYPE_CHECKING
 
-import numpy as np
-import scanpy as sc
-
 if TYPE_CHECKING:
+    import numpy as np
     from anndata import AnnData
-    from matplotlib.axes import Axes
 
 
 class GuideRnaPlot:
     @staticmethod
     def heatmap(
         adata: AnnData,
         layer: str | None = None,
         order_by: np.ndarray | str | None = None,
         key_to_save_order: str = None,
-        **kwds,
-    ) -> list[Axes]:
+        **kwargs,
+    ):
         """Heatmap plotting of guide RNA expression matrix.
 
         Assuming guides have sparse expression, this function reorders cells
         and plots guide RNA expression so that a nice sparse representation is achieved.
         The cell ordering can be stored and reused in future plots to obtain consistent
         plots before and after analysis of the guide RNA expression.
         Note: This function expects a log-normalized or binary data.
@@ -32,51 +30,35 @@
              layer: Key to the layer containing log normalized count values of the gRNAs.
                     adata.X is used if layer is None.
              order_by: The order of cells in y axis. Defaults to None.
                        If None, cells will be reordered to have a nice sparse representation.
                        If a string is provided, adata.obs[order_by] will be used as the order.
                        If a numpy array is provided, the array will be used for ordering.
              key_to_save_order: The obs key to save cell orders in the current plot. Only saves if not None.
-             kwds: Are passed to sc.pl.heatmap.
+             kwargs: Are passed to sc.pl.heatmap.
 
          Returns:
              List of Axes. Alternatively you can pass save or show parameters as they will be passed to sc.pl.heatmap.
              Order of cells in the y axis will be saved on adata.obs[key_to_save_order] if provided.
 
         Examples:
             Each cell is assigned to gRNA that occurs at least 5 times in the respective cell, which is then
             visualized using a heatmap.
 
             >>> import pertpy as pt
-            >>> mdata = pt.data.papalexi_2021()
-            >>> gdo = mdata.mod['gdo']
+            >>> mdata = pt.dt.papalexi_2021()
+            >>> gdo = mdata.mod["gdo"]
             >>> ga = pt.pp.GuideAssignment()
             >>> ga.assign_by_threshold(gdo, assignment_threshold=5)
-            >>> pt.pl.guide.heatmap(gdo)
+            >>> ga.plot_heatmap(gdo)
         """
-        data = adata.X if layer is None else adata.layers[layer]
-
-        if order_by is None:
-            max_guide_index = np.where(
-                np.array(data.max(axis=1)).squeeze() != data.min(), np.array(data.argmax(axis=1)).squeeze(), -1
-            )
-            order = np.argsort(max_guide_index)
-        elif isinstance(order_by, str):
-            order = adata.obs[order_by]
-        else:
-            order = order_by
-
-        adata.obs["_tmp_pertpy_grna_plot_dummy_group"] = ""
-        if key_to_save_order is not None:
-            adata.obs[key_to_save_order] = order
-        axis_group = sc.pl.heatmap(
-            adata[order],
-            adata.var.index.tolist(),
-            groupby="_tmp_pertpy_grna_plot_dummy_group",
-            cmap="viridis",
-            use_raw=False,
-            dendrogram=False,
-            layer=layer,
-            **kwds,
+        warnings.warn(
+            "This function is deprecated and will be removed in pertpy 0.8.0!"
+            " Please use the corresponding 'pt.tl' object",
+            FutureWarning,
+            stacklevel=2,
         )
-        del adata.obs["_tmp_pertpy_grna_plot_dummy_group"]
-        return axis_group
+
+        from pertpy.preprocessing import GuideAssignment
+
+        ga = GuideAssignment()
+        ga.plot_heatmap(adata=adata, layer=layer, order_by=order_by, key_to_save_order=key_to_save_order, kwargs=kwargs)
```

### Comparing `pertpy-0.6.0/pertpy/tools/__init__.py` & `pertpy-0.7.0/pertpy/tools/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-from rich import print
-
 from pertpy.tools._augur import Augur
 from pertpy.tools._cinemaot import Cinemaot
+from pertpy.tools._coda._sccoda import Sccoda
+from pertpy.tools._coda._tasccoda import Tasccoda
 from pertpy.tools._dialogue import Dialogue
 from pertpy.tools._differential_gene_expression import DifferentialGeneExpression
 from pertpy.tools._distances._distance_tests import DistanceTest
 from pertpy.tools._distances._distances import Distance
-from pertpy.tools._metadata._cell_line import CellLineMetaData
+from pertpy.tools._enrichment import Enrichment
 from pertpy.tools._milo import Milo
 from pertpy.tools._mixscape import Mixscape
 from pertpy.tools._perturbation_space._clustering import ClusteringSpace
-from pertpy.tools._perturbation_space._discriminator_classifier import DiscriminatorClassifierSpace
+from pertpy.tools._perturbation_space._discriminator_classifiers import (
+    DiscriminatorClassifierSpace,
+    LRClassifierSpace,
+    MLPClassifierSpace,
+)
 from pertpy.tools._perturbation_space._simple import CentroidSpace, DBSCANSpace, KMeansSpace, PseudobulkSpace
 from pertpy.tools._scgen import SCGEN
-
-try:
-    from pertpy.tools._coda._sccoda import Sccoda
-    from pertpy.tools._coda._tasccoda import Tasccoda
-except ImportError as e:
-    if "ete3" in str(e):
-        print("[bold yellow]To use sccoda or tasccoda please install ete3 with [green]pip install ete3")
-    else:
-        raise e
```

### Comparing `pertpy-0.6.0/pertpy/tools/_augur.py` & `pertpy-0.7.0/pertpy/tools/_augur.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import random
 from collections import defaultdict
 from dataclasses import dataclass
 from math import floor, nan
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
+import anndata as ad
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import statsmodels.api as sm
 from anndata import AnnData
 from joblib import Parallel, delayed
 from rich import print
@@ -30,14 +32,18 @@
     roc_auc_score,
 )
 from sklearn.model_selection import StratifiedKFold, cross_validate
 from sklearn.preprocessing import LabelEncoder
 from skmisc.loess import loess
 from statsmodels.stats.multitest import fdrcorrection
 
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from matplotlib.figure import Figure
+
 
 @dataclass
 class Params:
     """Type signature for random forest and logistic regression parameters.
 
     Parameters:
         n_estimators: defines the number of trees in the forest;
@@ -131,16 +137,16 @@
         if len(adata.obs["label"].unique()) < 2:
             raise ValueError("Less than two unique labels in dataset. At least two are needed for the analysis.")
         # dummy variables for categorical data
         if adata.obs["label"].dtype.name == "category":
             # filter samples according to label
             if condition_label is not None and treatment_label is not None:
                 print(f"Filtering samples with {condition_label} and {treatment_label} labels.")
-                adata = AnnData.concatenate(
-                    adata[adata.obs["label"] == condition_label], adata[adata.obs["label"] == treatment_label]
+                adata = ad.concat(
+                    [adata[adata.obs["label"] == condition_label], adata[adata.obs["label"] == treatment_label]]
                 )
             label_encoder = LabelEncoder()
             adata.obs["y_"] = label_encoder.fit_transform(adata.obs["label"])
         else:
             y = adata.obs["label"].to_frame()
             y = y.rename(columns={"label": "y_"})
             adata.obs = pd.concat([adata.obs, y], axis=1)
@@ -210,15 +216,17 @@
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.sc_sim_augur()
             >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
             >>> loaded_data = ag_rfc.load(adata)
             >>> ag_rfc.select_highly_variable(loaded_data)
             >>> features = loaded_data.var_names
-            >>> subsample = ag_rfc.sample(loaded_data, categorical=True, subsample_size=20, random_state=42, features=loaded_data.var_names)
+            >>> subsample = ag_rfc.sample(
+            ...     loaded_data, categorical=True, subsample_size=20, random_state=42, features=loaded_data.var_names
+            ... )
         """
         # export subsampling.
         random.seed(random_state)
         if categorical:
             label_subsamples = []
             y_encodings = adata.obs["y_"].unique()
             for code in y_encodings:
@@ -226,15 +234,15 @@
                     sc.pp.subsample(
                         adata[adata.obs["y_"] == code, features],
                         n_obs=subsample_size,
                         copy=True,
                         random_state=random_state,
                     )
                 )
-            subsample = AnnData.concatenate(*label_subsamples, index_unique=None)
+            subsample = ad.concat([*label_subsamples], index_unique=None)
         else:
             subsample = sc.pp.subsample(adata[:, features], n_obs=subsample_size, copy=True, random_state=random_state)
 
         # filter features with 0 variance
         subsample.var["highly_variable"] = False
         subsample.var["means"] = np.ravel(subsample.X.mean(axis=0))
         # Converting because the Syntax for power for numpy arrays is different -> use sparse Syntax as default
@@ -405,25 +413,25 @@
         Examples:
             >>> import pertpy as pt
             >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
             >>> scorer = ag_rfc.set_scorer(True, 0)
         """
         if multiclass:
             return {
-                "augur_score": make_scorer(roc_auc_score, multi_class="ovo", needs_proba=True),
-                "auc": make_scorer(roc_auc_score, multi_class="ovo", needs_proba=True),
+                "augur_score": make_scorer(roc_auc_score, multi_class="ovo", response_method="predict_proba"),
+                "auc": make_scorer(roc_auc_score, multi_class="ovo", response_method="predict_proba"),
                 "accuracy": make_scorer(accuracy_score),
                 "precision": make_scorer(precision_score, average="macro", zero_division=zero_division),
                 "f1": make_scorer(f1_score, average="macro"),
                 "recall": make_scorer(recall_score, average="macro"),
             }
         return (
             {
-                "augur_score": make_scorer(roc_auc_score, needs_proba=True),
-                "auc": make_scorer(roc_auc_score, needs_proba=True),
+                "augur_score": make_scorer(roc_auc_score, response_method="predict_proba"),
+                "auc": make_scorer(roc_auc_score, response_method="predict_proba"),
                 "accuracy": make_scorer(accuracy_score),
                 "precision": make_scorer(precision_score, average="binary", zero_division=zero_division),
                 "f1": make_scorer(f1_score, average="binary"),
                 "recall": make_scorer(recall_score, average="binary"),
             }
             if isinstance(self.estimator, RandomForestClassifier) or isinstance(self.estimator, LogisticRegression)
             else {
@@ -484,24 +492,24 @@
         results["subsample_idx"] = subsample_idx
         for score in scorer.keys():
             results[f"mean_{score}"] = results[f"test_{score}"].mean()
 
         # feature importances
         feature_importances = defaultdict(list)
         if isinstance(self.estimator, RandomForestClassifier) or isinstance(self.estimator, RandomForestRegressor):
-            for fold, estimator in list(zip(range(len(results["estimator"])), results["estimator"])):
+            for fold, estimator in list(zip(range(len(results["estimator"])), results["estimator"], strict=False)):
                 feature_importances["genes"].extend(x.columns.tolist())
                 feature_importances["feature_importances"].extend(estimator.feature_importances_.tolist())
                 feature_importances["subsample_idx"].extend(len(x.columns) * [subsample_idx])
                 feature_importances["fold"].extend(len(x.columns) * [fold])
 
         # standardized coefficients with Agresti method
         # cf. https://think-lab.github.io/d/205/#3
         if isinstance(self.estimator, LogisticRegression):
-            for fold, self.estimator in list(zip(range(len(results["estimator"])), results["estimator"])):
+            for fold, self.estimator in list(zip(range(len(results["estimator"])), results["estimator"], strict=False)):
                 feature_importances["genes"].extend(x.columns.tolist())
                 feature_importances["feature_importances"].extend(
                     (self.estimator.coef_ * self.estimator.coef_.std()).flatten().tolist()
                 )
                 feature_importances["subsample_idx"].extend(len(x.columns) * [subsample_idx])
                 feature_importances["fold"].extend(len(x.columns) * [fold])
 
@@ -719,14 +727,15 @@
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.sc_sim_augur()
             >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
             >>> loaded_data = ag_rfc.load(adata)
             >>> h_adata, h_results = ag_rfc.predict(loaded_data, subsample_size=20, n_threads=4)
         """
+        adata = adata.copy()
         if augur_mode == "permute" and n_subsamples < 100:
             n_subsamples = 500
         if is_regressor(self.estimator) and len(adata.obs["y_"].unique()) <= 3:
             raise ValueError(
                 f"Regressors cannot be used on {len(adata.obs['label'].unique())} labels. Try a classifier."
             )
         if isinstance(self.estimator, LogisticRegression) and len(adata.obs["y_"].unique()) > 2:
@@ -761,14 +770,15 @@
             if len(cell_type_subsample) < min_cells:
                 print(
                     f"[bold red]Skipping {cell_type} cell type - {len(cell_type_subsample)} samples is less than min_cells {min_cells}."
                 )
             elif (
                 cell_type_subsample.obs.groupby(
                     ["cell_type", "label"],
+                    observed=True,
                 ).y_.count()
                 < subsample_size
             ).any():
                 print(
                     f"[bold red]Skipping {cell_type} cell type - the number of samples for at least one class type is less than "
                     f"subsample size {subsample_size}."
                 )
@@ -800,15 +810,15 @@
                     for key, value in dictionary.items():
                         results["feature_importances"][key].extend(value)
                 results["feature_importances"]["cell_type"].extend(
                     [cell_type]
                     * (len(results["feature_importances"]["genes"]) - len(results["feature_importances"]["cell_type"]))
                 )
 
-                for idx, cv in zip(range(n_subsamples), results[cell_type]):
+                for idx, cv in zip(range(n_subsamples), results[cell_type], strict=False):
                     results["full_results"]["idx"].extend([idx] * folds)
                     results["full_results"]["augur_score"].extend(cv["test_augur_score"])
                     results["full_results"]["folds"].extend(range(folds))
                 results["full_results"]["cell_type"].extend([cell_type] * folds * n_subsamples)
         # make sure one cell type worked
         if len(results) <= 2:
             print("[bold red]No cells types had more than min_cells needed. Please adjust data or min_cells parameter.")
@@ -865,47 +875,50 @@
         # compare available cell types
         cell_types = (
             set(augur_results1["summary_metrics"].columns)
             & set(augur_results2["summary_metrics"].columns)
             & set(permuted_results1["summary_metrics"].columns)
             & set(permuted_results2["summary_metrics"].columns)
         )
+
+        cell_types_list = list(cell_types)
+
         # mean augur scores
         augur_score1 = (
             augur_results1["summary_metrics"]
-            .loc["mean_augur_score", cell_types]
+            .loc["mean_augur_score", cell_types_list]
             .reset_index()
             .rename(columns={"index": "cell_type"})
         )
         augur_score2 = (
             augur_results2["summary_metrics"]
-            .loc["mean_augur_score", cell_types]
+            .loc["mean_augur_score", cell_types_list]
             .reset_index()
             .rename(columns={"index": "cell_type"})
         )
 
         # mean permuted scores over cross validation runs
         permuted_cv_augur1 = (
-            permuted_results1["full_results"][permuted_results1["full_results"]["cell_type"].isin(cell_types)]
+            permuted_results1["full_results"][permuted_results1["full_results"]["cell_type"].isin(cell_types_list)]
             .groupby(["cell_type", "idx"], as_index=False)
             .mean()
         )
         permuted_cv_augur2 = (
-            permuted_results2["full_results"][permuted_results2["full_results"]["cell_type"].isin(cell_types)]
+            permuted_results2["full_results"][permuted_results2["full_results"]["cell_type"].isin(cell_types_list)]
             .groupby(["cell_type", "idx"], as_index=False)
             .mean()
         )
 
         sampled_permuted_cv_augur1 = []
         sampled_permuted_cv_augur2 = []
 
         # draw mean aucs for permute1 and permute2
         for celltype in permuted_cv_augur1["cell_type"].unique():
             df1 = permuted_cv_augur1[permuted_cv_augur1["cell_type"] == celltype]
-            df2 = permuted_cv_augur2[permuted_cv_augur1["cell_type"] == celltype]
+            df2 = permuted_cv_augur2[permuted_cv_augur2["cell_type"] == celltype]
             for permutation_idx in range(n_permutations):
                 # subsample
                 sample1 = df1.sample(n=n_subsamples, random_state=permutation_idx, axis="index")
                 sampled_permuted_cv_augur1.append(
                     pd.DataFrame(
                         {
                             "cell_type": [celltype],
@@ -957,7 +970,292 @@
         # calculate pvalues
         delta["pval"] = np.minimum(
             2 * (delta["b"] + 1) / (delta["m"] + 1), 2 * (delta["m"] - delta["b"] + 1) / (delta["m"] + 1)
         )
         delta["padj"] = fdrcorrection(delta["pval"])[1]
 
         return delta
+
+    def plot_dp_scatter(
+        self,
+        results: pd.DataFrame,
+        top_n: int = None,
+        return_fig: bool | None = None,
+        ax: Axes = None,
+        show: bool | None = None,
+        save: str | bool | None = None,
+    ) -> Axes | Figure | None:
+        """Plot scatterplot of differential prioritization.
+
+        Args:
+            results: Results after running differential prioritization.
+            top_n: optionally, the number of top prioritized cell types to label in the plot
+            ax: optionally, axes used to draw plot
+
+        Returns:
+            Axes of the plot.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.bhattacherjee()
+            >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
+
+            >>> data_15 = ag_rfc.load(adata, condition_label="Maintenance_Cocaine", treatment_label="withdraw_15d_Cocaine")
+            >>> adata_15, results_15 = ag_rfc.predict(data_15, random_state=None, n_threads=4)
+            >>> adata_15_permute, results_15_permute = ag_rfc.predict(data_15, augur_mode="permute", n_subsamples=100, random_state=None, n_threads=4)
+
+            >>> data_48 = ag_rfc.load(adata, condition_label="Maintenance_Cocaine", treatment_label="withdraw_48h_Cocaine")
+            >>> adata_48, results_48 = ag_rfc.predict(data_48, random_state=None, n_threads=4)
+            >>> adata_48_permute, results_48_permute = ag_rfc.predict(data_48, augur_mode="permute", n_subsamples=100, random_state=None, n_threads=4)
+
+            >>> pvals = ag_rfc.predict_differential_prioritization(augur_results1=results_15, augur_results2=results_48, \
+                permuted_results1=results_15_permute, permuted_results2=results_48_permute)
+            >>> ag_rfc.plot_dp_scatter(pvals)
+
+        Preview:
+            .. image:: /_static/docstring_previews/augur_dp_scatter.png
+        """
+        x = results["mean_augur_score1"]
+        y = results["mean_augur_score2"]
+
+        if ax is None:
+            fig, ax = plt.subplots()
+        scatter = ax.scatter(x, y, c=results.z, cmap="Greens")
+
+        # adding optional labels
+        top_n_index = results.sort_values(by="pval").index[:top_n]
+        for idx in top_n_index:
+            ax.annotate(
+                results.loc[idx, "cell_type"],
+                (results.loc[idx, "mean_augur_score1"], results.loc[idx, "mean_augur_score2"]),
+            )
+
+        # add diagonal
+        limits = max(ax.get_xlim(), ax.get_ylim())
+        (_,) = ax.plot(limits, limits, ls="--", c=".3")
+
+        # formatting and details
+        plt.xlabel("Augur scores 1")
+        plt.ylabel("Augur scores 2")
+        legend1 = ax.legend(*scatter.legend_elements(), loc="center left", title="z-scores", bbox_to_anchor=(1, 0.5))
+        ax.add_artist(legend1)
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return ax
+        return None
+
+    def plot_important_features(
+        self,
+        data: dict[str, Any],
+        key: str = "augurpy_results",
+        top_n: int = 10,
+        return_fig: bool | None = None,
+        ax: Axes = None,
+        show: bool | None = None,
+        save: str | bool | None = None,
+    ) -> Axes | None:
+        """Plot a lollipop plot of the n features with largest feature importances.
+
+        Args:
+            results: results after running `predict()` as dictionary or the AnnData object.
+            key: Key in the AnnData object of the results
+            top_n: n number feature importance values to plot. Default is 10.
+            ax: optionally, axes used to draw plot
+            return_figure: if `True` returns figure of the plot, default is `False`
+
+        Returns:
+            Axes of the plot.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.sc_sim_augur()
+            >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
+            >>> loaded_data = ag_rfc.load(adata)
+            >>> v_adata, v_results = ag_rfc.predict(
+            ...     loaded_data, subsample_size=20, select_variance_features=True, n_threads=4
+            ... )
+            >>> ag_rfc.plot_important_features(v_results)
+
+        Preview:
+            .. image:: /_static/docstring_previews/augur_important_features.png
+        """
+        if isinstance(data, AnnData):
+            results = data.uns[key]
+        else:
+            results = data
+        n_features = (
+            results["feature_importances"]
+            .groupby("genes", as_index=False)
+            .feature_importances.mean()
+            .sort_values(by="feature_importances")[-top_n:]
+        )
+
+        if ax is None:
+            fig, ax = plt.subplots()
+        y_axes_range = range(1, top_n + 1)
+        ax.hlines(
+            y_axes_range,
+            xmin=0,
+            xmax=n_features["feature_importances"],
+        )
+
+        ax.plot(n_features["feature_importances"], y_axes_range, "o")
+
+        plt.xlabel("Mean Feature Importance")
+        plt.ylabel("Gene")
+        plt.yticks(y_axes_range, n_features["genes"])
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return ax
+        return None
+
+    def plot_lollipop(
+        self,
+        data: dict[str, Any],
+        key: str = "augurpy_results",
+        return_fig: bool | None = None,
+        ax: Axes = None,
+        show: bool | None = None,
+        save: str | bool | None = None,
+    ) -> Axes | Figure | None:
+        """Plot a lollipop plot of the mean augur values.
+
+        Args:
+            results: results after running `predict()` as dictionary or the AnnData object.
+            key: Key in the AnnData object of the results
+            ax: optionally, axes used to draw plot
+            return_figure: if `True` returns figure of the plot
+
+        Returns:
+            Axes of the plot.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.sc_sim_augur()
+            >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
+            >>> loaded_data = ag_rfc.load(adata)
+            >>> v_adata, v_results = ag_rfc.predict(
+            ...     loaded_data, subsample_size=20, select_variance_features=True, n_threads=4
+            ... )
+            >>> ag_rfc.plot_lollipop(v_results)
+
+        Preview:
+            .. image:: /_static/docstring_previews/augur_lollipop.png
+        """
+        if isinstance(data, AnnData):
+            results = data.uns[key]
+        else:
+            results = data
+        if ax is None:
+            fig, ax = plt.subplots()
+        y_axes_range = range(1, len(results["summary_metrics"].columns) + 1)
+        ax.hlines(
+            y_axes_range,
+            xmin=0,
+            xmax=results["summary_metrics"].sort_values("mean_augur_score", axis=1).loc["mean_augur_score"],
+        )
+
+        ax.plot(
+            results["summary_metrics"].sort_values("mean_augur_score", axis=1).loc["mean_augur_score"],
+            y_axes_range,
+            "o",
+        )
+
+        plt.xlabel("Mean Augur Score")
+        plt.ylabel("Cell Type")
+        plt.yticks(y_axes_range, results["summary_metrics"].sort_values("mean_augur_score", axis=1).columns)
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return ax
+        return None
+
+    def plot_scatterplot(
+        self,
+        results1: dict[str, Any],
+        results2: dict[str, Any],
+        top_n: int = None,
+        return_fig: bool | None = None,
+        show: bool | None = None,
+        save: str | bool | None = None,
+    ) -> Axes | Figure | None:
+        """Create scatterplot with two augur results.
+
+        Args:
+            results1: results after running `predict()`
+            results2: results after running `predict()`
+            top_n: optionally, the number of top prioritized cell types to label in the plot
+            return_figure: if `True` returns figure of the plot
+
+        Returns:
+            Axes of the plot.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.sc_sim_augur()
+            >>> ag_rfc = pt.tl.Augur("random_forest_classifier")
+            >>> loaded_data = ag_rfc.load(adata)
+            >>> h_adata, h_results = ag_rfc.predict(loaded_data, subsample_size=20, n_threads=4)
+            >>> v_adata, v_results = ag_rfc.predict(
+            ...     loaded_data, subsample_size=20, select_variance_features=True, n_threads=4
+            ... )
+            >>> ag_rfc.plot_scatterplot(v_results, h_results)
+
+        Preview:
+            .. image:: /_static/docstring_previews/augur_scatterplot.png
+        """
+        cell_types = results1["summary_metrics"].columns
+
+        fig, ax = plt.subplots()
+        ax.scatter(
+            results1["summary_metrics"].loc["mean_augur_score", cell_types],
+            results2["summary_metrics"].loc["mean_augur_score", cell_types],
+        )
+
+        # adding optional labels
+        top_n_cell_types = (
+            (results1["summary_metrics"].loc["mean_augur_score"] - results2["summary_metrics"].loc["mean_augur_score"])
+            .sort_values(ascending=False)
+            .index[:top_n]
+        )
+        for txt in top_n_cell_types:
+            ax.annotate(
+                txt,
+                (
+                    results1["summary_metrics"].loc["mean_augur_score", txt],
+                    results2["summary_metrics"].loc["mean_augur_score", txt],
+                ),
+            )
+
+        # adding diagonal
+        limits = max(ax.get_xlim(), ax.get_ylim())
+        (diag_line,) = ax.plot(limits, limits, ls="--", c=".3")
+
+        plt.xlabel("Augur scores 1")
+        plt.ylabel("Augur scores 2")
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return ax
+        return None
```

### Comparing `pertpy-0.6.0/pertpy/tools/_cinemaot.py` & `pertpy-0.7.0/pertpy/tools/_cinemaot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
 import scipy.stats as ss
+import seaborn as sns
 import sklearn.metrics
 from ott.geometry import pointcloud
 from ott.problems.linear import linear_problem
 from ott.solvers.linear import sinkhorn, sinkhorn_lr
+from scanpy.plotting import _utils
 from scipy.sparse import issparse
 from sklearn.decomposition import FastICA
 from sklearn.linear_model import LinearRegression
 from sklearn.neighbors import NearestNeighbors
 
 if TYPE_CHECKING:
     from anndata import AnnData
+    from matplotlib.axes import Axes
     from statsmodels.tools.typing import ArrayLike
 
 
 class Cinemaot:
     """CINEMA-OT is a causal framework for perturbation effect analysis to identify individual treatment effects and synergy."""
 
     def __init__(self):
@@ -63,14 +67,22 @@
             preweight_label: The annotated label (e.g. cell type) that is used to assign weights for treated
                              and control cells to balance across the label. Helps overcome the differential abundance issue.
 
         Returns:
             Returns an AnnData object that contains the single-cell level treatment effect as de.X and the
             corresponding low dimensional embedding in de.obsm['X_embedding'], and optional matching matrix
             stored in the de.obsm['ot']. Also puts the confounding variation in adata.obsm[cf_rep].
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> model = pt.tl.Cinemaot()
+            >>> out_adata = model.causaleffect(
+            >>>         adata, pert_key="perturbation", control="No stimulation", return_matching=True,
+            >>>         thres=0.5, smoothness=1e-5, eps=1e-3, solver="Sinkhorn", preweight_label="cell_type0528")
         """
         available_solvers = ["Sinkhorn", "LRSinkhorn"]
         if solver not in available_solvers:
             raise ValueError(f"solver = {solver} is not one of the supported solvers:" f" {available_solvers}")
 
         if dim is None:
             dim = self.get_dim(adata, use_rep=use_rep)
@@ -221,14 +233,22 @@
             solver: Either "Sinkhorn" or "LRSinkhorn". The ott-jax solver used.
             resolution: the clustering resolution used in the sampling phase.
 
         Returns:
             Returns an anndata object that contains the single-cell level treatment effect as de.X and the
             corresponding low dimensional embedding in de.obsm['X_embedding'], and optional matching matrix
             stored in the de.obsm['ot']. Also puts the confounding variation in adata.obsm[cf_rep].
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> model = pt.tl.Cinemaot()
+            >>> ad, de = model.causaleffect_weighted(
+            >>>              adata, pert_key="perturbation", control="No stimulation", return_matching=True,
+            >>>              thres=0.5, smoothness=1e-5, eps=1e-3, solver="Sinkhorn")
         """
         available_solvers = ["Sinkhorn", "LRSinkhorn"]
         assert solver in available_solvers, (
             f"solver = {solver} is not one of the supported solvers:" f" {available_solvers}"
         )
 
         if dim is None:
@@ -284,14 +304,24 @@
             assign_cf: If a str is passed, a label in adata.obs instead of confounder Leiden label is used.
             cf_resolution: The leiden clustering resolution for the confounder.
             de_resolution: The leiden clustering resolution for the differential response.
             use_raw: If true, use adata.raw.X to aggregate the pseudobulk profiles. Otherwise use adata.X.
 
         Returns:
             Returns an anndata object that contains aggregated pseudobulk profiles and associated metadata.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> model = pt.tl.Cinemaot()
+            >>> de = model.causaleffect(
+            >>>         adata, pert_key="perturbation", control="No stimulation", return_matching=True, thres=0.5,
+            >>>         smoothness=1e-5, eps=1e-3, solver="Sinkhorn", preweight_label="cell_type0528")
+            >>> adata_pb = model.generate_pseudobulk(
+            >>>         adata, de, pert_key="perturbation", control="No stimulation", label_list=None)
         """
         sc.pp.neighbors(de, use_rep=de_rep)
         sc.tl.leiden(de, resolution=de_resolution)
         if use_raw:
             if issparse(adata.raw.X):
                 df = pd.DataFrame(adata.raw.X.toarray(), columns=adata.raw.var_names, index=adata.raw.obs_names)
             else:
@@ -332,14 +362,20 @@
         Args:
             adata: The annotated data object.
             c: the parameter regarding the quadratic variance distribution. c=0 means Poisson count matrices.
             use_rep: the embedding used to give a upper bound for the estimated rank.
 
         Returns:
             Returns the estimated dimension number.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> model = pt.tl.Cinemaot()
+            >>> dim = model.get_dim(adata)
         """
         sk = SinkhornKnopp()
         if issparse(adata.raw.X):
             data = adata.raw.X.toarray()
         else:
             data = adata.raw.X
         vm = (1e-3 + data + c * data * data) / (1 + c)
@@ -365,14 +401,20 @@
             c: the parameter regarding the quadratic variance distribution. c=0 means Poisson count matrices.
             use_rep: the embedding used to give a upper bound for the estimated rank.
             k: the number of neighbors used in the k-NN matching phase.
             resolution: the clustering resolution used in the sampling phase.
 
         Returns:
             Returns the indices.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> model = pt.tl.Cinemaot()
+            >>> idx = model.get_weightidx(adata, pert_key="perturbation", control="No stimulation")
         """
         adata_ = adata.copy()
         X_pca1 = adata_.obsm[use_rep][adata_.obs[pert_key] == control, :]
         X_pca2 = adata_.obsm[use_rep][adata_.obs[pert_key] != control, :]
         nbrs = NearestNeighbors(n_neighbors=k, algorithm="ball_tree").fit(X_pca1)
         mixscape_pca = adata.obsm[use_rep].copy()
         mixscapematrix = nbrs.kneighbors_graph(X_pca2).toarray()
@@ -481,14 +523,23 @@
             eps: Tolerate error of the optimal transport.
             preweight_label: the annotated label (e.g. cell type) that is used to assign weights for treated
                 and control cells to balance across the label. Helps overcome the differential abundance issue.
             **kwargs: other parameters that can be passed to Cinemaot.causaleffect()
 
         Returns:
             Returns an AnnData object that contains the single-cell level synergy matrix de.X and the embedding.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.dong_2023()
+            >>> sc.pp.pca(adata)
+            >>> model = pt.tl.Cinemaot()
+            >>> combo = model.synergy(adata, pert_key='perturbation', base='No stimulation', A='IFNb', B='IFNg',
+            >>>                   AB='IFNb+ IFNg', thres=0.5, smoothness=1e-5, eps=1e-3, solver='Sinkhorn')
+
         """
         adata1 = adata[adata.obs[pert_key].isin([base, A]), :].copy()
         adata2 = adata[adata.obs[pert_key].isin([B, AB]), :].copy()
         adata_link = adata[adata.obs[pert_key].isin([base, B]), :].copy()
         de1 = self.causaleffect(
             adata1,
             pert_key=pert_key,
@@ -548,14 +599,20 @@
             pert_key: The column  of `.obs` with perturbation categories, should also contain `control`.
             control: Control category from the `pert_key` column.
             cf_rep: the place to put the confounder embedding in the original adata.obsm.
             use_raw: If true, use adata.raw.X to aggregate the pseudobulk profiles. Otherwise use adata.X.
 
         Returns:
             Returns the confounder effect (c_effect) and the residual effect (s_effect).
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> model = pt.tl.Cinemaot()
+            >>> c_effect, s_effect = model.attribution_scatter(adata, pert_key="perturbation", control="No stimulation")
         """
         cf = adata.obsm[cf_rep]
         if use_raw:
             if issparse(adata.X):
                 Y0 = adata.raw.X.toarray()[adata.obs[pert_key] == control, :]
                 Y1 = adata.raw.X.toarray()[adata.obs[pert_key] != control, :]
             else:
@@ -578,14 +635,92 @@
         c1 = ols1.predict(X1) - np.mean(ols1.predict(X1), axis=0)
         e0 = Y0 - ols0.predict(X0)
         e1 = Y1 - ols1.predict(X1)
         c_effect = (np.linalg.norm(c1, axis=0) + 1e-6) / (np.linalg.norm(c0, axis=0) + 1e-6)
         s_effect = (np.linalg.norm(e1, axis=0) + 1e-6) / (np.linalg.norm(e0, axis=0) + 1e-6)
         return c_effect, s_effect
 
+    def plot_vis_matching(
+        self,
+        adata: AnnData,
+        de: AnnData,
+        pert_key: str,
+        control: str,
+        de_label: str,
+        source_label: str,
+        matching_rep: str = "ot",
+        resolution: float = 0.5,
+        normalize: str = "col",
+        title: str = "CINEMA-OT matching matrix",
+        min_val: float = 0.01,
+        show: bool = True,
+        save: str | None = None,
+        ax: Axes | None = None,
+        **kwargs,
+    ) -> None:
+        """Visualize the CINEMA-OT matching matrix.
+
+        Args:
+            adata: the original anndata after running cinemaot.causaleffect or cinemaot.causaleffect_weighted.
+            de: The anndata output from Cinemaot.causaleffect() or Cinemaot.causaleffect_weighted().
+            pert_key: The column  of `.obs` with perturbation categories, should also contain `control`.
+            control: Control category from the `pert_key` column.
+            de_label: the label for differential response. If none, use leiden cluster labels at resolution 1.0.
+            source_label: the confounder / cell type label.
+            matching_rep: the place that stores the matching matrix. default de.obsm['ot'].
+            normalize: normalize the coarse-grained matching matrix by row / column.
+            title: the title for the figure.
+            min_val: The min value to truncate the matching matrix.
+            show: Show the plot, do not return axis.
+            save: If `True` or a `str`, save the figure. A string is appended to the default filename.
+                Infer the filetype if ending on {`'.pdf'`, `'.png'`, `'.svg'`}.
+            **kwargs: Other parameters to input for seaborn.heatmap.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> adata = pt.dt.cinemaot_example()
+            >>> cot = pt.tl.Cinemaot()
+            >>> de = cot.causaleffect(
+            >>>         adata, pert_key="perturbation", control="No stimulation", return_matching=True,
+            >>>         thres=0.5, smoothness=1e-5, eps=1e-3, solver="Sinkhorn", preweight_label="cell_type0528")
+            >>> cot.plot_vis_matching(
+            >>>         adata, de, pert_key="perturbation",control="No stimulation", de_label=None, source_label="cell_type0528")
+        """
+        adata_ = adata[adata.obs[pert_key] == control]
+
+        df = pd.DataFrame(de.obsm[matching_rep])
+        if de_label is None:
+            de_label = "leiden"
+            sc.pp.neighbors(de, use_rep="X_embedding")
+            sc.tl.leiden(de, resolution=resolution)
+        df["de_label"] = de.obs[de_label].astype(str).values
+        df["de_label"] = "Response " + df["de_label"]
+        df = df.groupby("de_label").sum().T
+        df["source_label"] = adata_.obs[source_label].astype(str).values
+        df = df.groupby("source_label").sum()
+
+        if normalize == "col":
+            df = df / df.sum(axis=0)
+        else:
+            df = (df.T / df.sum(axis=1)).T
+        df = df.clip(lower=min_val) - min_val
+        if normalize == "col":
+            df = df / df.sum(axis=0)
+        else:
+            df = (df.T / df.sum(axis=1)).T
+
+        g = sns.heatmap(df, annot=True, ax=ax, **kwargs)
+        plt.title(title)
+        _utils.savefig_or_show("matching_heatmap", show=show, save=save)
+        if not show:
+            if ax is not None:
+                return ax
+            else:
+                return g
+
 
 class Xi:
     """
     A fast implementation of cross-rank dependence metric used in CINEMA-OT.
 
     """
 
@@ -606,15 +741,15 @@
         len_x = len(self.x)
         rng = np.random.default_rng()
         randomized_indices = rng.choice(np.arange(len_x), len_x, replace=False)
         randomized = [self.x[idx] for idx in randomized_indices]
         # same as pandas rank method 'first'
         rankdata = ss.rankdata(randomized, method="ordinal")
         # Reindexing based on pairs of indices before and after
-        unrandomized = [rankdata[j] for i, j in sorted(zip(randomized_indices, range(len_x)))]
+        unrandomized = [rankdata[j] for i, j in sorted(zip(randomized_indices, range(len_x), strict=False))]
         return unrandomized
 
     @property
     def y_rank_max(self):
         # f[i] is number of j s.t. y[j] <= y[i], divided by n.
         return ss.rankdata(self.y, method="max") / self.sample_size
 
@@ -644,14 +779,15 @@
             np.mean(
                 np.abs(
                     [
                         x - y
                         for x, y in zip(
                             x1,
                             x2,
+                            strict=False,
                         )
                     ]
                 )
             )
             * (self.sample_size - 1)
             / (2 * self.sample_size)
         )
@@ -690,21 +826,24 @@
         # If there are ties, and the theoretical method is to be used for calculation P-values:
         # The following steps calculate the theoretical variance in the presence of ties:
         sorted_ordered_x_rank = sorted(self.x_rank_max_ordered)
 
         ind = [i + 1 for i in range(self.sample_size)]
         ind2 = [2 * self.sample_size - 2 * ind[i - 1] + 1 for i in ind]
 
-        a = np.mean([i * j * j for i, j in zip(ind2, sorted_ordered_x_rank)]) / self.sample_size
+        a = np.mean([i * j * j for i, j in zip(ind2, sorted_ordered_x_rank, strict=False)]) / self.sample_size
 
-        c = np.mean([i * j for i, j in zip(ind2, sorted_ordered_x_rank)]) / self.sample_size
+        c = np.mean([i * j for i, j in zip(ind2, sorted_ordered_x_rank, strict=False)]) / self.sample_size
 
         cq = np.cumsum(sorted_ordered_x_rank)
 
-        m = [(i + (self.sample_size - j) * k) / self.sample_size for i, j, k in zip(cq, ind, sorted_ordered_x_rank)]
+        m = [
+            (i + (self.sample_size - j) * k) / self.sample_size
+            for i, j, k in zip(cq, ind, sorted_ordered_x_rank, strict=False)
+        ]
 
         b = np.mean([np.square(i) for i in m])
         v = (a - 2 * b + np.square(c)) / np.square(self.inverse_g_mean)
 
         return 1 - ss.norm.cdf(np.sqrt(self.sample_size) * self.correlation / np.sqrt(v))
```

### Comparing `pertpy-0.6.0/pertpy/tools/_dialogue.py` & `pertpy-0.7.0/pertpy/tools/_dialogue.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from __future__ import annotations
 
 import itertools
 from collections import defaultdict
-from typing import Any, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
 import anndata as ad
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import scanpy as sc
-import scipy.sparse as sp
+import seaborn as sns
 import statsmodels.formula.api as smf
 import statsmodels.stats.multitest as ssm
 from anndata import AnnData
 from pandas import DataFrame
 from rich import print
 from rich.console import Group
 from rich.live import Live
 from rich.progress import BarColumn, Progress, SpinnerColumn, TaskProgressColumn, TextColumn
 from scipy import stats
 from scipy.optimize import nnls
+from seaborn import PairGrid
 from sklearn.linear_model import LinearRegression
 from sparsecca import lp_pmd, multicca_permute, multicca_pmd
 from statsmodels.sandbox.stats.multicomp import multipletests
 
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from matplotlib.figure import Figure
+
 
 class Dialogue:
     """Python implementation of DIALOGUE"""
 
     def __init__(self, sample_id: str, celltype_key: str, n_counts_key: str, n_mpcs: int):
         """Constructor for Dialogue.
 
@@ -49,31 +55,30 @@
     def _get_pseudobulks(
         self, adata: AnnData, groupby: str, strategy: Literal["median", "mean"] = "median"
     ) -> pd.DataFrame:
         """Return cell-averaged data by groupby.
 
         Copied from `https://github.com/schillerlab/sc-toolbox/blob/397e80dc5e8fb8017b75f6c3fa634a1e1213d484/sc_toolbox/tools/__init__.py#L458`
 
-        # TODO: Replace with decoupler's implementation
-
         Args:
             groupby: The key to groupby for pseudobulks
             strategy: The pseudobulking strategy. One of "median" or "mean"
 
         Returns:
             A Pandas DataFrame of pseudobulk counts
         """
+        # TODO: Replace with decoupler's implementation
         pseudobulk = {"Genes": adata.var_names.values}
 
         for category in adata.obs.loc[:, groupby].cat.categories:
             temp = adata.obs.loc[:, groupby] == category
             if strategy == "median":
-                pseudobulk[category] = adata[temp].X.median(axis=0).A1
+                pseudobulk[category] = adata[temp].X.median(axis=0)
             elif strategy == "mean":
-                pseudobulk[category] = adata[temp].X.mean(axis=0).A1
+                pseudobulk[category] = adata[temp].X.mean(axis=0)
 
         pseudobulk = pd.DataFrame(pseudobulk).set_index("Genes")
 
         return pseudobulk
 
     def _pseudobulk_pca(self, adata: AnnData, groupby: str, n_components: int = 50) -> pd.DataFrame:
         """Return cell-averaged PCA components.
@@ -97,26 +102,24 @@
         aggr = pd.DataFrame(aggr)
 
         return aggr
 
     def _scale_data(self, pseudobulks: pd.DataFrame, normalize: bool = True) -> np.ndarray:
         """Row-wise mean center and scale by the standard deviation.
 
-        TODO: the `scale` function we implemented to match the R `scale` fn should already contain this functionality.
-
         Args:
             pseudobulks: The pseudobulk PCA components.
             normalize: Whether to mimic DIALOGUE behavior or not.
 
         Returns:
             The scaled count matrix.
         """
+        # TODO: the `scale` function we implemented to match the R `scale` fn should already contain this functionality.
         # DIALOGUE doesn't scale the data before passing to multicca, unlike what is recommended by sparsecca.
         # However, performing this scaling _does_ increase overall correlation of the end result
-        # WHEN SAMPLE ORDER AND DIALOGUE2+3 PROCESSING IS IGNORED.
         if normalize:
             return pseudobulks.to_numpy()
         else:
             return ((pseudobulks - pseudobulks.mean()) / pseudobulks.std()).to_numpy()
 
     def _concat_adata_mcp_scores(
         self, adata: AnnData, ct_subs: dict[str, AnnData], mcp_scores: dict[str, np.ndarray], celltype_key: str
@@ -309,21 +312,21 @@
             top_genes[mcp_name + suffix] = sorted(genes[i] for i in range(len(zscores)) if zscores[i] <= threshold)
 
         return top_genes
 
     def _apply_HLM_per_MCP_for_one_pair(
         self,
         mcp_name: str,
-        scores_df: dict,
+        scores_df: pd.DataFrame,
         ct_data: AnnData,
         tme: pd.DataFrame,
         sig: dict,
         n_counts: str,
         formula: str,
-        confounder: str,
+        confounder: str | None,
     ) -> tuple[pd.DataFrame, dict[str, Any]]:
         """Applies hierarchical modeling for a single MCP.
 
         TODO: separate the sig calculation so that this whole function is more tractable
 
         Args:
             mcp_name: The name of the MCP to model.
@@ -336,15 +339,15 @@
             confounder: Any modeling confounders.
 
         Returns:
             The HLM results together with significant up/downregulated genes per MCP
         """
         HLM_result = self._mixed_effects(
             scores=scores_df[[mcp_name]],
-            x_labels=ct_data.obs[[n_counts, confounder]],
+            x_labels=ct_data.obs[[n_counts, confounder]] if confounder else ct_data.obs[[n_counts]],
             tme=tme,
             genes_in_mcp=list(sig[mcp_name]["up"]) + list(sig[mcp_name]["down"]),
             formula=formula,
             confounder=confounder,
         )
 
         HLM_result["up"] = [gene in sig[mcp_name]["up"] for gene in HLM_result.index]
@@ -363,15 +366,15 @@
             lr = LinearRegression().fit(X.reshape(-1, 1), y_sub)
             pred = lr.predict(X.reshape(-1, 1))
             resid.append(y_sub - pred)
 
         return np.array(resid)
 
     def _iterative_nnls(self, A_orig: np.ndarray, y_orig: np.ndarray, feature_ranks: list[int], n_iter: int = 1000):
-        """Solves non-negative least squares separately for different feature categories.
+        """Solves non-negative least-squares separately for different feature categories.
 
         Mimics DLG.iterative.nnls.
         Variables are notated according to:
 
             `argmin|Ax - y|`
 
         Args:
@@ -394,15 +397,15 @@
         insig_mask = feature_ranks < sig_ranks[-1]  # type: ignore # TODO: rename variable after better understanding
         if sum(insig_mask) >= 5:  # such as genes with 0 rank, or those below 1/3
             masks.append(insig_mask)
             sig_ranks.append("insig")  # type: ignore
 
         x_final = np.zeros(A_orig.shape[0])
         Ax = np.zeros(A_orig.shape[1])
-        for _, mask in zip(sig_ranks, masks):
+        for _, mask in zip(sig_ranks, masks, strict=False):
             A = A_orig[mask].T
             coef_nnls, _ = nnls(A, y, maxiter=n_iter)
             y = y - A @ coef_nnls  # residuals
             Ax += A @ coef_nnls
             x_final[mask] = coef_nnls
 
         return x_final
@@ -512,16 +515,16 @@
             cca_sig_unformatted = self._get_top_elements(  # 3 up, 3 dn, for each mcp
                 pd.DataFrame(C1.T, index=top_cor_genes_flattened), max_length=max_genes, min_threshold=0.05
             )
 
             # TODO: probably format the up and down within get_top_elements
             cca_sig: dict[str, Any] = defaultdict(dict)
             for i in range(0, int(len(cca_sig_unformatted) / 2)):
-                cca_sig[f"MCP{i + 1}"]["up"] = cca_sig_unformatted[i * 2]
-                cca_sig[f"MCP{i + 1}"]["down"] = cca_sig_unformatted[i * 2 + 1]
+                cca_sig[f"MCP{i}"]["up"] = cca_sig_unformatted[i * 2]
+                cca_sig[f"MCP{i}"]["down"] = cca_sig_unformatted[i * 2 + 1]
 
             cca_sig = dict(cca_sig)
             cca_sig_results[ct] = cca_sig
 
             # This is basically DIALOGUE 3 now
             pre_r_scores = {
                 ct: ct_subs[ct].obsm["X_pca"][:, :50] @ ws_dict[ct]
@@ -551,15 +554,15 @@
                 # scores = zscores.T @ coef
                 # TODO: The line below has to be new_mcp_scores.append(scores) after we implemented the NF value caluation
                 scores.append(zscores)
             new_mcp_scores[ct] = scores
 
         return cca_sig_results, new_mcp_scores
 
-    def load(
+    def _load(
         self,
         adata: AnnData,
         ct_order: list[str],
         agg_pca: bool = True,
         normalize: bool = True,
     ) -> tuple[list, dict]:
         """Separates cell into AnnDatas by celltype_key and creates the multifactor PMD input.
@@ -570,24 +573,14 @@
             adata: AnnData object generate celltype objects for
             ct_order: The order of cell types
             agg_pca: Whether to aggregate pseudobulks with PCA or not. Defaults to True.
             normalize: Whether to mimic DIALOGUE behavior or not. Defaults to True.
 
         Returns:
             A celltype_label:array dictionary.
-
-        Examples:
-            >>> import pertpy as pt
-            >>> import scanpy as sc
-            >>> adata = pt.dt.dialogue_example()
-            >>> sc.pp.pca(adata)
-            >>> dl = pt.tl.Dialogue(sample_id = "clinical.status", celltype_key = "cell.subtypes", \
-                n_counts_key = "nCount_RNA", n_mpcs = 3)
-            >>> cell_types = adata.obs[dl.celltype_key].astype("category").cat.categories
-            >>> mcca_in, ct_subs = dl.load(adata, ct_order=cell_types)
         """
         ct_subs = {ct: adata[adata.obs[self.celltype_key] == ct].copy() for ct in ct_order}
         fn = self._pseudobulk_pca if agg_pca else self._get_pseudobulks
         ct_aggr = {ct: fn(ad, self.sample_id) for ct, ad in ct_subs.items()}  # type: ignore
 
         # TODO: implement check (as in https://github.com/livnatje/DIALOGUE/blob/55da9be0a9bf2fcd360d9e11f63e30d041ec4318/R/DIALOGUE.main.R#L114-L119)
         # that there are at least 5 share samples here
@@ -627,27 +620,27 @@
             MCP scores  # TODO this requires more detail
 
         Examples:
             >>> import pertpy as pt
             >>> import scanpy as sc
             >>> adata = pt.dt.dialogue_example()
             >>> sc.pp.pca(adata)
-            >>> dl = pt.tl.Dialogue(sample_id = "clinical.status", celltype_key = "cell.subtypes", \
-                n_counts_key = "nCount_RNA", n_mpcs = 3)
+            >>> dl = pt.tl.Dialogue(
+            ...     sample_id="clinical.status", celltype_key="cell.subtypes", n_counts_key="nCount_RNA", n_mpcs=3
+            ... )
             >>> adata, mcps, ws, ct_subs = dl.calculate_multifactor_PMD(adata, normalize=True)
         """
-        # IMPORTANT NOTE: the order in which matrices are passed to multicca matters. As such,
-        # it is important here that to obtain the same result as in R, we pass the matrices in
-        # in the same order.
+        # IMPORTANT NOTE: the order in which matrices are passed to multicca matters.
+        # As such, it is important here that to obtain the same result as in R, we pass the matrices in the same order.
         if ct_order is not None:
             cell_types = ct_order
         else:
             ct_order = cell_types = adata.obs[self.celltype_key].astype("category").cat.categories
 
-        mcca_in, ct_subs = self.load(adata, ct_order=cell_types, agg_pca=agg_pca, normalize=normalize)
+        mcca_in, ct_subs = self._load(adata, ct_order=cell_types, agg_pca=agg_pca, normalize=normalize)
 
         n_samples = mcca_in[0].shape[1]
         if penalties is None:
             penalties = multicca_permute(
                 mcca_in, penalties=np.sqrt(n_samples) / 2, nperms=10, niter=50, standardize=True
             )["bestpenalties"]
         else:
@@ -681,53 +674,54 @@
         return adata, mcp_scores, ws_dict, ct_subs
 
     def multilevel_modeling(
         self,
         ct_subs: dict,
         mcp_scores: dict,
         ws_dict: dict,
-        confounder: str,
+        confounder: str | None,
         formula: str = None,
     ):
         """Runs the multilevel modeling step to match genes to MCPs and generate p-values for MCPs.
 
         Args:
             ct_subs: The DIALOGUE cell type objects.
             mcp_scores: The determined MCP scores from the PMD step.
             confounder: Any modeling confounders.
             formula: The hierarchical modeling formula. Defaults to y ~ x + n_counts.
 
         Returns:
             A Pandas DataFrame containing:
             - for each mcp: HLM_result_1, HLM_result_2, sig_genes_1, sig_genes_2
             - merged HLM_result_1, HLM_result_2, sig_genes_1, sig_genes_2 of all mcps
-            TODO: Describe both returns
 
         Examples:
             >>> import pertpy as pt
             >>> import scanpy as sc
             >>> adata = pt.dt.dialogue_example()
             >>> sc.pp.pca(adata)
             >>> dl = pt.tl.Dialogue(sample_id = "clinical.status", celltype_key = "cell.subtypes", \
                 n_counts_key = "nCount_RNA", n_mpcs = 3)
             >>> adata, mcps, ws, ct_subs = dl.calculate_multifactor_PMD(adata, normalize=True)
             >>> all_results, new_mcps = dl.multilevel_modeling(ct_subs=ct_subs, mcp_scores=mcps, ws_dict=ws, \
                 confounder="gender")
         """
-        # all possible pairs of cell types with out pairing same cell type
+        # TODO the returns of the function better
+
+        # all possible pairs of cell types without pairing same cell type
         cell_types = list(ct_subs.keys())
         pairs = list(itertools.combinations(cell_types, 2))
 
         if not formula:
             formula = f"y ~ x + {self.n_counts_key}"
 
         # Hierarchical modeling expects DataFrames
-        mcp_cell_types = {f"MCP{i + 1}": cell_types for i in range(self.n_mcps)}
+        mcp_cell_types = {f"MCP{i}": cell_types for i in range(self.n_mcps)}
         mcp_scores_df = {
-            ct: pd.DataFrame(v, index=ct_subs[ct].obs.index, columns=mcp_cell_types.keys())
+            ct: pd.DataFrame(v, index=ct_subs[ct].obs.index, columns=list(mcp_cell_types.keys()))
             for ct, v in mcp_scores.items()
         }
 
         # run HLM for each pair
         all_results: dict[str, dict[Any, dict[str, tuple[DataFrame, dict[str, Any]]]]] = {}
         mlm_progress = Progress(
             SpinnerColumn(),
@@ -801,15 +795,15 @@
 
                 merged_results = {}
 
                 mm_task = mixed_model_progress.add_task("[bold blue]Determining mixed effects", total=len(mcps))
                 for mcp in mcps:
                     mixed_model_progress.update(mm_task, description=f"[bold blue]Determining mixed effects for {mcp}")
 
-                    # TODO Check that the genes in result{sig_genes_1] are different and if so note that somewhere and explain why
+                    # TODO Check whether the genes in result{sig_genes_1] are different and if so note that somewhere and explain why
                     result = {}
                     result["HLM_result_1"], result["sig_genes_1"] = self._apply_HLM_per_MCP_for_one_pair(
                         mcp_name=mcp,
                         scores_df=mcp_scores_df[cell_type_2],
                         ct_data=ct_data_2,
                         tme=tme_2,
                         sig=sig_1,
@@ -871,44 +865,40 @@
             >>> adata, mcps, ws, ct_subs = dl.calculate_multifactor_PMD(adata, normalize=True)
             >>> stats = dl.test_association(adata, condition_label="pathology")
         """
         celltype_label = self.celltype_key
         sample_label = self.sample_id
         n_mcps = self.n_mcps
 
-        # create conditions_compare if not supplied
         if conditions_compare is None:
-            conditions_compare = list(adata.obs["path_str"].cat.categories)  # type: ignore
+            conditions_compare = list(adata.obs[condition_label].cat.categories)  # type: ignore
             if len(conditions_compare) != 2:
                 raise ValueError("Please specify conditions to compare or supply an object with only 2 conditions")
 
-        # create data frames to store results
         pvals = pd.DataFrame(1, adata.obs[celltype_label].unique(), ["mcp_" + str(n) for n in range(0, n_mcps)])
         tstats = pd.DataFrame(1, adata.obs[celltype_label].unique(), ["mcp_" + str(n) for n in range(0, n_mcps)])
         pvals_adj = pd.DataFrame(1, adata.obs[celltype_label].unique(), ["mcp_" + str(n) for n in range(0, n_mcps)])
 
         response = adata.obs.groupby(sample_label)[condition_label].agg(pd.Series.mode)
         for celltype in adata.obs[celltype_label].unique():
-            # subset data to cell type
             df = adata.obs[adata.obs[celltype_label] == celltype]
-            # run t-test for each MCP
+
             for mcpnum in ["mcp_" + str(n) for n in range(0, n_mcps)]:
                 mns = df.groupby(sample_label)[mcpnum].mean()
                 mns = pd.concat([mns, response], axis=1)
                 res = stats.ttest_ind(
                     mns[mns[condition_label] == conditions_compare[0]][mcpnum],
                     mns[mns[condition_label] == conditions_compare[1]][mcpnum],
                 )
                 pvals.loc[celltype, mcpnum] = res[1]
                 tstats.loc[celltype, mcpnum] = res[0]
-                # return(res)
 
-        # benjamini-hochberg correction for number of cell types (use BH because correlated MCPs)
         for mcpnum in ["mcp_" + str(n) for n in range(0, n_mcps)]:
             pvals_adj[mcpnum] = multipletests(pvals[mcpnum], method="fdr_bh")[1]
+
         return {"pvals": pvals, "tstats": tstats, "pvals_adj": pvals_adj}
 
     def get_mlm_mcp_genes(
         self,
         celltype: str,
         results: dict,
         MCP: str = "mcp_0",
@@ -917,15 +907,15 @@
     ):
         """Extracts MCP genes from the MCP multilevel modeling object for the cell type of interest.
 
         Args:
             celltype: Cell type of interest.
             results: dl.MultilevelModeling result object.
             MCP: MCP key of the result object.
-            threshhold: Number between [0,1]. The fraction of cell types compared against which must have the associated MCP gene.
+            threshold: Number between [0,1]. The fraction of cell types compared against which must have the associated MCP gene.
                         Defaults to 0.70.
             focal_celltypes: None (compare against all cell types) or a list of other cell types which you want to compare against.
                              Defaults to None.
 
         Returns:
             Dict with keys 'up_genes' and 'down_genes' and values of lists of genes
 
@@ -941,15 +931,14 @@
                 confounder="gender")
             >>> mcp_genes = dl.get_mlm_mcp_genes(celltype='Macrophages', results=all_results)
         """
         # Convert "mcp_x" to "MCPx" format
         # REMOVE THIS BLOCK ONCE MLM OUTPUT MATCHES STANDARD
         if MCP.startswith("mcp_"):
             MCP = MCP.replace("mcp_", "MCP")
-            # convert from MCPx to MCPx+1
             MCP = "MCP" + str(int(MCP[3:]) - 1)
 
         # Extract all comparison keys from the results object
         comparisons = list(results.keys())
 
         filtered_keys = [key for key in comparisons if celltype in key]
 
@@ -1010,34 +999,34 @@
                       Defaults to 0.1.
 
         Returns:
             Dictionary where keys are subpopulation names and values are Anndata
             objects containing the results of gene ranking analysis.
 
         Examples:
-            ct_subs = {
-            "subpop1": anndata_obj1,
-            "subpop2": anndata_obj2,
-            # ... more subpopulations ...
-            }
-            genes_results = _get_extrema_MCP_genes_single(ct_subs, mcp="mcp_4", fraction=0.2)
+            >>> ct_subs = {
+            ...     "subpop1": anndata_obj1,
+            ...     "subpop2": anndata_obj2,
+            ...     # ... more subpopulations ...
+            ... }
+            >>> genes_results = _get_extrema_MCP_genes_single(ct_subs, mcp="mcp_4", fraction=0.2)
         """
         genes = {}
         for ct in ct_subs.keys():
             mini = ct_subs[ct]
-            mini.obs[mcp]
             mini.obs["extrema"] = pd.qcut(
                 mini.obs[mcp],
                 [0, 0 + fraction, 1 - fraction, 1.0],
                 labels=["low " + mcp + " " + ct, "no", "high" + mcp + " " + ct],
             )
             sc.tl.rank_genes_groups(
                 mini, "extrema", groups=["high" + mcp + " " + ct], reference="low " + mcp + " " + ct
             )
             genes[ct] = mini  # .uns['rank_genes_groups']
+
         return genes
 
     def get_extrema_MCP_genes(self, ct_subs: dict, fraction: float = 0.1):
         """Identifies cells with extreme MCP scores.
 
         Takes as input a dictionary of subpopulations AnnData objects (DIALOGUE output),
         For each MCP it identifies cells with extreme MCP scores, then calls rank_genes_groups to
@@ -1060,16 +1049,135 @@
             >>> sc.pp.pca(adata)
             >>> dl = pt.tl.Dialogue(sample_id = "clinical.status", celltype_key = "cell.subtypes", \
                 n_counts_key = "nCount_RNA", n_mpcs = 3)
             >>> adata, mcps, ws, ct_subs = dl.calculate_multifactor_PMD(adata, normalize=True)
             >>> extrema_mcp_genes = dl.get_extrema_MCP_genes(ct_subs)
         """
         rank_dfs: dict[str, dict[Any, Any]] = {}
-        _, ct_sub = next(iter(ct_subs.items()))
+        ct_sub = next(iter(ct_subs.values()))
         mcps = [col for col in ct_sub.obs.columns if col.startswith("mcp_")]
 
         for mcp in mcps:
             rank_dfs[mcp] = {}
             ct_ranked = self._get_extrema_MCP_genes_single(ct_subs, mcp=mcp, fraction=fraction)
             for celltype in ct_ranked.keys():
                 rank_dfs[mcp][celltype] = sc.get.rank_genes_groups_df(ct_ranked[celltype], group=None)
+
         return rank_dfs
+
+    def plot_split_violins(
+        self,
+        adata: AnnData,
+        split_key: str,
+        celltype_key: str,
+        split_which: tuple[str, str] = None,
+        mcp: str = "mcp_0",
+        return_fig: bool | None = None,
+        ax: Axes | None = None,
+        save: bool | str | None = None,
+        show: bool | None = None,
+    ) -> Axes | Figure | None:
+        """Plots split violin plots for a given MCP and split variable.
+
+        Any cells with a value for split_key not in split_which are removed from the plot.
+
+        Args:
+            adata: Annotated data object.
+            split_key: Variable in adata.obs used to split the data.
+            celltype_key: Key for cell type annotations.
+            split_which: Which values of split_key to plot. Required if more than 2 values in split_key.
+            mcp: Key for MCP data. Defaults to "mcp_0".
+
+        Returns:
+            A :class:`~matplotlib.axes.Axes` object
+
+        Examples:
+            >>> import pertpy as pt
+            >>> import scanpy as sc
+            >>> adata = pt.dt.dialogue_example()
+            >>> sc.pp.pca(adata)
+            >>> dl = pt.tl.Dialogue(sample_id = "clinical.status", celltype_key = "cell.subtypes", \
+                n_counts_key = "nCount_RNA", n_mpcs = 3)
+            >>> adata, mcps, ws, ct_subs = dl.calculate_multifactor_PMD(adata, normalize=True)
+            >>> dl.plot_split_violins(adata, split_key='gender', celltype_key='cell.subtypes')
+
+        Preview:
+            .. image:: /_static/docstring_previews/dialogue_violin.png
+        """
+        df = sc.get.obs_df(adata, [celltype_key, mcp, split_key])
+        if split_which is None:
+            split_which = df[split_key].unique()
+        df = df[df[split_key].isin(split_which)]
+        df[split_key] = df[split_key].cat.remove_unused_categories()
+
+        ax = sns.violinplot(data=df, x=celltype_key, y=mcp, hue=split_key, split=True)
+
+        ax.set_xticklabels(ax.get_xticklabels(), rotation=90)
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return ax
+        return None
+
+    def plot_pairplot(
+        self,
+        adata: AnnData,
+        celltype_key: str,
+        color: str,
+        sample_id: str,
+        mcp: str = "mcp_0",
+        return_fig: bool | None = None,
+        show: bool | None = None,
+        save: bool | str | None = None,
+    ) -> PairGrid | Figure | None:
+        """Generate a pairplot visualization for multi-cell perturbation (MCP) data.
+
+        Computes the mean of a specified MCP feature (mcp) for each combination of sample and cell type,
+        then creates a pairplot to visualize the relationships between these mean MCP values.
+
+        Args:
+            adata: Annotated data object.
+            celltype_key: Key in `adata.obs` containing cell type annotations.
+            color: Key in `adata.obs` for color annotations. This parameter is used as the hue
+            sample_id: Key in `adata.obs` for the sample annotations.
+            mcp: Key in `adata.obs` for MCP feature values. Defaults to `"mcp_0"`.
+
+        Returns:
+            Seaborn Pairgrid object.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> import scanpy as sc
+            >>> adata = pt.dt.dialogue_example()
+            >>> sc.pp.pca(adata)
+            >>> dl = pt.tl.Dialogue(sample_id = "clinical.status", celltype_key = "cell.subtypes", \
+                n_counts_key = "nCount_RNA", n_mpcs = 3)
+            >>> adata, mcps, ws, ct_subs = dl.calculate_multifactor_PMD(adata, normalize=True)
+            >>> dl.plot_pairplot(adata, celltype_key="cell.subtypes", color="gender", sample_id="clinical.status")
+
+        Preview:
+            .. image:: /_static/docstring_previews/dialogue_pairplot.png
+        """
+        mean_mcps = adata.obs.groupby([sample_id, celltype_key])[mcp].mean()
+        mean_mcps = mean_mcps.reset_index()
+        mcp_pivot = pd.pivot(mean_mcps[[sample_id, celltype_key, mcp]], index=sample_id, columns=celltype_key)[mcp]
+
+        aggstats = adata.obs.groupby([sample_id])[color].describe()
+        aggstats = aggstats.loc[list(mcp_pivot.index), :]
+        aggstats[color] = aggstats["top"]
+        mcp_pivot = pd.concat([mcp_pivot, aggstats[color]], axis=1)
+        ax = sns.pairplot(mcp_pivot, hue=color, corner=True)
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return ax
+        return None
```

### Comparing `pertpy-0.6.0/pertpy/tools/_kernel_pca.py` & `pertpy-0.7.0/pertpy/tools/_kernel_pca.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/pertpy/tools/_milo.py` & `pertpy-0.7.0/pertpy/tools/_milo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 from __future__ import annotations
 
 import logging
 import random
 import re
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import scanpy as sc
+import seaborn as sns
 from anndata import AnnData
 from mudata import MuData
 from rich import print
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
+    from matplotlib.axes import Axes
+    from matplotlib.colors import Colormap
+
 try:
     from rpy2.robjects import conversion, numpy2ri, pandas2ri
     from rpy2.robjects.packages import STAP, PackageNotInstalledError, importr
 except ModuleNotFoundError:
     print(
         "[bold yellow]ryp2 is not installed. Install with [green]pip install rpy2 [yellow]to run tools with R support."
     )
@@ -35,15 +44,15 @@
     ) -> MuData:
         """Prepare a MuData object for subsequent processing.
 
         Args:
             input: AnnData
             feature_key: Key to store the cell-level AnnData object in the MuData object
         Returns:
-            MuData: MuData object with original AnnData (default is `mudata[feature_key]`).
+            MuData: MuData object with original AnnData. Defaults to`mudata[feature_key]`.
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.bhattacherjee()
             >>> milo = pt.tl.Milo()
             >>> mdata = milo.load(adata)
         """
@@ -67,19 +76,19 @@
         Thus, multiple neighbourhoods may be collapsed to prevent over-sampling the graph space.
 
         Args:
             data: AnnData object with KNN graph defined in `obsp` or MuData object with a modality with KNN graph defined in `obsp`
             neighbors_key: The key in `adata.obsp` or `mdata[feature_key].obsp` to use as KNN graph.
                            If not specified, `make_nhoods` looks .obsp[‘connectivities’] for connectivities (default storage places for `scanpy.pp.neighbors`).
                            If specified, it looks at .obsp[.uns[neighbors_key][‘connectivities_key’]] for connectivities.
-                           (default: None)
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
-            prop: Fraction of cells to sample for neighbourhood index search. (default: 0.1)
-            seed: Random seed for cell sampling. (default: 0)
-            copy: Determines whether a copy of the `adata` is returned. (default: False)
+                           Defaults to None.
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
+            prop: Fraction of cells to sample for neighbourhood index search. Defaults to 0.1.
+            seed: Random seed for cell sampling. Defaults to 0.
+            copy: Determines whether a copy of the `adata` is returned. Defaults to False.
 
         Returns:
             If `copy=True`, returns the copy of `adata` with the result in `.obs`, `.obsm`, and `.uns`.
             Otherwise:
 
             nhoods: scipy.sparse._csr.csr_matrix in `adata.obsm['nhoods']`.
             A binary matrix of cell to neighbourhood assignments. Neighbourhoods in the columns are ordered by the order of the index cell in adata.obs_names
@@ -186,15 +195,15 @@
         feature_key: str | None = "rna",
     ):
         """Builds a sample-level AnnData object storing the matrix of cell counts per sample per neighbourhood.
 
         Args:
             data: AnnData object with neighbourhoods defined in `obsm['nhoods']` or MuData object with a modality with neighbourhoods defined in `obsm['nhoods']`
             sample_col: Column in adata.obs that contains sample information
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
 
         Returns:
             MuData object storing the original (i.e. rna) AnnData in `mudata[feature_key]`
             and the compositional anndata storing the neighbourhood cell counts in `mudata['milo']`.
             Here:
             - `mudata['milo'].obs_names` are samples (defined from `adata.obs['sample_col']`)
             - `mudata['milo'].var_names` are neighbourhoods
@@ -419,15 +428,15 @@
             >>> import scanpy as sc
             >>> adata = pt.dt.bhattacherjee()
             >>> milo = pt.tl.Milo()
             >>> mdata = milo.load(adata)
             >>> sc.pp.neighbors(mdata["rna"])
             >>> milo.make_nhoods(mdata["rna"])
             >>> mdata = milo.count_nhoods(mdata, sample_col="orig.ident")
-            >>> milo.annotate_nhoods(mdata, anno_col='cell_type')
+            >>> milo.annotate_nhoods(mdata, anno_col="cell_type")
         """
         try:
             sample_adata = mdata["milo"]
         except KeyError:
             print(
                 "milo_mdata should be a MuData object with two slots: feature_key and 'milo' - please run milopy.count_nhoods(adata) first"
             )
@@ -470,15 +479,15 @@
             >>> import scanpy as sc
             >>> adata = pt.dt.bhattacherjee()
             >>> milo = pt.tl.Milo()
             >>> mdata = milo.load(adata)
             >>> sc.pp.neighbors(mdata["rna"])
             >>> milo.make_nhoods(mdata["rna"])
             >>> mdata = milo.count_nhoods(mdata, sample_col="orig.ident")
-            >>> milo.annotate_nhoods_continuous(mdata, anno_col='nUMI')
+            >>> milo.annotate_nhoods_continuous(mdata, anno_col="nUMI")
         """
         if "milo" not in mdata.mod:
             raise ValueError(
                 "milo_mdata should be a MuData object with two slots: feature_key and 'milo' - please run milopy.count_nhoods(adata) first"
             )
         adata = mdata[feature_key]
 
@@ -659,15 +668,17 @@
             raise
 
     def _graph_spatial_fdr(
         self,
         sample_adata: AnnData,
         neighbors_key: str | None = None,
     ):
-        """FDR correction weighted on inverse of connectivity of neighbourhoods. The distance to the k-th nearest neighbor is used as a measure of connectivity.
+        """FDR correction weighted on inverse of connectivity of neighbourhoods.
+
+        The distance to the k-th nearest neighbor is used as a measure of connectivity.
 
         Args:
             sample_adata: Sample-level AnnData.
             neighbors_key: The key in `adata.obsp` to use as KNN graph. Defaults to None.
         """
         # use 1/connectivity as the weighting for the weighted BH adjustment from Cydar
         w = 1 / sample_adata.var["kth_distance"]
@@ -682,7 +693,330 @@
 
         adjp = np.zeros(shape=len(o))
         adjp[o] = (sum(w) * pvalues / np.cumsum(w))[::-1].cummin()[::-1]
         adjp = np.array([x if x < 1 else 1 for x in adjp])
 
         sample_adata.var["SpatialFDR"] = np.nan
         sample_adata.var.loc[keep_nhoods, "SpatialFDR"] = adjp
+
+    def plot_nhood_graph(
+        self,
+        mdata: MuData,
+        alpha: float = 0.1,
+        min_logFC: float = 0,
+        min_size: int = 10,
+        plot_edges: bool = False,
+        title: str = "DA log-Fold Change",
+        color_map: Colormap | str | None = None,
+        palette: str | Sequence[str] | None = None,
+        ax: Axes | None = None,
+        show: bool | None = None,
+        save: bool | str | None = None,
+        **kwargs,
+    ) -> None:
+        """Visualize DA results on abstracted graph (wrapper around sc.pl.embedding)
+
+        Args:
+            mdata: MuData object
+            alpha: Significance threshold. (default: 0.1)
+            min_logFC: Minimum absolute log-Fold Change to show results. If is 0, show all significant neighbourhoods. Defaults to 0.
+            min_size: Minimum size of nodes in visualization. (default: 10)
+            plot_edges: If edges for neighbourhood overlaps whould be plotted. Defaults to False.
+            title: Plot title. Defaults to "DA log-Fold Change".
+            show: Show the plot, do not return axis.
+            save: If `True` or a `str`, save the figure. A string is appended to the default filename.
+                  Infer the filetype if ending on {`'.pdf'`, `'.png'`, `'.svg'`}.
+            **kwargs: Additional arguments to `scanpy.pl.embedding`.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> import scanpy as sc
+            >>> adata = pt.dt.bhattacherjee()
+            >>> milo = pt.tl.Milo()
+            >>> mdata = milo.load(adata)
+            >>> sc.pp.neighbors(mdata["rna"])
+            >>> sc.tl.umap(mdata["rna"])
+            >>> milo.make_nhoods(mdata["rna"])
+            >>> mdata = milo.count_nhoods(mdata, sample_col="orig.ident")
+            >>> milo.da_nhoods(mdata,
+            >>>            design='~label',
+            >>>            model_contrasts='labelwithdraw_15d_Cocaine-labelwithdraw_48h_Cocaine')
+            >>> milo.build_nhood_graph(mdata)
+            >>> milo.plot_nhood_graph(mdata)
+
+        Preview:
+            .. image:: /_static/docstring_previews/milo_nhood_graph.png
+        """
+        nhood_adata = mdata["milo"].T.copy()
+
+        if "Nhood_size" not in nhood_adata.obs.columns:
+            raise KeyError(
+                'Cannot find "Nhood_size" column in adata.uns["nhood_adata"].obs -- \
+                    please run milopy.utils.build_nhood_graph(adata)'
+            )
+
+        nhood_adata.obs["graph_color"] = nhood_adata.obs["logFC"]
+        nhood_adata.obs.loc[nhood_adata.obs["SpatialFDR"] > alpha, "graph_color"] = np.nan
+        nhood_adata.obs["abs_logFC"] = abs(nhood_adata.obs["logFC"])
+        nhood_adata.obs.loc[nhood_adata.obs["abs_logFC"] < min_logFC, "graph_color"] = np.nan
+
+        # Plotting order - extreme logFC on top
+        nhood_adata.obs.loc[nhood_adata.obs["graph_color"].isna(), "abs_logFC"] = np.nan
+        ordered = nhood_adata.obs.sort_values("abs_logFC", na_position="first").index
+        nhood_adata = nhood_adata[ordered]
+
+        vmax = np.max([nhood_adata.obs["graph_color"].max(), abs(nhood_adata.obs["graph_color"].min())])
+        vmin = -vmax
+
+        sc.pl.embedding(
+            nhood_adata,
+            "X_milo_graph",
+            color="graph_color",
+            cmap="RdBu_r",
+            size=nhood_adata.obs["Nhood_size"] * min_size,
+            edges=plot_edges,
+            neighbors_key="nhood",
+            sort_order=False,
+            frameon=False,
+            vmax=vmax,
+            vmin=vmin,
+            title=title,
+            color_map=color_map,
+            palette=palette,
+            ax=ax,
+            show=show,
+            save=save,
+            **kwargs,
+        )
+
+    def plot_nhood(
+        self,
+        mdata: MuData,
+        ix: int,
+        feature_key: str | None = "rna",
+        basis: str = "X_umap",
+        color_map: Colormap | str | None = None,
+        palette: str | Sequence[str] | None = None,
+        return_fig: bool | None = None,
+        ax: Axes | None = None,
+        show: bool | None = None,
+        save: bool | str | None = None,
+        **kwargs,
+    ) -> None:
+        """Visualize cells in a neighbourhood.
+
+        Args:
+            mdata: MuData object with feature_key slot, storing neighbourhood assignments in `mdata[feature_key].obsm['nhoods']`
+            ix: index of neighbourhood to visualize
+            basis: Embedding to use for visualization. Defaults to "X_umap".
+            show: Show the plot, do not return axis.
+            save: If True or a str, save the figure. A string is appended to the default filename. Infer the filetype if ending on {'.pdf', '.png', '.svg'}.
+            **kwargs: Additional arguments to `scanpy.pl.embedding`.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> import scanpy as sc
+            >>> adata = pt.dt.bhattacherjee()
+            >>> milo = pt.tl.Milo()
+            >>> mdata = milo.load(adata)
+            >>> sc.pp.neighbors(mdata["rna"])
+            >>> sc.tl.umap(mdata["rna"])
+            >>> milo.make_nhoods(mdata["rna"])
+            >>> milo.plot_nhood(mdata, ix=0)
+
+        Preview:
+            .. image:: /_static/docstring_previews/milo_nhood.png
+        """
+        mdata[feature_key].obs["Nhood"] = mdata[feature_key].obsm["nhoods"][:, ix].toarray().ravel()
+        sc.pl.embedding(
+            mdata[feature_key],
+            basis,
+            color="Nhood",
+            size=30,
+            title="Nhood" + str(ix),
+            color_map=color_map,
+            palette=palette,
+            return_fig=return_fig,
+            ax=ax,
+            show=show,
+            save=save,
+            **kwargs,
+        )
+
+    def plot_da_beeswarm(
+        self,
+        mdata: MuData,
+        feature_key: str | None = "rna",
+        anno_col: str = "nhood_annotation",
+        alpha: float = 0.1,
+        subset_nhoods: list[str] = None,
+        palette: str | Sequence[str] | dict[str, str] | None = None,
+        return_fig: bool | None = None,
+        save: bool | str | None = None,
+        show: bool | None = None,
+    ) -> None:
+        """Plot beeswarm plot of logFC against nhood labels
+
+        Args:
+            mdata: MuData object
+            anno_col: Column in adata.uns['nhood_adata'].obs to use as annotation. (default: 'nhood_annotation'.)
+            alpha: Significance threshold. (default: 0.1)
+            subset_nhoods: List of nhoods to plot. If None, plot all nhoods. Defaults to None.
+            palette: Name of Seaborn color palette for violinplots.
+                     Defaults to pre-defined category colors for violinplots.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> import scanpy as sc
+            >>> adata = pt.dt.bhattacherjee()
+            >>> milo = pt.tl.Milo()
+            >>> mdata = milo.load(adata)
+            >>> sc.pp.neighbors(mdata["rna"])
+            >>> milo.make_nhoods(mdata["rna"])
+            >>> mdata = milo.count_nhoods(mdata, sample_col="orig.ident")
+            >>> milo.da_nhoods(mdata, design="~label")
+            >>> milo.annotate_nhoods(mdata, anno_col="cell_type")
+            >>> milo.plot_da_beeswarm(mdata)
+
+        Preview:
+            .. image:: /_static/docstring_previews/milo_da_beeswarm.png
+        """
+        try:
+            nhood_adata = mdata["milo"].T.copy()
+        except KeyError:
+            raise RuntimeError(
+                "mdata should be a MuData object with two slots: feature_key and 'milo'. Run 'milopy.count_nhoods(adata)' first."
+            ) from None
+
+        try:
+            nhood_adata.obs[anno_col]
+        except KeyError:
+            raise RuntimeError(
+                f"Unable to find {anno_col} in mdata['milo'].var. Run 'milopy.utils.annotate_nhoods(adata, anno_col)' first"
+            ) from None
+
+        if subset_nhoods is not None:
+            nhood_adata = nhood_adata[nhood_adata.obs[anno_col].isin(subset_nhoods)]
+
+        try:
+            nhood_adata.obs["logFC"]
+        except KeyError:
+            raise RuntimeError(
+                "Unable to find 'logFC' in mdata.uns['nhood_adata'].obs. Run 'core.da_nhoods(adata)' first."
+            ) from None
+
+        sorted_annos = (
+            nhood_adata.obs[[anno_col, "logFC"]].groupby(anno_col).median().sort_values("logFC", ascending=True).index
+        )
+
+        anno_df = nhood_adata.obs[[anno_col, "logFC", "SpatialFDR"]].copy()
+        anno_df["is_signif"] = anno_df["SpatialFDR"] < alpha
+        anno_df = anno_df[anno_df[anno_col] != "nan"]
+
+        try:
+            obs_col = nhood_adata.uns["annotation_obs"]
+            if palette is None:
+                palette = dict(
+                    zip(
+                        mdata[feature_key].obs[obs_col].cat.categories,
+                        mdata[feature_key].uns[f"{obs_col}_colors"],
+                        strict=False,
+                    )
+                )
+            sns.violinplot(
+                data=anno_df,
+                y=anno_col,
+                x="logFC",
+                order=sorted_annos,
+                inner=None,
+                orient="h",
+                palette=palette,
+                linewidth=0,
+                scale="width",
+            )
+        except BaseException:  # noqa: BLE001
+            sns.violinplot(
+                data=anno_df,
+                y=anno_col,
+                x="logFC",
+                order=sorted_annos,
+                inner=None,
+                orient="h",
+                linewidth=0,
+                scale="width",
+            )
+        sns.stripplot(
+            data=anno_df,
+            y=anno_col,
+            x="logFC",
+            order=sorted_annos,
+            size=2,
+            hue="is_signif",
+            palette=["grey", "black"],
+            orient="h",
+            alpha=0.5,
+        )
+        plt.legend(loc="upper left", title=f"< {int(alpha * 100)}% SpatialFDR", bbox_to_anchor=(1, 1), frameon=False)
+        plt.axvline(x=0, ymin=0, ymax=1, color="black", linestyle="--")
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if (not show and not save) or (show is None and save is None):
+            return plt.gca()
+
+    def plot_nhood_counts_by_cond(
+        self,
+        mdata: MuData,
+        test_var: str,
+        subset_nhoods: list[str] = None,
+        log_counts: bool = False,
+        return_fig: bool | None = None,
+        save: bool | str | None = None,
+        show: bool | None = None,
+    ) -> None:
+        """Plot boxplot of cell numbers vs condition of interest.
+
+        Args:
+            mdata: MuData object storing cell level and nhood level information
+            test_var: Name of column in adata.obs storing condition of interest (y-axis for boxplot)
+            subset_nhoods: List of obs_names for neighbourhoods to include in plot. If None, plot all nhoods. Defaults to None.
+            log_counts: Whether to plot log1p of cell counts. Defaults to False.
+        """
+        try:
+            nhood_adata = mdata["milo"].T.copy()
+        except KeyError:
+            raise RuntimeError(
+                "mdata should be a MuData object with two slots: feature_key and 'milo'. Run milopy.count_nhoods(mdata) first"
+            ) from None
+
+        if subset_nhoods is None:
+            subset_nhoods = nhood_adata.obs_names
+
+        pl_df = pd.DataFrame(nhood_adata[subset_nhoods].X.A, columns=nhood_adata.var_names).melt(
+            var_name=nhood_adata.uns["sample_col"], value_name="n_cells"
+        )
+        pl_df = pd.merge(pl_df, nhood_adata.var)
+        pl_df["log_n_cells"] = np.log1p(pl_df["n_cells"])
+        if not log_counts:
+            sns.boxplot(data=pl_df, x=test_var, y="n_cells", color="lightblue")
+            sns.stripplot(data=pl_df, x=test_var, y="n_cells", color="black", s=3)
+            plt.ylabel("# cells")
+        else:
+            sns.boxplot(data=pl_df, x=test_var, y="log_n_cells", color="lightblue")
+            sns.stripplot(data=pl_df, x=test_var, y="log_n_cells", color="black", s=3)
+            plt.ylabel("log(# cells + 1)")
+
+        plt.xticks(rotation=90)
+        plt.xlabel(test_var)
+
+        if save:
+            plt.savefig(save, bbox_inches="tight")
+        if show:
+            plt.show()
+        if return_fig:
+            return plt.gcf()
+        if not (show or save):
+            return plt.gca()
```

### Comparing `pertpy-0.6.0/pertpy/tools/transferlearning_MMD_LICENSE` & `pertpy-0.7.0/pertpy/tools/transferlearning_MMD_LICENSE`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/pertpy/tools/_coda/_sccoda.py` & `pertpy-0.7.0/pertpy/tools/_coda/_sccoda.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 
 import arviz as az
 import jax.numpy as jnp
 import numpy as np
 import numpyro as npy
 import numpyro.distributions as npd
 from anndata import AnnData
-from jax import random
-from jax.config import config
+from jax import config, random
 from mudata import MuData
 from numpyro.infer import Predictive
 from rich import print
 
 from pertpy.tools._coda._base_coda import CompositionalModel2, from_scanpy
 
 if TYPE_CHECKING:
     import pandas as pd
 
 config.update("jax_enable_x64", True)
 
 
 class Sccoda(CompositionalModel2):
-
     """
     Statistical model for single-cell differential composition analysis with specification of a reference cell type.
     This is the standard scCODA model and recommended for all uses.
 
     The hierarchical formulation of the model for one sample is:
 
     .. math::
@@ -86,16 +84,19 @@
         Returns:
             MuData: MuData object with cell-level AnnData (`mudata[modality_key_1]`) and aggregated sample-level AnnData (`mudata[modality_key_2]`).
 
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch", covariate_obs=["condition"])
         """
         if type == "cell_level":
             if generate_sample_level:
                 adata_coda = from_scanpy(
                     adata=adata,
                     cell_type_identifier=cell_type_identifier,
                     sample_identifier=sample_identifier,
@@ -140,16 +141,20 @@
             - `adata.uns["scCODA_params"]["model_type"]` or `data[modality_key].uns["scCODA_params"]["model_type"]`: String indicating the model type ("classic")
             - `adata.uns["scCODA_params"]["select_type"]` or `data[modality_key].uns["scCODA_params"]["select_type"]`: String indicating the type of spike_and_slab selection ("spikeslab")
 
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
         """
         if isinstance(data, MuData):
             adata = data[modality_key]
             is_MuData = True
         if isinstance(data, AnnData):
             adata = data
@@ -189,18 +194,22 @@
         Returns:
             Return AnnData object.
 
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
-            >>> adata = sccoda.set_init_mcmc_states(rng_key=42, ref_index=0, sample_adata=mdata['coda'])
+            >>> adata = sccoda.set_init_mcmc_states(rng_key=42, ref_index=0, sample_adata=mdata["coda"])
         """
         # data dimensions
         N, D = sample_adata.obsm["covariate_matrix"].shape
         P = sample_adata.X.shape[1]
 
         # Sizes of different parameter matrices
         alpha_size = [P]
@@ -308,16 +317,20 @@
         Returns:
             az.InferenceData: arviz_data with all MCMC information
 
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
             >>> sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000, rng_key=42)
             >>> arviz_data = sccoda.make_arviz(mdata, num_prior_samples=100)
         """
         if isinstance(data, MuData):
             try:
                 sample_adata = data[modality_key]
@@ -361,15 +374,15 @@
         # Prior and posterior predictive simulation
         numpyro_covariates = jnp.array(sample_adata.obsm["covariate_matrix"], dtype=dtype)
         numpyro_n_total = jnp.array(sample_adata.obsm["sample_counts"], dtype=dtype)
         ref_index = jnp.array(sample_adata.uns["scCODA_params"]["reference_index"])
 
         if rng_key is None:
             rng = np.random.default_rng()
-            rng_key = random.PRNGKey(rng.integers(0, 10000))
+            rng_key = random.key(rng.integers(0, 10000))
 
         if use_posterior_predictive:
             posterior_predictive = Predictive(self.model, self.mcmc.get_samples())(
                 rng_key,
                 counts=None,
                 covariates=numpyro_covariates,
                 n_total=numpyro_n_total,
@@ -410,63 +423,79 @@
         **kwargs,
     ):
         """
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
             >>> sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000, rng_key=42)
         """
         return super().run_nuts(data, modality_key, num_samples, num_warmup, rng_key, copy, *args, **kwargs)
 
     run_nuts.__doc__ = CompositionalModel2.run_nuts.__doc__ + run_nuts.__doc__
 
     def credible_effects(self, data: AnnData | MuData, modality_key: str = "coda", est_fdr: float = None) -> pd.Series:
         """
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
             >>> sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000, rng_key=42)
             >>> credible_effects = sccoda.credible_effects(mdata)
         """
         return super().credible_effects(data, modality_key, est_fdr)
 
     credible_effects.__doc__ = CompositionalModel2.credible_effects.__doc__ + credible_effects.__doc__
 
     def summary(self, data: AnnData | MuData, extended: bool = False, modality_key: str = "coda", *args, **kwargs):
         """
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
             >>> sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000, rng_key=42)
             >>> sccoda.summary(mdata)
         """
         return super().summary(data, extended, modality_key, *args, **kwargs)
 
     summary.__doc__ = CompositionalModel2.summary.__doc__ + summary.__doc__
 
     def set_fdr(self, data: AnnData | MuData, est_fdr: float, modality_key: str = "coda", *args, **kwargs):
         """
         Examples:
             >>> import pertpy as pt
             >>> haber_cells = pt.dt.haber_2017_regions()
             >>> sccoda = pt.tl.Sccoda()
-            >>> mdata = sccoda.load(haber_cells, type="cell_level", generate_sample_level=True, cell_type_identifier="cell_label", \
-                sample_identifier="batch", covariate_obs=["condition"])
+            >>> mdata = sccoda.load(haber_cells,
+            >>>                     type="cell_level",
+            >>>                     generate_sample_level=True,
+            >>>                     cell_type_identifier="cell_label",
+            >>>                     sample_identifier="batch",
+            >>>                     covariate_obs=["condition"])
             >>> mdata = sccoda.prepare(mdata, formula="condition", reference_cell_type="Endocrine")
             >>> sccoda.run_nuts(mdata, num_warmup=100, num_samples=1000, rng_key=42)
             >>> sccoda.set_fdr(mdata, est_fdr=0.4)
         """
         return super().set_fdr(data, est_fdr, modality_key, *args, **kwargs)
 
     set_fdr.__doc__ = CompositionalModel2.set_fdr.__doc__ + set_fdr.__doc__
```

### Comparing `pertpy-0.6.0/pertpy/tools/_coda/_tasccoda.py` & `pertpy-0.7.0/pertpy/tools/_coda/_tasccoda.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal
 
 import arviz as az
-import ete3 as ete
 import jax.numpy as jnp
 import numpy as np
 import numpyro as npy
 import numpyro.distributions as npd
 import toytree as tt
 from anndata import AnnData
-from jax import random
-from jax.config import config
+from jax import config, random
 from mudata import MuData
 from numpyro.infer import Predictive
 from rich import print
 
 from pertpy.tools._coda._base_coda import (
     CompositionalModel2,
     collapse_singularities,
@@ -101,15 +99,15 @@
             modality_key_2: Key to the aggregated sample-level AnnData object in the MuData object. Defaults to "coda".
 
         Returns:
             MuData: MuData object with cell-level AnnData (`mudata[modality_key_1]`) and aggregated sample-level AnnData (`mudata[modality_key_2]`).
 
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
         """
@@ -144,25 +142,27 @@
         formula: str,
         reference_cell_type: str = "automatic",
         automatic_reference_absence_threshold: float = 0.05,
         tree_key: str = None,
         pen_args: dict = None,
         modality_key: str = "coda",
     ) -> AnnData | MuData:
-        """Handles data preprocessing, covariate matrix creation, reference selection, and zero count replacement for tascCODA. Also sets model parameters, model type (tree_agg), effect selection type (sslaso) and performs tree processing.
+        """Handles data preprocessing, covariate matrix creation, reference selection, and zero count replacement for tascCODA.
 
         Args:
             data: Anndata object with cell counts as .X and covariates saved in .obs or a MuData object.
             formula: R-style formula for building the covariate matrix.
-                Categorical covariates are handled automatically, with the covariate value of the first sample being used as the reference category.
-                To set a different level as the base category for a categorical covariate, use "C(<CovariateName>, Treatment('<ReferenceLevelName>'))"
+                     Categorical covariates are handled automatically, with the covariate value of the first sample being used as the reference category.
+                     To set a different level as the base category for a categorical covariate, use "C(<CovariateName>, Treatment('<ReferenceLevelName>'))"
             reference_cell_type: Column name that sets the reference cell type.
-                Reference the name of a column. If "automatic", the cell type with the lowest dispersion in relative abundance that is present in at least 90% of samlpes will be chosen. Defaults to "automatic".
-            automatic_reference_absence_threshold: If using reference_cell_type = "automatic", determine the maximum fraction of zero entries for a cell type
-                to be considered as a possible reference cell type. Defaults to 0.05.
+                                 If "automatic", the cell type with the lowest dispersion in relative abundance that is present in at least 90% of samlpes will be chosen.
+                                 Defaults to "automatic".
+            automatic_reference_absence_threshold: If using reference_cell_type = "automatic",
+                                                   determine the maximum fraction of zero entries for a cell type
+                                                   to be considered as a possible reference cell type. Defaults to 0.05.
             tree_key: Key in `adata.uns` that contains the tree structure
             pen_args: Dictionary with penalty arguments. With `reg="scaled_3"`, the parameters phi (aggregation bias), lambda_1, lambda_0 can be set here.
                 See the tascCODA paper for an explanation of these parameters. Default: lambda_0 = 50, lambda_1 = 5, phi = 0.
             modality_key: If data is a MuData object, specify key to the aggregated sample-level AnnData object in the MuData object. Defaults to "coda".
 
         Returns:
             Return an AnnData (if input data is an AnnData object) or return a MuData (if input data is a MuData object)
@@ -171,15 +171,15 @@
 
             - `adata.uns["param_names"]` or `data[modality_key].uns["param_names"]`: List with the names of all tracked latent model parameters (through `npy.sample` or `npy.deterministic`)
             - `adata.uns["scCODA_params"]["model_type"]` or `data[modality_key].uns["scCODA_params"]["model_type"]`: String indicating the model type ("classic")
             - `adata.uns["scCODA_params"]["select_type"]` or `data[modality_key].uns["scCODA_params"]["select_type"]`: String indicating the type of spike_and_slab selection ("spikeslab")
 
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
@@ -195,14 +195,22 @@
             adata = data
             is_MuData = False
         adata = super().prepare(adata, formula, reference_cell_type, automatic_reference_absence_threshold)
 
         if tree_key is None:
             raise ValueError("Please specify the key in .uns that contains the tree structure!")
 
+        # Scoped import due to installation issues
+        try:
+            import ete3 as ete
+        except ImportError:
+            raise ImportError(
+                "To use tasccoda please install additional dependencies as `pip install pertpy[coda]`"
+            ) from None
+
         # toytree tree - only for legacy reasons, can be removed in the final version
         if isinstance(adata.uns[tree_key], tt.tree):
             # Collapse singularities in the tree
             phy_tree = collapse_singularities(adata.uns[tree_key])
 
             # Get ancestor matrix
             A, T = get_a(phy_tree)
@@ -311,25 +319,25 @@
             sample_adata: Anndata object with cell counts as sample_adata.X and covariates saved in sample_adata.obs.
 
         Returns:
             Return AnnData
 
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
             >>>     mdata, formula="Health", reference_cell_type="automatic", tree_key="lineage", pen_args={"phi": 0}
             >>> )
-            >>> adata = tasccoda.set_init_mcmc_states(rng_key=42, ref_index=[0,1], sample_adata=mdata['coda'])
+            >>> adata = tasccoda.set_init_mcmc_states(rng_key=42, ref_index=[0, 1], sample_adata=mdata["coda"])
         """
         N, D = sample_adata.obsm["covariate_matrix"].shape
         P = sample_adata.X.shape[1]
         T = sample_adata.uns["scCODA_params"]["T"]
 
         # Reference nodes must be sorted by index
         ref_index = np.sort(ref_index)
@@ -475,15 +483,15 @@
             use_posterior_predictive: If True, the posterior predictive will be calculated. Defaults to True.
 
         Returns:
             arviz.InferenceData: arviz_data
 
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
@@ -539,15 +547,15 @@
         # Prior and posterior predictive simulation
         numpyro_covariates = jnp.array(sample_adata.obsm["covariate_matrix"], dtype=dtype)
         numpyro_n_total = jnp.array(sample_adata.obsm["sample_counts"], dtype=dtype)
         ref_index = jnp.array(sample_adata.uns["scCODA_params"]["reference_index"])
 
         if rng_key is None:
             rng = np.random.default_rng()
-            rng_key = random.PRNGKey(rng.integers(0, 10000))
+            rng_key = random.key(rng.integers(0, 10000))
 
         if use_posterior_predictive:
             posterior_predictive = Predictive(self.model, self.mcmc.get_samples())(
                 rng_key,
                 counts=None,
                 covariates=numpyro_covariates,
                 n_total=numpyro_n_total,
@@ -586,15 +594,15 @@
         copy: bool = False,
         *args,
         **kwargs,
     ):
         """
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
@@ -606,15 +614,15 @@
 
     run_nuts.__doc__ = CompositionalModel2.run_nuts.__doc__ + run_nuts.__doc__
 
     def summary(self, data: AnnData | MuData, extended: bool = False, modality_key: str = "coda", *args, **kwargs):
         """
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
@@ -627,15 +635,15 @@
 
     summary.__doc__ = CompositionalModel2.summary.__doc__ + summary.__doc__
 
     def credible_effects(self, data: AnnData | MuData, modality_key: str = "coda", est_fdr: float = None) -> pd.Series:
         """
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
@@ -648,15 +656,15 @@
 
     credible_effects.__doc__ = CompositionalModel2.credible_effects.__doc__ + credible_effects.__doc__
 
     def set_fdr(self, data: AnnData | MuData, est_fdr: float, modality_key: str = "coda", *args, **kwargs):
         """
         Examples:
             >>> import pertpy as pt
-            >>> adata = pt.dt.smillie()
+            >>> adata = pt.dt.tasccoda_example()
             >>> tasccoda = pt.tl.Tasccoda()
             >>> mdata = tasccoda.load(
             >>>     adata, type="sample_level",
             >>>     levels_agg=["Major_l1", "Major_l2", "Major_l3", "Major_l4", "Cluster"],
             >>>     key_added="lineage", add_level_name=True
             >>> )
             >>> mdata = tasccoda.prepare(
```

### Comparing `pertpy-0.6.0/pertpy/tools/_distances/_distance_tests.py` & `pertpy-0.7.0/pertpy/tools/_distances/_distance_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         alpha: Significance level. Defaults to 0.05.
         correction: Multiple testing correction method. Defaults to 'holm-sidak'.
         cell_wise_metric: Metric to use between single cells. Defaults to "euclidean".
 
     Examples:
         >>> import pertpy as pt
         >>> adata = pt.dt.distance_example_data()
-        >>> distance_test = pt.tl.DistanceTest('edistance', n_perms=1000)
-        >>> tab = distance_test(adata, groupby='perturbation', contrast='control')
+        >>> distance_test = pt.tl.DistanceTest("edistance", n_perms=1000)
+        >>> tab = distance_test(adata, groupby="perturbation", contrast="control")
     """
 
     def __init__(
         self,
         metric: str,
         n_perms: int = 1000,
         layer_key: str = None,
@@ -96,16 +96,16 @@
                 - significant: whether the group is significantly different from the contrast group
                 - pvalue_adj: p-value after multiple testing correction
                 - significant_adj: whether the group is significantly different from the contrast group after multiple testing correction
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.distance_example_data()
-            >>> distance_test = pt.tl.DistanceTest('edistance', n_perms=1000)
-            >>> tab = distance_test(adata, groupby='perturbation', contrast='control')
+            >>> distance_test = pt.tl.DistanceTest("edistance", n_perms=1000)
+            >>> tab = distance_test(adata, groupby="perturbation", contrast="control")
         """
         if self.distance.metric_fct.accepts_precomputed:
             # Much faster if the metric can be called on the precomputed
             # distance matrix, but not all metrics can do that.
             return self.test_precomputed(adata, groupby, contrast, show_progressbar)
         else:
             return self.test_xy(adata, groupby, contrast, show_progressbar)
@@ -130,16 +130,16 @@
                 - significant: whether the group is significantly different from the contrast group
                 - pvalue_adj: p-value after multiple testing correction
                 - significant_adj: whether the group is significantly different from the contrast group after multiple testing correction
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.distance_example_data()
-            >>> distance_test = pt.tl.DistanceTest('edistance', n_perms=1000)
-            >>> test_results = distance_test.test_xy(adata, groupby='perturbation', contrast='control')
+            >>> distance_test = pt.tl.DistanceTest("edistance", n_perms=1000)
+            >>> test_results = distance_test.test_xy(adata, groupby="perturbation", contrast="control")
         """
         groups = adata.obs[groupby].unique()
         if contrast not in groups:
             raise ValueError(f"Contrast group {contrast} not found in {groupby} of adata.obs.")
         fct = track if show_progressbar else lambda iterable: iterable
         embedding = adata.obsm[self.obsm_key]
 
@@ -222,16 +222,16 @@
                 - significant: whether the group is significantly different from the contrast group
                 - pvalue_adj: p-value after multiple testing correction
                 - significant_adj: whether the group is significantly different from the contrast group after multiple testing correction
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.distance_example_data()
-            >>> distance_test = pt.tl.DistanceTest('edistance', n_perms=1000)
-            >>> test_results = distance_test.test_precomputed(adata, groupby='perturbation', contrast='control')
+            >>> distance_test = pt.tl.DistanceTest("edistance", n_perms=1000)
+            >>> test_results = distance_test.test_precomputed(adata, groupby="perturbation", contrast="control")
         """
         if not self.distance.metric_fct.accepts_precomputed:
             raise ValueError(f"Metric {self.metric} does not accept precomputed distances.")
 
         groups = adata.obs[groupby].unique()
         if contrast not in groups:
             raise ValueError(f"Contrast group {contrast} not found in {groupby} of adata.obs.")
```

### Comparing `pertpy-0.6.0/pertpy/tools/_distances/_distances.py` & `pertpy-0.7.0/pertpy/tools/_distances/_distances.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
+import numba
 import numpy as np
 import pandas as pd
 from ott.geometry.geometry import Geometry
 from ott.geometry.pointcloud import PointCloud
 from ott.problems.linear.linear_problem import LinearProblem
 from ott.solvers.linear.sinkhorn import Sinkhorn
+from pandas import Series
 from rich.progress import track
 from scipy.sparse import issparse
 from scipy.spatial.distance import cosine
 from scipy.special import gammaln
-from scipy.stats import kendalltau, pearsonr, spearmanr
+from scipy.stats import kendalltau, kstest, pearsonr, spearmanr
+from sklearn.linear_model import LogisticRegression
 from sklearn.metrics import pairwise_distances, r2_score
 from sklearn.metrics.pairwise import polynomial_kernel, rbf_kernel
 from statsmodels.discrete.discrete_model import NegativeBinomialP
 
 if TYPE_CHECKING:
-    from collections.abc import Iterable
-
     from anndata import AnnData
 
 
 class Distance:
     """Distance class, used to compute distances between groups of cells.
 
     The distance metric can be specified by the user. This class also provides a
     method to compute the pairwise distances between all groups of cells.
     Currently available metrics:
+
     - "edistance": Energy distance (Default metric).
         In essence, it is twice the mean pairwise distance between cells of two
         groups minus the mean pairwise distance between cells within each group
         respectively. More information can be found in
         `Peidli et al. (2023) <https://doi.org/10.1101/2022.08.20.504663>`__.
     - "euclidean": euclidean distance.
         Euclidean distance between the means of cells from two groups.
@@ -51,33 +53,37 @@
         Kendall tau distance between the means of cells from two groups.
     - "cosine_distance": Cosine distance.
         Cosine distance between the means of cells from two groups.
     - "r2_distance": coefficient of determination distance.
         Coefficient of determination distance between the means of cells from two groups.
     - "mean_pairwise": Mean pairwise distance.
         Mean of the pairwise euclidean distances between cells of two groups.
-    - "mean_pairwise": Mean pairwise distance.
-        Mean of the pairwise euclidean distances between cells of two groups.
     - "mmd": Maximum mean discrepancy
         Maximum mean discrepancy between the cells of two groups.
         Here, uses linear, rbf, and quadratic polynomial MMD. For theory on MMD in single-cell applications, see
         `Lotfollahi et al. (2019) <https://doi.org/10.48550/arXiv.1910.01791>`__.
     - "wasserstein": Wasserstein distance (Earth Mover's Distance)
         Wasserstein distance between the cells of two groups. Uses an
         OTT-JAX implementation of the Sinkhorn algorithm to compute the distance.
         For more information on the optimal transport solver, see
         `Cuturi et al. (2013) <https://proceedings.neurips.cc/paper/2013/file/af21d0c97db2e27e13572cbf59eb343d-Paper.pdf>`__.
-    - "kl_divergence": Kullback–Leibler divergence distance.
+    - "sym_kldiv": symmetrized Kullback–Leibler divergence distance.
         Kullback–Leibler divergence of the gaussian distributions between cells of two groups.
-        Here we fit a gaussian distribution over each group of cells and then calculate the KL divergence
+        Here we fit a gaussian distribution over one group of cells and then calculate the KL divergence on the other, and vice versa.
     - "t_test": t-test statistic.
         T-test statistic measure between cells of two groups.
+    - "ks_test": Kolmogorov-Smirnov test statistic.
+        Kolmogorov-Smirnov test statistic measure between cells of two groups.
     - "nb_ll": log-likelihood over negative binomial
         Average of log-likelihoods of samples of the secondary group after fitting a negative binomial distribution
         over the samples of the first group.
+    - "classifier_proba": probability of a binary classifier
+        Average of the classification probability of the perturbation for a binary classifier.
+    - "classifier_cp": classifier class projection
+        Average of the class
 
     Attributes:
         metric: Name of distance metric.
         layer_key: Name of the counts to use in adata.layers.
         obsm_key: Name of embedding in adata.obsm to use.
         cell_wise_metric: Metric from scipy.spatial.distance to use for pairwise distances between single cells.
 
@@ -133,20 +139,26 @@
             metric_fct = R2ScoreDistance()
         elif metric == "mean_pairwise":
             metric_fct = MeanPairwiseDistance()
         elif metric == "mmd":
             metric_fct = MMD()
         elif metric == "wasserstein":
             metric_fct = WassersteinDistance()
-        elif metric == "kl_divergence":
-            metric_fct = KLDivergence()
+        elif metric == "sym_kldiv":
+            metric_fct = SymmetricKLDivergence()
         elif metric == "t_test":
             metric_fct = TTestDistance()
+        elif metric == "ks_test":
+            metric_fct = KSTestDistance()
         elif metric == "nb_ll":
             metric_fct = NBLL()
+        elif metric == "classifier_proba":
+            metric_fct = ClassifierProbaDistance()
+        elif metric == "classifier_cp":
+            metric_fct = ClassifierClassProjection()
         else:
             raise ValueError(f"Metric {metric} not recognized.")
         self.metric_fct = metric_fct
 
         if layer_key and obsm_key:
             raise ValueError(
                 "Cannot use 'counts_layer_key' and 'obsm_key' at the same time.\n"
@@ -276,15 +288,15 @@
         groupby: str,
         selected_group: str | None = None,
         groups: list[str] | None = None,
         show_progressbar: bool = True,
         n_jobs: int = -1,
         **kwargs,
     ) -> pd.DataFrame:
-        """Get pairwise distances between groups of cells.
+        """Get distances between one selected cell group and the remaining other cell groups.
 
         Args:
             adata: Annotated data matrix.
             groupby: Column name in adata.obs.
             selected_group: Group to compute pairwise distances to all other.
             groups: List of groups to compute distances to selected_group for.
                     If None, uses all groups. Defaults to None.
@@ -297,14 +309,19 @@
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.distance_example()
             >>> Distance = pt.tools.Distance(metric="edistance")
             >>> pairwise_df = Distance.onesided_distances(adata, groupby="perturbation", selected_group="control")
         """
+        if self.metric == "classifier_cp":
+            return self.metric_fct.onesided_distances(  # type: ignore
+                adata, groupby, selected_group, groups, show_progressbar, n_jobs, **kwargs
+            )
+
         groups = adata.obs[groupby].unique() if groups is None else groups
         grouping = adata.obs[groupby].copy()
         df = pd.Series(index=groups, dtype=float)
         fct = track if show_progressbar else lambda iterable: iterable
 
         # Some metrics are able to handle precomputed distances. This means that
         # the pairwise distances between all cells are computed once and then
@@ -325,23 +342,26 @@
                     idx_y = grouping == group_y
                     # subset the pairwise distance matrix to the two groups
                     sub_pwd = pwd[idx_x | idx_y, :][:, idx_x | idx_y]
                     sub_idx = grouping[idx_x | idx_y] == group_x
                     dist = self.metric_fct.from_precomputed(sub_pwd, sub_idx, **kwargs)
                 df.loc[group_x] = dist
         else:
-            embedding = adata.obsm[self.obsm_key].copy()
+            if self.layer_key:
+                embedding = adata.layers[self.layer_key]
+            else:
+                embedding = adata.obsm[self.obsm_key].copy()
             for group_x in fct(groups):
                 cells_x = embedding[grouping == group_x].copy()
                 group_y = selected_group
                 if group_x == group_y:
                     dist = 0.0
                 else:
                     cells_y = embedding[grouping == group_y].copy()
-                    dist = self.metric_fct(cells_x, cells_y, **kwargs)
+                    dist = self(cells_x, cells_y, **kwargs)
                 df.loc[group_x] = dist
         df.index.name = groupby
         df.name = f"{self.metric} to {selected_group}"
         return df
 
     def precompute_distances(self, adata: AnnData, n_jobs: int = -1) -> None:
         """Precompute pairwise distances between all cells, writes to adata.obsp.
@@ -467,19 +487,16 @@
         return self.solve_ot_problem(geom, **kwargs)
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
         geom = Geometry(cost_matrix=P[idx, :][:, ~idx])
         return self.solve_ot_problem(geom, **kwargs)
 
     def solve_ot_problem(self, geom: Geometry, **kwargs):
-        # Define a linear problem with that cost structure.
         ot_prob = LinearProblem(geom)
-        # Create a Sinkhorn solver
         solver = Sinkhorn()
-        # Solve OT problem
         ot = solver(ot_prob, **kwargs)
         return ot.reg_ot_cost.item()
 
 
 class EuclideanDistance(AbstractDistance):
     """Euclidean distance between pseudobulk vectors."""
 
@@ -498,29 +515,29 @@
     """Mean squared distance between pseudobulk vectors."""
 
     def __init__(self) -> None:
         super().__init__()
         self.accepts_precomputed = False
 
     def __call__(self, X: np.ndarray, Y: np.ndarray, **kwargs) -> float:
-        return np.linalg.norm(X.mean(axis=0) - Y.mean(axis=0), ord=2, **kwargs) ** 0.5
+        return np.linalg.norm(X.mean(axis=0) - Y.mean(axis=0), ord=2, **kwargs) ** 2 / X.shape[1]
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
         raise NotImplementedError("MeanSquaredDistance cannot be called on a pairwise distance matrix.")
 
 
 class MeanAbsoluteDistance(AbstractDistance):
     """Absolute (Norm-1) distance between pseudobulk vectors."""
 
     def __init__(self) -> None:
         super().__init__()
         self.accepts_precomputed = False
 
     def __call__(self, X: np.ndarray, Y: np.ndarray, **kwargs) -> float:
-        return np.linalg.norm(X.mean(axis=0) - Y.mean(axis=0), ord=1, **kwargs)
+        return np.linalg.norm(X.mean(axis=0) - Y.mean(axis=0), ord=1, **kwargs) / X.shape[1]
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
         raise NotImplementedError("MeanAbsoluteDistance cannot be called on a pairwise distance matrix.")
 
 
 class MeanPairwiseDistance(AbstractDistance):
     """Mean of the pairwise euclidean distance between two groups of cells."""
@@ -610,37 +627,39 @@
     def __call__(self, X: np.ndarray, Y: np.ndarray, **kwargs) -> float:
         return 1 - r2_score(X.mean(axis=0), Y.mean(axis=0))
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
         raise NotImplementedError("R2ScoreDistance cannot be called on a pairwise distance matrix.")
 
 
-class KLDivergence(AbstractDistance):
-    """Average of KL divergence between gene distributions of two groups
+class SymmetricKLDivergence(AbstractDistance):
+    """Average of symmetric KL divergence between gene distributions of two groups
 
     Assuming a Gaussian distribution for each gene in each group, calculates
-    the KL divergence between them and averages over all genes
+    the KL divergence between them and averages over all genes. Repeats this ABBA to get a symmetrized distance.
+    See https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence#Symmetrised_divergence.
 
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.accepts_precomputed = False
 
     def __call__(self, X: np.ndarray, Y: np.ndarray, epsilon=1e-8, **kwargs) -> float:
         kl_all = []
         for i in range(X.shape[1]):
             x_mean, x_std = X[:, i].mean(), X[:, i].std() + epsilon
             y_mean, y_std = Y[:, i].mean(), Y[:, i].std() + epsilon
             kl = np.log(y_std / x_std) + (x_std**2 + (x_mean - y_mean) ** 2) / (2 * y_std**2) - 1 / 2
-            kl_all.append(kl)
+            klr = np.log(x_std / y_std) + (y_std**2 + (y_mean - x_mean) ** 2) / (2 * x_std**2) - 1 / 2
+            kl_all.append(kl + klr)
         return sum(kl_all) / len(kl_all)
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
-        raise NotImplementedError("KLDivergence cannot be called on a pairwise distance matrix.")
+        raise NotImplementedError("SymmetricKLDivergence cannot be called on a pairwise distance matrix.")
 
 
 class TTestDistance(AbstractDistance):
     """Average of T test statistic between two groups assuming unequal variances"""
 
     def __init__(self) -> None:
         super().__init__()
@@ -659,14 +678,31 @@
             t_test_all.append(abs(t))
         return sum(t_test_all) / len(t_test_all)
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
         raise NotImplementedError("TTestDistance cannot be called on a pairwise distance matrix.")
 
 
+class KSTestDistance(AbstractDistance):
+    """Average of two-sided KS test statistic between two groups"""
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.accepts_precomputed = False
+
+    def __call__(self, X: np.ndarray, Y: np.ndarray, **kwargs) -> float:
+        stats = []
+        for i in range(X.shape[1]):
+            stats.append(abs(kstest(X[:, i], Y[:, i])[0]))
+        return sum(stats) / len(stats)
+
+    def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
+        raise NotImplementedError("KSTestDistance cannot be called on a pairwise distance matrix.")
+
+
 class NBLL(AbstractDistance):
     """
     Average of Log likelihood (scalar) of group B cells
     according to a NB distribution fitted over group A
     """
 
     def __init__(self) -> None:
@@ -679,31 +715,145 @@
                 return True
             else:
                 return False
 
         if not _is_count_matrix(matrix=X) or not _is_count_matrix(matrix=Y):
             raise ValueError("NBLL distance only works for raw counts.")
 
-        nlls = []
-        for i in range(X.shape[1]):
-            x, y = X[:, i], Y[:, i]
-            nb_params = NegativeBinomialP(x, np.ones_like(x)).fit(disp=False).params
-            mu = np.repeat(np.exp(nb_params[0]), y.shape[0])
-            theta = np.repeat(1 / nb_params[1], y.shape[0])
-            if mu[0] == np.nan or theta[0] == np.nan:
-                raise ValueError("Could not fit a negative binomial distribution to the input data")
-            # calculate the nll of y
-            eps = np.repeat(epsilon, y.shape[0])
+        @numba.jit(forceobj=True)
+        def _compute_nll(y: np.ndarray, nb_params: tuple[float, float], epsilon: float) -> float:
+            mu = np.exp(nb_params[0])
+            theta = 1 / nb_params[1]
+            eps = epsilon
+
             log_theta_mu_eps = np.log(theta + mu + eps)
             nll = (
                 theta * (np.log(theta + eps) - log_theta_mu_eps)
                 + y * (np.log(mu + eps) - log_theta_mu_eps)
                 + gammaln(y + theta)
                 - gammaln(theta)
                 - gammaln(y + 1)
             )
-            nlls.append(nll.mean())
+            return nll.mean()
+
+        def _process_gene(x: np.ndarray, y: np.ndarray, epsilon: float) -> float:
+            try:
+                nb_params = NegativeBinomialP(x, np.ones_like(x)).fit(disp=False).params
+                return _compute_nll(y, nb_params, epsilon)
+            except np.linalg.linalg.LinAlgError:
+                if x.mean() < 10 and y.mean() < 10:
+                    return 0.0
+                else:
+                    return np.nan  # Use NaN to indicate skipped genes
+
+        nlls = []
+        genes_skipped = 0
+
+        for i in range(X.shape[1]):
+            nll = _process_gene(X[:, i], Y[:, i], epsilon)
+            if np.isnan(nll):
+                genes_skipped += 1
+            else:
+                nlls.append(nll)
+
+        if genes_skipped > X.shape[1] / 2:
+            raise AttributeError(f"{genes_skipped} genes could not be fit, which is over half.")
 
-        return -sum(nlls) / len(nlls)
+        return -np.sum(nlls) / len(nlls)
 
     def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
         raise NotImplementedError("NBLL cannot be called on a pairwise distance matrix.")
+
+
+def _sample(X, frac=None, n=None):
+    """Returns subsample of cells in format (train, test)."""
+    if frac and n:
+        raise ValueError("Cannot pass both frac and n.")
+    if frac:
+        n_cells = max(1, int(X.shape[0] * frac))
+    elif n:
+        n_cells = n
+    else:
+        raise ValueError("Must pass either `frac` or `n`.")
+
+    rng = np.random.default_rng()
+    sampled_indices = rng.choice(X.shape[0], n_cells, replace=False)
+    remaining_indices = np.setdiff1d(np.arange(X.shape[0]), sampled_indices)
+    return X[remaining_indices, :], X[sampled_indices, :]
+
+
+class ClassifierProbaDistance(AbstractDistance):
+    """Average of classification probabilites of a binary classifier.
+
+    Assumes the first condition is control and the second is perturbed.
+    Always holds out 20% of the perturbed condition.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.accepts_precomputed = False
+
+    def __call__(self, X: np.ndarray, Y: np.ndarray, **kwargs) -> float:
+        Y_train, Y_test = _sample(Y, frac=0.2)
+        label = ["c"] * X.shape[0] + ["p"] * Y_train.shape[0]
+        train = np.concatenate([X, Y_train])
+
+        reg = LogisticRegression()
+        reg.fit(train, label)
+        test_labels = reg.predict_proba(Y_test)
+        return np.mean(test_labels[:, 1])
+
+    def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
+        raise NotImplementedError("ClassifierProbaDistance cannot be called on a pairwise distance matrix.")
+
+
+class ClassifierClassProjection(AbstractDistance):
+    """Average of 1-(classification probability of control).
+
+    Warning: unlike all other distances, this must also take a list of categorical labels the same length as X.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.accepts_precomputed = False
+
+    def __call__(self, X: np.ndarray, Y: np.ndarray, **kwargs) -> float:
+        raise NotImplementedError("ClassifierClassProjection can currently only be called with onesided.")
+
+    def onesided_distances(
+        self,
+        adata: AnnData,
+        groupby: str,
+        selected_group: str | None = None,
+        groups: list[str] | None = None,
+        show_progressbar: bool = True,
+        n_jobs: int = -1,
+        **kwargs,
+    ) -> Series:
+        """Unlike the parent function, all groups except the selected group are factored into the classifier.
+
+        Similar to the parent function, the returned dataframe contains only the specified groups.
+        """
+        groups = adata.obs[groupby].unique() if groups is None else groups
+
+        X = adata[adata.obs[groupby] != selected_group].X
+        labels = adata[adata.obs[groupby] != selected_group].obs[groupby].values
+        Y = adata[adata.obs[groupby] == selected_group].X
+
+        reg = LogisticRegression()
+        reg.fit(X, labels)
+        test_probas = reg.predict_proba(Y)
+
+        df = pd.Series(index=groups, dtype=float)
+        for group in groups:
+            if group == selected_group:
+                df.loc[group] = 0
+            else:
+                class_idx = list(reg.classes_).index(group)
+                df.loc[group] = 1 - np.mean(test_probas[:, class_idx])
+        df.index.name = groupby
+        df.name = f"classifier_cp to {selected_group}"
+
+        return df
+
+    def from_precomputed(self, P: np.ndarray, idx: np.ndarray, **kwargs) -> float:
+        raise NotImplementedError("ClassifierClassProjection cannot be called on a pairwise distance matrix.")
```

### Comparing `pertpy-0.6.0/pertpy/tools/_metadata/_cell_line.py` & `pertpy-0.7.0/pertpy/metadata/_cell_line.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,613 +1,826 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import TYPE_CHECKING, Literal
 
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 from rich import print
 from scanpy import settings
+from scipy import stats
 
 from pertpy.data._dataloader import _download
 
 from ._look_up import LookUp
+from ._metadata import MetaData
 
 if TYPE_CHECKING:
     from anndata import AnnData
 
 
-class CellLineMetaData:
+class CellLine(MetaData):
     """Utilities to fetch cell line metadata."""
 
     def __init__(self):
-        settings.cachedir = ".pertpy_cache"
-        # Download cell line metadata from DepMap
-        # Source: https://depmap.org/portal/download/all/ (DepMap Public 22Q2)
-        cell_line_file_path = settings.cachedir.__str__() + "/sample_info.csv"
-        if not Path(cell_line_file_path).exists():
-            print("[bold yellow]No DepMap metadata file found. Starting download now.")
-            _download(
-                url="https://ndownloader.figshare.com/files/35020903",
-                output_file_name="sample_info.csv",
-                output_path=settings.cachedir,
-                block_size=4096,
-                is_zip=False,
-            )
-        self.cell_line_meta = pd.read_csv(cell_line_file_path)
+        super().__init__()
+        self.depmap = None
+        self.cancerxgene = None
+        self.gene_annotation = None
+        self.bulk_rna_sanger = None
+        self.bulk_rna_broad = None
+        self.proteomics = None
+        self.drug_response_gdsc1 = None
+        self.drug_response_gdsc2 = None
 
-        # Download cell line metadata from The Genomics of Drug Sensitivity in Cancer Project
-        # Source: https://www.cancerrxgene.org/celllines
-        cell_line_cancer_project_file_path = settings.cachedir.__str__() + "/cell_line_cancer_project.csv"
-        cell_line_cancer_project_transformed_path = (
-            settings.cachedir.__str__() + "/cell_line_cancer_project_transformed.csv"
-        )
-        if not Path(cell_line_cancer_project_transformed_path).exists():
-            if not Path(cell_line_cancer_project_file_path).exists():
-                print(
-                    "[bold yellow]No cell line metadata file from The Genomics of Drug Sensitivity "
-                    "in Cancer Project found. Starting download now."
-                )
+    def _download_cell_line(self, cell_line_source: Literal["DepMap", "Cancerrxgene"] = "DepMap") -> None:
+        if cell_line_source == "DepMap":
+            # Download cell line metadata from DepMap
+            # Source: https://depmap.org/portal/download/all/ (DepMap Public 23Q4)
+            depmap_cell_line_path = Path(settings.cachedir) / "depmap_23Q4_info.csv"
+            if not Path(depmap_cell_line_path).exists():
+                print("[bold yellow]No DepMap metadata file found. Starting download now.")
                 _download(
-                    url="https://www.cancerrxgene.org/api/celllines?list=all&sEcho=1&iColumns=7&sColumns=&"
-                    "iDisplayStart=0&iDisplayLength=25&mDataProp_0=0&mDataProp_1=1&mDataProp_2=2&mDataProp_3=3&"
-                    "mDataProp_4=4&mDataProp_5=5&mDataProp_6=6&sSearch=&bRegex=false&sSearch_0=&bRegex_0=false&"
-                    "bSearchable_0=true&sSearch_1=&bRegex_1=false&bSearchable_1=true&sSearch_2=&bRegex_2=false&"
-                    "bSearchable_2=true&sSearch_3=&bRegex_3=false&bSearchable_3=true&sSearch_4=&bRegex_4=false&"
-                    "bSearchable_4=true&sSearch_5=&bRegex_5=false&bSearchable_5=true&sSearch_6=&bRegex_6=false&"
-                    "bSearchable_6=true&iSortCol_0=0&sSortDir_0=asc&iSortingCols=1&bSortable_0=true&bSortable_1=true&"
-                    "bSortable_2=true&bSortable_3=true&bSortable_4=true&bSortable_5=true&bSortable_6=true&export=csv",
-                    output_file_name="cell_line_cancer_project.csv",
+                    url="https://ndownloader.figshare.com/files/43746708",
+                    output_file_name="depmap_23Q4_info.csv",
                     output_path=settings.cachedir,
                     block_size=4096,
                     is_zip=False,
                 )
-
-            self.cl_cancer_project_meta = pd.read_csv(cell_line_cancer_project_file_path)
-            self.cl_cancer_project_meta.columns = self.cl_cancer_project_meta.columns.str.strip()
-            self.cl_cancer_project_meta["stripped_cell_line_name"] = self.cl_cancer_project_meta[
-                "Cell line Name"
-            ].str.replace(r"\-|\.", "", regex=True)
-            self.cl_cancer_project_meta["stripped_cell_line_name"] = pd.Categorical(
-                self.cl_cancer_project_meta["stripped_cell_line_name"].str.upper()
-            )
-            # pivot the data frame so that each cell line has only one row of metadata
-            index_col = list(set(self.cl_cancer_project_meta.columns) - {"Datasets", "number of drugs"})
-            self.cl_cancer_project_meta = self.cl_cancer_project_meta.pivot(
-                index=index_col, columns="Datasets", values="number of drugs"
-            )
-            self.cl_cancer_project_meta.columns.name = None
-            self.cl_cancer_project_meta = self.cl_cancer_project_meta.reset_index()
-            self.cl_cancer_project_meta = self.cl_cancer_project_meta.rename(
-                columns={"Cell line Name": "cell_line_name"}
-            )
-            self.cl_cancer_project_meta.to_csv(cell_line_cancer_project_transformed_path)
-
+            self.depmap = pd.read_csv(depmap_cell_line_path)
         else:
-            self.cl_cancer_project_meta = pd.read_csv(cell_line_cancer_project_transformed_path, index_col=0)
+            # Download cell line metadata from The Genomics of Drug Sensitivity in Cancer Project
+            # Source: https://www.cancerrxgene.org/celllines
+            cancerxgene_cell_line_path = Path(settings.cachedir) / "cell_line_cancer_project.csv"
+            transformed_cancerxgene_cell_line_path = Path(settings.cachedir) / "cancerrxgene_info.csv"
+
+            if not Path(transformed_cancerxgene_cell_line_path).exists():
+                if not Path(cancerxgene_cell_line_path).exists():
+                    print(
+                        "[bold yellow]No cell line metadata file from The Genomics of Drug Sensitivity "
+                        "in Cancer Project found. Starting download now."
+                    )
+                    _download(
+                        url="https://www.cancerrxgene.org/api/celllines?list=all&sEcho=1&iColumns=7&sColumns=&"
+                        "iDisplayStart=0&iDisplayLength=25&mDataProp_0=0&mDataProp_1=1&mDataProp_2=2&mDataProp_3=3&"
+                        "mDataProp_4=4&mDataProp_5=5&mDataProp_6=6&sSearch=&bRegex=false&sSearch_0=&bRegex_0=false&"
+                        "bSearchable_0=true&sSearch_1=&bRegex_1=false&bSearchable_1=true&sSearch_2=&bRegex_2=false&"
+                        "bSearchable_2=true&sSearch_3=&bRegex_3=false&bSearchable_3=true&sSearch_4=&bRegex_4=false&"
+                        "bSearchable_4=true&sSearch_5=&bRegex_5=false&bSearchable_5=true&sSearch_6=&bRegex_6=false&"
+                        "bSearchable_6=true&iSortCol_0=0&sSortDir_0=asc&iSortingCols=1&bSortable_0=true&bSortable_1=true&"
+                        "bSortable_2=true&bSortable_3=true&bSortable_4=true&bSortable_5=true&bSortable_6=true&export=csv",
+                        output_file_name="cell_line_cancer_project.csv",
+                        output_path=settings.cachedir,
+                        block_size=4096,
+                        is_zip=False,
+                    )
+                self.cancerxgene = pd.read_csv(cancerxgene_cell_line_path)
+                self.cancerxgene.columns = self.cancerxgene.columns.str.strip()
+                self.cancerxgene["stripped_cell_line_name"] = (
+                    self.cancerxgene["Cell line Name"]
+                    .str.replace(r"\-|\.", "", regex=True)
+                    .str.upper()
+                    .astype("category")
+                )
+                # pivot the data frame so that each cell line has only one row of metadata
+                index_col = set(self.cancerxgene.columns) - {
+                    "Datasets",
+                    "number of drugs",
+                }
+                self.cancerxgene = self.cancerxgene.pivot(index=index_col, columns="Datasets", values="number of drugs")
+                self.cancerxgene.columns.name = None
+                self.cancerxgene = self.cancerxgene.reset_index().rename(columns={"Cell line Name": "cell_line_name"})
+                self.cancerxgene.to_csv(transformed_cancerxgene_cell_line_path)
+            else:
+                self.cancerxgene = pd.read_csv(transformed_cancerxgene_cell_line_path, index_col=0)
 
+    def _download_gene_annotation(self) -> None:
         # Download metadata for driver genes from DepMap.Sanger
         # Source: https://cellmodelpassports.sanger.ac.uk/downloads (Gene annotation)
-        gene_annotation_file_path = settings.cachedir.__str__() + "/gene_identifiers_20191101.csv"
+        gene_annotation_file_path = Path(settings.cachedir) / "genes_info.csv"
         if not Path(gene_annotation_file_path).exists():
-            print("[bold yellow]No metadata file was found for gene annotation." " Starting download now.")
+            print("[bold yellow]No metadata file was found for gene annotation. Starting download now.")
             _download(
                 url="https://cog.sanger.ac.uk/cmp/download/gene_identifiers_20191101.csv",
-                output_file_name="gene_identifiers_20191101.csv",
+                output_file_name="genes_info.csv",
                 output_path=settings.cachedir,
                 block_size=4096,
                 is_zip=False,
             )
         self.gene_annotation = pd.read_table(gene_annotation_file_path, delimiter=",")
 
-        # Download bulk RNA-seq data collated by the Wellcome Sanger Institute and the Broad Institute from DepMap.Sanger
-        # Source: https://cellmodelpassports.sanger.ac.uk/downloads (Expression data)
-        # issue: read count values contain random whitespace, not sure what it supposes to mean
-        # solution: remove the white space and convert to int before depmap updates the metadata
-        bulk_rna_sanger_file_path = settings.cachedir.__str__() + "/rnaseq_read_count_20220624_processed.csv"
-        if not Path(bulk_rna_sanger_file_path).exists():
-            print(
-                "[bold yellow]No metadata file was found for bulk RNA-seq data of Sanger cell line."
-                " Starting download now..."
-            )
-            _download(
-                url="https://figshare.com/ndownloader/files/42467103",
-                output_file_name="rnaseq_read_count_20220624_processed.csv",
-                output_path=settings.cachedir,
-                block_size=4096,
-                is_zip=False,
-            )
-        self.bulk_rna_sanger = pd.read_csv(bulk_rna_sanger_file_path, index_col=0)
-
-        # Download CCLE expression data from DepMap
-        # Source: https://depmap.org/portal/download/all/ (DepMap Public 22Q2)
-        bulk_rna_broad_file_path = settings.cachedir.__str__() + "/CCLE_expression_full.csv"
-        if not Path(bulk_rna_broad_file_path).exists():
-            print("[bold yellow]No metadata file was found for CCLE expression data. Starting download now.")
-            _download(
-                url="https://figshare.com/ndownloader/files/34989922",
-                output_file_name="CCLE_expression_full.csv",
-                output_path=settings.cachedir,
-                block_size=4096,
-                is_zip=False,
-            )
-        self.bulk_rna_broad = pd.read_csv(bulk_rna_broad_file_path, index_col=0)
+    def _download_bulk_rna(self, cell_line_source: Literal["broad", "sanger"] = "broad") -> None:
+        if cell_line_source == "sanger":
+            # Download bulk RNA-seq data collated by the Wellcome Sanger Institute and the Broad Institute from DepMap.Sanger
+            # Source: https://cellmodelpassports.sanger.ac.uk/downloads (Expression data)
+            # issue: read count values contain random whitespace
+            # solution: remove the white space and convert to int before depmap updates the metadata
+            bulk_rna_sanger_file_path = Path(settings.cachedir) / "rnaseq_sanger_info.csv"
+            if not Path(bulk_rna_sanger_file_path).exists():
+                print(
+                    "[bold yellow]No metadata file was found for bulk RNA-seq data of Sanger cell line."
+                    " Starting download now."
+                )
+                _download(
+                    url="https://figshare.com/ndownloader/files/42467103",
+                    output_file_name="rnaseq_sanger_info.csv",
+                    output_path=settings.cachedir,
+                    block_size=4096,
+                    is_zip=False,
+                )
+            self.bulk_rna_sanger = pd.read_csv(bulk_rna_sanger_file_path, index_col=0, dtype="unicode")
+        else:
+            # Download CCLE expression data from DepMap
+            # Source: https://depmap.org/portal/download/all/ (DepMap Public 22Q2)
+            bulk_rna_broad_file_path = Path(settings.cachedir) / "rnaseq_depmap_info.csv"
+            if not Path(bulk_rna_broad_file_path).exists():
+                print("[bold yellow]No metadata file was found for CCLE expression data. Starting download now.")
+                _download(
+                    url="https://figshare.com/ndownloader/files/34989922",
+                    output_file_name="rnaseq_depmap_info.csv",
+                    output_path=settings.cachedir,
+                    block_size=4096,
+                    is_zip=False,
+                )
+            self.bulk_rna_broad = pd.read_csv(bulk_rna_broad_file_path, index_col=0)
 
+    def _download_proteomics(self) -> None:
         # Download proteomics data processed by DepMap.Sanger
         # Source: https://cellmodelpassports.sanger.ac.uk/downloads (Proteomics)
-        proteomics_file_path = settings.cachedir.__str__() + "/proteomics_all_20221214_processed.csv"
+        proteomics_file_path = Path(settings.cachedir) / "proteomics_info.csv"
         if not Path(proteomics_file_path).exists():
             print("[bold yellow]No metadata file was found for proteomics data (DepMap.Sanger). Starting download now.")
             _download(
                 url="https://figshare.com/ndownloader/files/42468393",
-                output_file_name="proteomics_all_20221214_processed.csv",
-                output_path=settings.cachedir,
-                block_size=4096,
-                is_zip=False,
-            )
-        self.proteomics_data = pd.read_csv(proteomics_file_path, index_col=0)
-
-        # Download GDSC drug response data
-        # Source: https://www.cancerrxgene.org/downloads/bulk_download (Drug Screening - IC50s)
-        drug_response_gdsc1_file_path = settings.cachedir.__str__() + "/ic50_gdsc1.xlsx"
-        if not Path(drug_response_gdsc1_file_path).exists():
-            print(
-                "[bold yellow]No metadata file was found for drug response data of GDSC1 dataset."
-                " Starting download now."
-            )
-            _download(
-                url="https://cog.sanger.ac.uk/cancerrxgene/GDSC_release8.4/GDSC1_fitted_dose_response_24Jul22.xlsx",
-                output_file_name="ic50_gdsc1.xlsx",
+                output_file_name="proteomics_info.csv",
                 output_path=settings.cachedir,
                 block_size=4096,
                 is_zip=False,
             )
-        self.drug_response_gdsc1 = pd.read_excel(drug_response_gdsc1_file_path)
-        self.drug_response_gdsc1 = self.drug_response_gdsc1.iloc[:, [3, 4, 5, 7, 8, 15, 16]]
-        self.drug_response_gdsc1.rename(columns=lambda col: col.lower(), inplace=True)
-        self.drug_response_gdsc1 = self.drug_response_gdsc1.loc[
-            self.drug_response_gdsc1.groupby(["cell_line_name", "drug_name"])["auc"].idxmax()
-        ]
-        self.drug_response_gdsc1 = self.drug_response_gdsc1.reset_index(drop=True)
+        self.proteomics = pd.read_csv(proteomics_file_path, index_col=0)
 
-        drug_response_gdsc2_file_path = settings.cachedir.__str__() + "/ic50_gdsc2.xlsx"
-        if not Path(drug_response_gdsc2_file_path).exists():
-            print(
-                "[bold yellow]No metadata file was found for drug response data of GDSC2 dataset."
-                " Starting download now."
-            )
-            _download(
-                url="https://cog.sanger.ac.uk/cancerrxgene/GDSC_release8.4/GDSC2_fitted_dose_response_24Jul22.xlsx",
-                output_file_name="ic50_gdsc2.xlsx",
-                output_path=settings.cachedir,
-                block_size=4096,
-                is_zip=False,
-            )
-        self.drug_response_gdsc2 = pd.read_excel(drug_response_gdsc2_file_path)
-        self.drug_response_gdsc2 = self.drug_response_gdsc2.iloc[:, [3, 4, 5, 7, 8, 15, 16]]
-        self.drug_response_gdsc2.rename(columns=lambda col: col.lower(), inplace=True)
-        self.drug_response_gdsc2 = self.drug_response_gdsc2.loc[
-            self.drug_response_gdsc2.groupby(["cell_line_name", "drug_name"])["auc"].idxmax()
-        ]
-        self.drug_response_gdsc2 = self.drug_response_gdsc2.reset_index(drop=True)
+    def _download_gdsc(self, gdsc_dataset: Literal[1, 2] = 1) -> None:
+        if gdsc_dataset == 1:
+            # Download GDSC drug response data
+            # Source: https://www.cancerrxgene.org/downloads/bulk_download (Drug Screening - IC50s)
+            # URL: https://cog.sanger.ac.uk/cancerrxgene/GDSC_release8.4/GDSC1_fitted_dose_response_24Jul22.xlsx
+            drug_response_gdsc1_file_path = Path(settings.cachedir) / "gdsc1_info.csv"
+            if not Path(drug_response_gdsc1_file_path).exists():
+                print(
+                    "[bold yellow]No metadata file was found for drug response data of GDSC1 dataset."
+                    " Starting download now."
+                )
+                _download(
+                    url="https://figshare.com/ndownloader/files/43757235",
+                    output_file_name="gdsc1_info.csv",
+                    output_path=settings.cachedir,
+                    block_size=4096,
+                    is_zip=False,
+                )
+            self.drug_response_gdsc1 = pd.read_csv(drug_response_gdsc1_file_path, index_col=0)
+        if gdsc_dataset == 2:
+            drug_response_gdsc2_file_path = Path(settings.cachedir) / "gdsc2_info.csv"
+            if not Path(drug_response_gdsc2_file_path).exists():
+                print(
+                    "[bold yellow]No metadata file was found for drug response data of GDSC2 dataset."
+                    " Starting download now."
+                )
+                _download(
+                    url="https://figshare.com/ndownloader/files/43757232",
+                    output_file_name="gdsc2_info.csv",
+                    output_path=settings.cachedir,
+                    block_size=4096,
+                    is_zip=False,
+                )
+            self.drug_response_gdsc2 = pd.read_csv(drug_response_gdsc2_file_path, index_col=0)
 
-    def annotate_cell_lines(
+    def annotate(
         self,
         adata: AnnData,
         query_id: str = "DepMap_ID",
-        reference_id: str = "DepMap_ID",
-        cell_line_information: list[str] | None = None,
+        reference_id: str = "ModelID",
+        fetch: list[str] | None = None,
         cell_line_source: Literal["DepMap", "Cancerrxgene"] = "DepMap",
+        verbosity: int | str = 5,
         copy: bool = False,
     ) -> AnnData:
-        """Fetch cell line annotation.
+        """Annotate cell lines.
 
-        For each cell, we fetch cell line annotation from Dependency Map (DepMap).
+        For each cell, we fetch cell line annotation from either the Dependency Map (DepMap) or The Genomics of Drug Sensitivity in Cancer Project (Cancerxgene).
 
         Args:
             adata: The data object to annotate.
             query_id: The column of `.obs` with cell line information. Defaults to "DepMap_ID".
-            reference_id: The type of cell line identifier in the meta data, e.g. DepMap_ID, cell_line_name or
-                stripped_cell_line_name. If fetch cell line metadata from Cancerrxgene, it is recommended to choose
-                "stripped_cell_line_name". Defaults to "DepMap_ID".
-            cell_line_information: The metadata to fetch. All metadata will be fetched by default. Defaults to None (=all).
+            reference_id: The type of cell line identifier in the meta data, e.g. ModelID, CellLineName	or StrippedCellLineName.
+                          If fetching cell line metadata from Cancerrxgene, it is recommended to choose
+                          "stripped_cell_line_name". Defaults to "ModelID".
+            fetch: The metadata to fetch. Defaults to None (=all).
             cell_line_source: The source of cell line metadata, DepMap or Cancerrxgene. Defaults to "DepMap".
+            verbosity: The number of unmatched identifiers to print, can be either non-negative values or "all".
+                       Defaults to 5.
             copy: Determines whether a copy of the `adata` is returned. Defaults to False.
 
         Returns:
             Returns an AnnData object with cell line annotation.
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.dialogue_example()
-            >>> adata.obs['cell_line_name'] = 'MCF7'
-            >>> pt_metadata = pt.tl.CellLineMetaData()
-            >>> adata_annotated = pt_metadata.annotate_cell_lines(adata=adata, reference_id='cell_line_name', query_id='cell_line_name', copy=True)
+            >>> adata.obs["cell_line_name"] = "MCF7"
+            >>> pt_metadata = pt.md.CellLine()
+            >>> adata_annotated = pt_metadata.annotate(adata=adata,
+            >>>                                        reference_id='cell_line_name',
+            >>>                                        query_id='cell_line_name',
+            >>>                                        fetch=["cell_line_name", "age", "primary_disease"],
+            >>>                                        copy=True)
         """
         if copy:
             adata = adata.copy()
 
         if cell_line_source == "DepMap":
-            cell_line_meta = self.cell_line_meta
+            if self.depmap is None:
+                self._download_cell_line(cell_line_source="DepMap")
+            cell_line_meta = self.depmap
         else:
             reference_id = "stripped_cell_line_name"
             if query_id == "DepMap_ID":
                 query_id = "stripped_cell_line_name"
                 print(
-                    "[bold blue]`stripped_cell_line_name` is used as reference and query indentifier ",
+                    "[bold blue]`stripped_cell_line_name` is used as reference and query identifier ",
                     " to annotate cell line metadata from Cancerrxgene. "
-                    "So please make sure that `stripped_cell_line_name` is available in the adata.obs. ",
+                    "Ensure that stripped cell line names are available in 'adata.obs.' ",
                     "or use the DepMap as `cell_line_source` to annotate the cell line first ",
                 )
-            cell_line_meta = self.cl_cancer_project_meta
+            if self.cancerxgene is None:
+                self._download_cell_line(cell_line_source="Cancerrxgene")
+            cell_line_meta = self.cancerxgene
 
         if query_id not in adata.obs.columns:
-            raise ValueError(f"The requested query_id {query_id} is not in `adata.obs`. \n" "Please check again. ")
+            raise ValueError(f"The requested query_id {query_id} is not in `adata.obs`.")
 
         if reference_id in cell_line_meta.columns:
             # If the specified cell line type can be found in the database,
             # we can compare these keys and fetch the corresponding metadata.
             identifier_num_all = len(adata.obs[query_id].unique())
             not_matched_identifiers = list(set(adata.obs[query_id]) - set(cell_line_meta[reference_id]))
-            if len(not_matched_identifiers) == identifier_num_all:
-                raise ValueError(
-                    f"Attempting to match the query id {query_id} in the adata.obs to the reference id {reference_id} in the metadata.\n"
-                    "However, none of the query IDs could be found in the cell line annotation data.\n"
-                    "The annotation process has been halted.\n"
-                    "To resolve this issue, please call the `CellLineMetaData.lookup()` function to create a LookUp object.\n"
-                    "By using the `LookUp.cell_line()` method, "
-                    "you can obtain the count of matched identifiers in the adata for different types of reference IDs and query IDs."
-                )
 
-            if len(not_matched_identifiers) > 0:
-                print(
-                    f"[bold blue]There are {identifier_num_all} identifiers in `adata.obs`."
-                    f"However, {len(not_matched_identifiers)} identifiers can't be found in the cell line annotation,"
-                    "leading to the presence of NA values for their respective metadata.\n",
-                    "Please check again: ",
-                    *not_matched_identifiers,
-                    sep="\n- ",
-                )
-
-            if cell_line_information is None:
-                # If no cell_line_information is specified, all metadata is fetched by default.
-                # Sometimes there is already different cell line information in the AnnData object.
-                # To avoid redundant information we will remove the duplicate information from metadata after merging.
-                adata.obs = (
-                    adata.obs.merge(
-                        cell_line_meta,
-                        left_on=query_id,
-                        right_on=reference_id,
-                        how="left",
-                        suffixes=("", "_fromMeta"),
-                    )
-                    .filter(regex="^(?!.*_fromMeta)")
-                    .set_index(adata.obs.index)
-                )
-                # If query_id and reference_id have different names,
-                # there will be a column for each of them after merging,
-                # which is redundant as they refer to the same information.
-                # We will move the reference_id column.
-                if query_id != reference_id:
-                    del adata.obs[reference_id]
+            self._warn_unmatch(
+                total_identifiers=identifier_num_all,
+                unmatched_identifiers=not_matched_identifiers,
+                query_id=query_id,
+                reference_id=reference_id,
+                metadata_type="cell line",
+                verbosity=verbosity,
+            )
 
-            elif set(cell_line_information).issubset(set(cell_line_meta.columns)):
-                # If cell_line_information is specified and can be found in the DepMap database,
+            if fetch is not None:
+                # If fetch is specified and can be found in the DepMap database,
                 # We will subset the original metadata dataframe correspondingly and add them to the AnnData object.
-                # Again, redundant information will be removed.
-                if reference_id not in cell_line_information:
-                    cell_line_information.append(reference_id)
-                cell_line_meta_part = cell_line_meta[cell_line_information]
-                adata.obs = (
-                    adata.obs.merge(
-                        cell_line_meta_part,
-                        left_on=query_id,
-                        right_on=reference_id,
-                        how="left",
-                        suffixes=("", "_fromMeta"),
+                # Redundant information will be removed.
+                if set(fetch).issubset(set(cell_line_meta.columns)):
+                    if reference_id not in fetch:
+                        fetch.append(reference_id)
+                else:
+                    raise ValueError(
+                        "Selected cell line information is not present in the metadata.\n"
+                        "Please create a `CellLineMetaData.lookup()` object to obtain the available cell line information in the metadata."
                     )
-                    .filter(regex="^(?!.*_fromMeta)")
-                    .set_index(adata.obs.index)
+
+            # If no fetch is specified, all metadata is fetched by default.
+            # Sometimes there is already different cell line information in the AnnData object.
+            # To avoid redundant information we will remove duplicate information from metadata after merging.
+            adata.obs = (
+                adata.obs.merge(
+                    cell_line_meta if fetch is None else cell_line_meta[fetch],
+                    left_on=query_id,
+                    right_on=reference_id,
+                    how="left",
+                    suffixes=("", "_fromMeta"),
                 )
-                # Again, redundant information will be removed.
-                if query_id != reference_id:
-                    del adata.obs[reference_id]
+                .filter(regex="^(?!.*_fromMeta)")
+                .set_index(adata.obs.index)
+            )
+            # If query_id and reference_id have different names,
+            # there will be a column for each of them after merging,
+            # which is redundant as they refer to the same information.
+            # We will move the reference_id column.
+            if query_id != reference_id:
+                del adata.obs[reference_id]
 
         else:
             raise ValueError(
                 f"The requested cell line type {reference_id} is currently unavailable in the database.\n"
-                "To solve ths issue, please refer to the available reference identifier in the chosen database.\n"
+                "Refer to the available reference identifier in the chosen database.\n"
                 "DepMap_ID is compared by default.\n"
-                "Alternatively, you can call the `CellLineMetaData.lookup()` function to create a LookUp object.\n"
-                "By using the `LookUp.cell_line()` method, you can obtain the available reference identifiers in the metadata."
+                "Alternatively, create a `CellLineMetaData.lookup()` object to "
+                "obtain the available reference identifiers in the metadata."
             )
 
         return adata
 
-    def annotate_bulk_rna_expression(
+    def annotate_bulk_rna(
         self,
         adata: AnnData,
         query_id: str = "cell_line_name",
         cell_line_source: Literal["broad", "sanger"] = "sanger",
+        verbosity: int | str = 5,
+        gene_identifier: Literal["gene_name", "gene_ID", "both"] = "gene_ID",
         copy: bool = False,
     ) -> AnnData:
-        """Fetch bulk rna expression.
+        """Fetch bulk rna expression from the Broad or Sanger.
 
         For each cell, we fetch bulk rna expression from either Broad or Sanger cell line.
 
         Args:
             adata: The data object to annotate.
             query_id: The column of `.obs` with cell line information. Defaults to "cell_line_name" if `cell_line_source` is sanger, otherwise "DepMap_ID".
             cell_line_source: The bulk rna expression data from either broad or sanger cell line. Defaults to "sanger".
+            verbosity: The number of unmatched identifiers to print, can be either non-negative values or "all". Defaults to 5.
             copy: Determines whether a copy of the `adata` is returned. Defaults to False.
 
         Returns:
             Returns an AnnData object with bulk rna expression annotation.
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.dialogue_example()
-            >>> adata.obs['cell_line_name'] = 'MCF7'
-            >>> pt_metadata = pt.tl.CellLineMetaData()
-            >>> adata_annotated = pt_metadata.annotate_cell_lines(adata=adata, reference_id='cell_line_name', query_id='cell_line_name', copy=True)
-            >>> pt_metadata.annotate_bulk_rna_expression(adata_annotated)
+            >>> adata.obs["cell_line_name"] = "MCF7"
+            >>> pt_metadata = pt.md.CellLine()
+            >>> adata_annotated = pt_metadata.annotate(
+            ...     adata=adata, reference_id="cell_line_name", query_id="cell_line_name", copy=True
+            ... )
+            >>> pt_metadata.annotate_bulk_rna(adata_annotated)
         """
         if copy:
             adata = adata.copy()
 
         # Make sure that the specified `cell_line_type` can be found in the bulk rna expression data,
         # then we can compare these keys and fetch the corresponding metadata.
         if query_id not in adata.obs.columns:
             raise ValueError(
                 f"The specified `query_id` {query_id} can't be found in the `adata.obs`.\n"
-                "Please ensure that you are using one of the available query IDs present in the adata.obs for the annotation.\n"
+                "Ensure that you are using one of the available query IDs present in the adata.obs for the annotation.\n"
                 "If the desired query ID is not available, you can fetch the cell line metadata "
-                "using the `annotate_cell_lines()` function before calling annotate_ccle_expression(). "
-                "This will help ensure that the required query ID is included in your data, e.g. stripped_cell_line_name, DepMap ID."
+                "using the `annotate()` function before calling 'annotate_bulk_rna()'. "
+                "This ensures that the required query ID is included in your data, e.g. stripped_cell_line_name, DepMap ID."
             )
 
         identifier_num_all = len(adata.obs[query_id].unique())
+
+        # Lazily download the bulk rna expression data
         if cell_line_source == "sanger":
+            if self.bulk_rna_sanger is None:
+                self._download_bulk_rna(cell_line_source="sanger")
             reference_id = "model_name"
             not_matched_identifiers = list(set(adata.obs[query_id]) - set(self.bulk_rna_sanger.index))
         else:
             reference_id = "DepMap_ID"
             print(
-                "To annotate bulk RNA expression data from Broad Institue, ",
-                "`DepMap_ID` is used as default reference and query indentifier if no `reference_id` is given. ",
-                "Please make sure that `DepMap_ID` is available in the adata.obs. ",
-                "Alternatively, use the `annotate_cell_lines()` function to annotate the cell line first ",
+                "To annotate bulk RNA data from Broad Institue, ",
+                "`DepMap_ID` is used as default reference and query identifier if no `reference_id` is given. ",
+                "Ensure that `DepMap_ID` is available in 'adata.obs'. ",
+                "Alternatively, use `annotate()` to annotate the cell line first ",
             )
-
+            if self.bulk_rna_broad is None:
+                self._download_bulk_rna(cell_line_source="broad")
             if query_id == "cell_line_name":
                 query_id = "DepMap_ID"
             not_matched_identifiers = list(set(adata.obs[query_id]) - set(self.bulk_rna_broad.index))
 
-        if len(not_matched_identifiers) == identifier_num_all:
-            raise ValueError(
-                f"You are attempting to match the query id {query_id} in the adata.obs to the reference id {reference_id} in the metadata."
-                "However, none of the query IDs could be found in the bulk RNA expression data.\n"
-                "The annotation process has been halted.\n"
-                "To resolve this issue, please call the `CellLineMetaData.lookup()` function to create a LookUp object.\n"
-                "By using the `LookUp.bulk_rna_expression()` method, "
-                "you can obtain the count of matched identifiers in the adata for different types of reference IDs and query IDs.\n"
-                "Additionally, you can call the `CellLineMetaData.annotate_cell_lines()` function "
-                "to acquire more possible query IDs that can be used for annotation purposes."
-            )
+        self._warn_unmatch(
+            total_identifiers=identifier_num_all,
+            unmatched_identifiers=not_matched_identifiers,
+            query_id=query_id,
+            reference_id=reference_id,
+            metadata_type="bulk RNA",
+            verbosity=verbosity,
+        )
 
-        if len(not_matched_identifiers) > 0:
-            print(f"There are {identifier_num_all} identifiers in `adata.obs`.")
-            print(
-                f"[bold yellow]Following {len(not_matched_identifiers)} identifiers can't be found in bulk RNA expression data, "
-            )
-            print(
-                "leading to the presence of NA values for their respective metadata. Please check again: ",
-                *not_matched_identifiers,
-                sep="\n- ",
-            )
         if cell_line_source == "sanger":
             sanger_rna_exp = self.bulk_rna_sanger[self.bulk_rna_sanger.index.isin(adata.obs[query_id])]
             sanger_rna_exp = sanger_rna_exp.reindex(adata.obs[query_id])
             sanger_rna_exp.index = adata.obs.index
-            adata.obsm["bulk_rna_expression_sanger"] = sanger_rna_exp
+            adata.obsm["bulk_rna_sanger"] = sanger_rna_exp
         else:
+            if gene_identifier == "gene_ID":
+                self.bulk_rna_broad.columns = [
+                    (gene_name.split(" (")[1].split(")")[0] if "(" in gene_name else gene_name)
+                    for gene_name in self.bulk_rna_broad.columns
+                ]
+            elif gene_identifier == "gene_name":
+                self.bulk_rna_broad.columns = [
+                    gene_name.split(" (")[0] if "(" in gene_name else gene_name
+                    for gene_name in self.bulk_rna_broad.columns
+                ]
             broad_rna_exp = self.bulk_rna_broad[self.bulk_rna_broad.index.isin(adata.obs[query_id])]
             ccle_expression = broad_rna_exp.reindex(adata.obs[query_id])
             ccle_expression.index = adata.obs.index
-            adata.obsm["bulk_rna_expression_broad"] = ccle_expression
+            adata.obsm["bulk_rna_broad"] = ccle_expression
 
         return adata
 
     def annotate_protein_expression(
         self,
         adata: AnnData,
         query_id: str = "cell_line_name",
         reference_id: Literal["model_name", "model_id"] = "model_name",
         protein_information: Literal["protein_intensity", "zscore"] = "protein_intensity",
         protein_id: Literal["uniprot_id", "symbol"] = "uniprot_id",
+        verbosity: int | str = 5,
         copy: bool = False,
     ) -> AnnData:
         """Fetch protein expression.
 
         For each cell, we fetch protein intensity values acquired using data-independent acquisition mass spectrometry (DIA-MS).
 
         Args:
             adata: The data object to annotate.
             query_id: The column of `.obs` with cell line information. Defaults to "cell_line_name".
-            reference_id: The type of cell line identifier in the meta data, model_name or model_id. Defaults to "model_name".
-            protein_information: The type of protein expression data to fetch, protein_intensity or zscore. Defaults to "protein_intensity".
-            protein_id: The protein identifier saved in the fetched meta data, uniprot_id or symbol. Defaults to "uniprot_id".
+            reference_id: The type of cell line identifier in the meta data, model_name or model_id.
+                          Defaults to "model_name".
+            protein_information: The type of protein expression data to fetch, protein_intensity or zscore.
+                                 Defaults to "protein_intensity".
+            protein_id: The protein identifier saved in the fetched meta data, uniprot_id or symbol.
+                        Defaults to "uniprot_id".
+            verbosity: The number of unmatched identifiers to print, can be either non-negative values or "all".
+                       Defaults to 5.
             copy: Determines whether a copy of the `adata` is returned. Defaults to False.
 
         Returns:
             Returns an AnnData object with protein expression annotation.
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.dialogue_example()
-            >>> adata.obs['cell_line_name'] = 'MCF7'
-            >>> pt_metadata = pt.tl.CellLineMetaData()
-            >>> adata_annotated = pt_metadata.annotate_cell_lines(adata=adata, reference_id='cell_line_name', query_id='cell_line_name', copy=True)
+            >>> adata.obs["cell_line_name"] = "MCF7"
+            >>> pt_metadata = pt.md.CellLine()
+            >>> adata_annotated = pt_metadata.annotate(
+            ...     adata=adata, reference_id="cell_line_name", query_id="cell_line_name", copy=True
+            ... )
             >>> pt_metadata.annotate_protein_expression(adata_annotated)
         """
         if copy:
             adata = adata.copy()
 
         # Make sure that the specified `cell_line_type` can be found in the protein expression data,
         # then we can compare these keys and fetch the corresponding metadata.
         if query_id not in adata.obs.columns:
             raise ValueError(
-                f"The specified `query_id` {query_id} can't be found in the `adata.obs`. \n"
-                "Please ensure that you are using one of the available query IDs present in the adata.obs for the annotation. \n"
+                f"The specified `query_id` {query_id} can't be found in `adata.obs`. \n"
                 "If the desired query ID is not available, you can fetch the cell line metadata \n"
-                "using the `annotate_cell_lines()` function before calling annotate_protein_expression(). \n"
-                "This will help ensure that the required query ID is included in your data"
+                "using the `annotate()` function before calling annotate_protein_expression(). \n"
+                "This ensures that the required query ID is included in your data."
             )
-
-        if reference_id not in self.proteomics_data.columns:
+        # Lazily download the proteomics data
+        if self.proteomics is None:
+            self._download_proteomics()
+        if reference_id not in self.proteomics.columns:
             raise ValueError(
                 f"The specified `reference_id`{reference_id} can't be found in the protein expression data. \n"
                 "To solve the issue, please use the reference identifier available in the metadata.  \n"
-                "Alternatively, you can call the `CellLineMetaData.lookup()` function to create a LookUp object. \n"
-                "By using the `LookUp.protein_expression()` method, you can obtain the available reference identifiers in the metadata. "
+                "Alternatively, create a `CellLineMetaData.lookup()` object to obtain the available reference identifiers in the metadata. "
             )
 
         identifier_num_all = len(adata.obs[query_id].unique())
-        not_matched_identifiers = list(set(adata.obs[query_id]) - set(self.proteomics_data[reference_id]))
+        not_matched_identifiers = list(set(adata.obs[query_id]) - set(self.proteomics[reference_id]))
 
-        if len(not_matched_identifiers) == identifier_num_all:
-            raise ValueError(
-                f"You are attempting to match the query id {query_id} in the adata.obs to the reference id {reference_id} in the metadata."
-                "However, none of the query IDs could be found in the proteomics data. \n"
-                "The annotation process has been halted. \n"
-                "To resolve this issue, please call the `CellLineMetaData.lookup()` function to create a LookUp object. \n"
-                "By using the `LookUp.protein_expression()` method, "
-                "you can obtain the count of matched identifiers in the adata for different types of reference IDs and query IDs. \n"
-                "Additionally, you can call the `CellLineMetaData.annotate_cell_lines` function "
-                "to acquire more possible query IDs that can be used for annotation purposes."
-            )
+        self._warn_unmatch(
+            total_identifiers=identifier_num_all,
+            unmatched_identifiers=not_matched_identifiers,
+            query_id=query_id,
+            reference_id=reference_id,
+            metadata_type="protein expression",
+            verbosity=verbosity,
+        )
 
-        if len(not_matched_identifiers) > 0:
-            print(
-                f"[bold yellow]There are {identifier_num_all} identifiers in `adata.obs`. "
-                f"However {len(not_matched_identifiers)} identifiers can't be found in the protein expression data, "
-                "leading to the presence of NA values for their respective metadata. Please check again: ",
-                *not_matched_identifiers,
-                sep="\n- ",
-            )
         # convert the original protein intensities table from long format to wide format, group by the cell lines
-        prot_exp = self.proteomics_data[[reference_id, protein_id, protein_information]]
-        prot_exp = pd.pivot(prot_exp, index=reference_id, columns=protein_id, values=protein_information)
-        prot_exp = prot_exp.reindex(adata.obs[query_id])
-        prot_exp.index = adata.obs.index
-        adata.obsm["proteomics_" + protein_information] = prot_exp
-
+        adata.obsm["proteomics_" + protein_information] = (
+            self.proteomics[[reference_id, protein_id, protein_information]]
+            .pivot(index=reference_id, columns=protein_id, values=protein_information)
+            .reindex(adata.obs.index)
+        )
         return adata
 
     def annotate_from_gdsc(
         self,
         adata: AnnData,
         query_id: str = "cell_line_name",
         reference_id: Literal["cell_line_name", "sanger_model_id", "cosmic_id"] = "cell_line_name",
         query_perturbation: str = "perturbation",
         reference_perturbation: Literal["drug_name", "drug_id"] = "drug_name",
         gdsc_dataset: Literal[1, 2] = 1,
+        verbosity: int | str = 5,
         copy: bool = False,
     ) -> AnnData:
-        """Fetch drug response data.
+        """Fetch drug response data from GDSC.
 
-        For each cell, we fetch drug response data as natural log of the fitted IC50 for its corresponding cell line and perturbation from GDSC fitted data results file.
+        For each cell, we fetch drug response data as natural log of the fitted IC50 for its
+        corresponding cell line and perturbation from GDSC fitted data results file.
 
         Args:
             adata: The data object to annotate.
             query_id: The column of `.obs` with cell line information. Defaults to "cell_line_name".
-            reference_id: The type of cell line identifier in the meta data, cell_line_name, sanger_model_id or cosmic_id. Defaults to "cell_line_name".
-            query_perturbation: The column of `.obs` with perturbation information. Defaults to "perturbation".
-            reference_perturbation: The type of perturbation in the meta data, drug_name or drug_id. Defaults to "drug_name".
-            gdsc_dataset: The GDSC dataset, 1 or 2. Defaults to 1. The GDSC1 dataset updates previous releases with additional drug screening data from the Wellcome Sanger Institute and Massachusetts General Hospital. It covers 970 Cell lines and 403 Compounds with 333292 IC50s. GDSC2 is new and has 243,466 IC50 results from the latest screening at the Wellcome Sanger Institute using improved experimental procedures.
+            reference_id: The type of cell line identifier in the meta data, cell_line_name, sanger_model_id or cosmic_id.
+                          Defaults to "cell_line_name".
+            query_perturbation: The column of `.obs` with perturbation information.
+                                Defaults to "perturbation".
+            reference_perturbation: The type of perturbation in the meta data, drug_name or drug_id.
+                                    Defaults to 'drug_name'.
+            gdsc_dataset: The GDSC dataset, 1 or 2.
+                          The GDSC1 dataset updates previous releases with additional drug screening data from the
+                          Sanger Institute and Massachusetts General Hospital.
+                          It covers 970 Cell lines and 403 Compounds with 333292 IC50s.
+                          GDSC2 is new and has 243,466 IC50 results from the latest screening at the Sanger Institute.
+                          Defaults to 1.
+            verbosity: The number of unmatched identifiers to print, can be either non-negative values or 'all'.
+                       Defaults to 5.
             copy: Determines whether a copy of the `adata` is returned. Defaults to False.
 
         Returns:
             Returns an AnnData object with drug response annotation.
 
         Examples:
             >>> import pertpy as pt
             >>> adata = pt.dt.mcfarland_2020()
-            >>> pt_metadata = pt.tl.CellLineMetaData()
-            >>> pt_metadata.annotate_from_gdsc(adata, query_id='cell_line')
+            >>> pt_metadata = pt.md.CellLine()
+            >>> pt_metadata.annotate_from_gdsc(adata, query_id="cell_line")
         """
         if copy:
             adata = adata.copy()
         if query_id not in adata.obs.columns:
             raise ValueError(
                 f"The specified `query_id` {query_id} can't be found in the `adata.obs`. \n"
-                "Please ensure that you are using one of the available query IDs present in the adata.obs for the annotation. \n"
+                "Ensure that you are using one of the available query IDs present in 'adata.obs' for the annotation.\n"
                 "If the desired query ID is not available, you can fetch the cell line metadata "
-                "using the `annotate_cell_lines()` function before calling `annotate_from_gdsc()`. "
-                "This will help ensure that the required query ID is included in your data."
+                "using the `annotate()` function before calling `annotate_from_gdsc()`. "
+                "This ensures that the required query ID is included in your data."
             )
+        # Lazily download the GDSC data
         if gdsc_dataset == 1:
+            if self.drug_response_gdsc1 is None:
+                self._download_gdsc(gdsc_dataset=1)
             gdsc_data = self.drug_response_gdsc1
         else:
+            if self.drug_response_gdsc2 is None:
+                self._download_gdsc(gdsc_dataset=2)
             gdsc_data = self.drug_response_gdsc2
-        not_matched_identifiers = list(set(adata.obs[query_id]) - set(gdsc_data[reference_id]))
-        if len(not_matched_identifiers) > 0:
-            print(
-                f"[bold yellow]Following {len(not_matched_identifiers)} identifiers can not be found in the drug response data for GDSC{gdsc_dataset},"
-                "leading to the presence of NA values for their respective metadata. Please check it again:",
-                *not_matched_identifiers,
-                sep="\n- ",
-            )
+
         identifier_num_all = len(adata.obs[query_id].unique())
-        if len(not_matched_identifiers) == identifier_num_all:
-            raise ValueError(
-                f"You are attempting to match the query id {query_id} in the adata.obs to the reference id {reference_id} in the metadata. \n"
-                "However, none of the query IDs could be found in the drug response data. \n"
-                "The annotation process has been halted. \n"
-                "To resolve this issue, please call the `CellLineMetaData.lookup()` function to create a LookUp object. \n"
-                "By using the `LookUp.drug_response_gdsc()` method, \n"
-                "you can obtain the count of matched identifiers in the adata for different query IDs. \n"
-                "Additionally, you can call the `CellLineMetaData.annotate_cell_lines()` function to \n"
-                "acquire more cell line information that can be used for annotation purposes."
-            )
+        not_matched_identifiers = list(set(adata.obs[query_id]) - set(gdsc_data[reference_id]))
+        self._warn_unmatch(
+            total_identifiers=identifier_num_all,
+            unmatched_identifiers=not_matched_identifiers,
+            query_id=query_id,
+            reference_id=reference_id,
+            metadata_type="drug response",
+            verbosity=verbosity,
+        )
+
+        old_index_name = "index" if adata.obs.index.name is None else adata.obs.index.name
         adata.obs = (
-            adata.obs.merge(
-                gdsc_data[[reference_id, reference_perturbation, "ln_ic50"]],
-                how="left",
-                left_on=[query_id, query_perturbation],
-                right_on=[reference_id, reference_perturbation],
-                suffixes=("", "_fromMeta"),
-            )
-            .filter(regex="^(?!.*_fromMeta)")
-            .set_index(adata.obs.index)
+            adata.obs.reset_index()
+            .set_index([query_id, query_perturbation])
+            .assign(ln_ic50=self.drug_response_gdsc1.set_index([reference_id, reference_perturbation]).ln_ic50)
+            .reset_index()
+            .set_index(old_index_name)
         )
 
         return adata
 
     def lookup(self) -> LookUp:
         """Generate LookUp object for CellLineMetaData.
 
         The LookUp object provides an overview of the metadata to annotate.
         Each annotate_{metadata} function has a corresponding lookup function in the LookUp object,
         where users can search the reference_id in the metadata and
         compare with the query_id in their own data.
 
         Returns:
-            Returns a LookUp object specific for cell line annotation.
+            A LookUp object specific for cell line annotation.
 
         Examples:
             >>> import pertpy as pt
-            >>> pt_metadata = pt.tl.CellLineMetaData()
+            >>> pt_metadata = pt.md.CellLine()
             >>> lookup = pt_metadata.lookup()
         """
+        # Fetch the metadata if it hasn't beed downloaded yet
+        if self.depmap is None:
+            self._download_cell_line(cell_line_source="DepMap")
+        if self.cancerxgene is None:
+            self._download_cell_line(cell_line_source="Cancerrxgene")
+        if self.gene_annotation is None:
+            self._download_gene_annotation()
+        if self.bulk_rna_broad is None:
+            self._download_bulk_rna(cell_line_source="broad")
+        if self.bulk_rna_sanger is None:
+            self._download_bulk_rna(cell_line_source="sanger")
+        if self.proteomics is None:
+            self._download_proteomics()
+        if self.drug_response_gdsc1 is None:
+            self._download_gdsc(gdsc_dataset=1)
+        if self.drug_response_gdsc2 is None:
+            self._download_gdsc(gdsc_dataset=2)
+
+        # Transfer the data
         return LookUp(
             type="cell_line",
             transfer_metadata=[
-                self.cell_line_meta,
-                self.cl_cancer_project_meta,
+                self.depmap,
+                self.cancerxgene,
                 self.gene_annotation,
                 self.bulk_rna_sanger,
                 self.bulk_rna_broad,
-                self.proteomics_data,
+                self.proteomics,
                 self.drug_response_gdsc1,
                 self.drug_response_gdsc2,
             ],
         )
+
+    def _pairwise_correlation(
+        self, mat1: np.array, mat2: np.array, row_name: Iterable, col_name: Iterable
+    ) -> tuple[pd.DataFrame, pd.DataFrame]:
+        """Calculate the row-wise pearson correlation between two matrices.
+
+        Args:
+            mat1: Input array
+            mat2: Input array
+            row_name: Row name of the output dataframes
+            col_name: Row name of the output dataframes
+
+        Returns:
+            Returns DataFrames for both the Pearson correlation coefficients and their associated p-values.
+        """
+        corr = np.empty((mat1.shape[0], mat2.shape[0]))
+        pvals = np.empty((mat1.shape[0], mat2.shape[0]))
+
+        for i in range(mat1.shape[0]):
+            for j in range(mat2.shape[0]):
+                if i > j:
+                    corr[i, j] = corr[j, i]
+                    pvals[i, j] = pvals[j, i]
+                else:
+                    corr[i, j], pvals[i, j] = stats.pearsonr(mat1[i], mat2[j])
+        corr = pd.DataFrame(corr, index=row_name, columns=col_name)
+        pvals = pd.DataFrame(pvals, index=row_name, columns=col_name)
+
+        return corr, pvals
+
+    def correlate(
+        self,
+        adata: AnnData,
+        identifier: str = "DepMap_ID",
+        metadata_key: str = "bulk_rna_broad",
+    ) -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame | None, pd.DataFrame | None]:
+        """Correlate cell lines with annotated metadata.
+
+        Args:
+            adata: Input data object.
+            identifier: Column in `.obs` containing cell line identifiers. Defaults to "DepMap_ID".
+            metadata_key: Key of the AnnData obsm for comparison with the X matrix. Defaults to "bulk_rna_broad".
+
+        Returns:
+            Returns pearson correlation coefficients and their corresponding p-values for matched and unmatched cell lines separately.
+        """
+        if metadata_key not in adata.obsm:
+            raise ValueError("The metadata can not be found in adata.obsm")
+        if identifier not in adata.obs:
+            raise ValueError("The identifier can not be found in adata.obs")
+        if adata.X.shape[1] != adata.obsm[metadata_key].shape[1]:
+            raise ValueError(
+                "Dimensions of adata.X do not match those of metadata. Ensure that they have the same gene list."
+            )
+        if isinstance(adata.obsm[metadata_key], pd.DataFrame):
+            # Give warning if the genes are not the same
+            if sum(adata.obsm[metadata_key].columns != adata.var.index.values) > 0:
+                print(
+                    "Column name of metadata is not the same as the index of adata.var. Ensure that the genes are in the same order."
+                )
+
+        # Divide cell lines into those are present and not present in the metadata
+        overlapped_cl = adata[~adata.obsm[metadata_key].isna().all(axis=1), :]
+        missing_cl = adata[adata.obsm[metadata_key].isna().all(axis=1), :]
+
+        corr, pvals = self._pairwise_correlation(
+            overlapped_cl.X,
+            overlapped_cl.obsm[metadata_key].values,
+            row_name=overlapped_cl.obs[identifier],
+            col_name=overlapped_cl.obs[identifier],
+        )
+        if missing_cl is not None:
+            new_corr, new_pvals = self._pairwise_correlation(
+                missing_cl.X,
+                overlapped_cl.obsm[metadata_key].values,
+                row_name=missing_cl.obs[identifier],
+                col_name=overlapped_cl.obs[identifier],
+            )
+        else:
+            new_corr = new_pvals = None
+
+        return corr, pvals, new_corr, new_pvals
+
+    def plot_correlation(
+        self,
+        adata: AnnData,
+        corr: pd.DataFrame,
+        pval: pd.DataFrame,
+        identifier: str = "DepMap_ID",
+        metadata_key: str = "bulk_rna_broad",
+        category: str = "cell line",
+        subset_identifier: str | int | Iterable[str] | Iterable[int] | None = None,
+    ) -> None:
+        """Visualise the correlation of cell lines with annotated metadata.
+
+        Args:
+            adata: Input data object.
+            corr: Pearson correlation scores.
+            pval: P-values for pearson correlation.
+            identifier: Column in `.obs` containing the identifiers. Defaults to 'DepMap_ID'.
+            metadata_key: Key of the AnnData obsm for comparison with the X matrix. Defaults to 'bulk_rna_broad'.
+            category: The category for correlation comparison. Defaults to "cell line".
+            subset_identifier: Selected identifiers for scatter plot visualization between the X matrix and `metadata_key`.
+                              If not None, only the chosen cell line will be plotted, either specified as a value in `identifier` (string) or as an index number.
+                              If None, all cell lines will be plotted.
+                              Defaults to None.
+        Returns:
+            Pearson correlation coefficients and their corresponding p-values for matched and unmatched cell lines separately.
+        """
+        if corr is None or pval is None:
+            raise ValueError(
+                "Missing required input parameter: 'corr' or 'pval'. Please call the function `pt.md.CellLine.correlate()` to generate these outputs before proceeding."
+            )
+
+        if category == "cell line":
+            if subset_identifier is None:
+                annotation = "\n".join(
+                    (
+                        f"Mean pearson correlation: {np.mean(np.diag(corr)):.4f}",
+                        f"Mean p-value: {np.mean(np.diag(pval)):.4f}",
+                    )
+                )
+                plt.scatter(x=adata.obsm[metadata_key], y=adata.X)
+                plt.xlabel(metadata_key)
+                plt.ylabel("Baseline")
+            else:
+                subset_identifier_list = (
+                    [subset_identifier] if isinstance(subset_identifier, str | int) else list(subset_identifier)
+                )
+                # Convert the valid identifiers to the index list
+                if all(isinstance(id, str) for id in subset_identifier_list):
+                    if set(subset_identifier_list).issubset(adata.obs[identifier].unique()):
+                        subset_identifier_list = np.where(
+                            np.in1d(adata.obs[identifier].values, subset_identifier_list)
+                        )[0]
+                    else:
+                        raise ValueError("`Subset_identifier` must be found in adata.obs.`identifier`.")
+                elif all(isinstance(id, int) and 0 <= id < adata.n_obs for id in subset_identifier_list):
+                    pass
+                elif all(isinstance(id, int) and (id < 0 or id >= adata.n_obs) for id in subset_identifier_list):
+                    raise ValueError("`Subset_identifier` out of index.")
+                else:
+                    raise ValueError("`Subset_identifier` must contain either all strings or all integers.")
+
+                plt.scatter(
+                    x=adata.obsm[metadata_key].iloc[subset_identifier_list],
+                    y=adata[subset_identifier_list].X,
+                )
+                plt.xlabel(
+                    f"{metadata_key}: {adata.obs[identifier].values[subset_identifier_list[0]]}"
+                    if len(subset_identifier_list) == 1
+                    else f"{metadata_key}"
+                )
+                plt.ylabel(
+                    f"Baseline: {adata.obs[identifier].values[subset_identifier_list[0]]}"
+                    if len(subset_identifier_list) == 1
+                    else "Baseline"
+                )
+
+                # Annotate with the correlation coefficient and p-value of the chosen cell lines
+                subset_cor = np.mean(np.diag(corr.iloc[subset_identifier_list, subset_identifier_list]))
+                subset_pval = np.mean(np.diag(pval.iloc[subset_identifier_list, subset_identifier_list]))
+                annotation = "\n".join(
+                    (
+                        f"Pearson correlation: {subset_cor:.4f}",
+                        f"P-value: {subset_pval:.4f}",
+                    )
+                )
+
+            plt.text(
+                0.05,
+                0.95,
+                annotation,
+                fontsize=10,
+                transform=plt.gca().transAxes,
+                verticalalignment="top",
+                bbox={
+                    "boxstyle": "round",
+                    "alpha": 0.5,
+                    "facecolor": "white",
+                    "edgecolor": "black",
+                },
+            )
+            plt.show()
+        else:
+            raise NotImplementedError
```

### Comparing `pertpy-0.6.0/pertpy/tools/_perturbation_space/_clustering.py` & `pertpy-0.7.0/pertpy/tools/_perturbation_space/_clustering.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,27 @@
         """Evaluation of previously computed clustering against ground truth labels.
 
         Args:
             adata: AnnData object that contains the clustered data and the cluster labels.
             true_label_col: ground truth labels.
             cluster_col: cluster computed labels.
             metrics: Metrics to compute. Defaults to ['nmi', 'ari', 'asw'].
+            **kwargs: Additional arguments to pass to the metrics. For nmi, average_method can be passed.
+                For asw, metric, distances, sample_size, and random_state can be passed.
 
         Examples:
             Example usage with KMeansSpace:
 
             >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> kmeans = pt.tl.KMeansSpace()
             >>> kmeans_adata = kmeans.compute(mdata["rna"], n_clusters=26)
-            >>> results = kmeans.evaluate_clustering(kmeans_adata, true_label_col="gene_target", cluster_col="k-means", metrics=['nmi'])
+            >>> results = kmeans.evaluate_clustering(
+            ...     kmeans_adata, true_label_col="gene_target", cluster_col="k-means", metrics=["nmi"]
+            ... )
         """
         if metrics is None:
             metrics = ["nmi", "ari", "asw"]
         true_labels = adata.obs[true_label_col]
 
         results = {}
         for metric in metrics:
```

### Comparing `pertpy-0.6.0/pertpy/tools/_perturbation_space/_metrics.py` & `pertpy-0.7.0/pertpy/tools/_perturbation_space/_metrics.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/pertpy/tools/_perturbation_space/_perturbation_space.py` & `pertpy-0.7.0/pertpy/tools/_perturbation_space/_perturbation_space.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,69 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 from anndata import AnnData
+from pynndescent import NNDescent
 from rich import print
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
 
 
 class PerturbationSpace:
     """Implements various ways of interacting with PerturbationSpaces.
 
     We differentiate between a cell space and a perturbation space.
-    Visually speaking, in cell spaces single dota points in an embeddings summarize a cell,
+    Visually speaking, in cell spaces single data points in an embeddings summarize a cell,
     whereas in a perturbation space, data points summarize whole perturbations.
     """
 
     def __init__(self):
         self.control_diff_computed = False
 
     def compute_control_diff(  # type: ignore
         self,
         adata: AnnData,
-        target_col: str = "perturbations",
+        target_col: str = "perturbation",
+        group_col: str = None,
         reference_key: str = "control",
         layer_key: str = None,
         new_layer_key: str = "control_diff",
         embedding_key: str = None,
         new_embedding_key: str = "control_diff",
         all_data: bool = False,
         copy: bool = False,
-    ):
+    ) -> AnnData:
         """Subtract mean of the control from the perturbation.
 
         Args:
             adata: Anndata object of size cells x genes.
             target_col: .obs column name that stores the label of the perturbation applied to each cell. Defaults to 'perturbations'.
+            group_col: .obs column name that stores the label of the group of eah cell. If None, ignore groups. Defaults to 'perturbations'.
             reference_key: The key of the control values. Defaults to 'control'.
             layer_key: Key of the AnnData layer to use for computation. Defaults to the `X` matrix otherwise.
-            new_layer_key: the results are stored in the given layer. Defaults to 'differential diff'.
+            new_layer_key: the results are stored in the given layer. Defaults to 'control_diff'.
             embedding_key: `obsm` key of the AnnData embedding to use for computation. Defaults to the 'X' matrix otherwise.
-            new_embedding_key: Results are stored in a new embedding in `obsm` with this key. Defaults to 'control diff'.
+            new_embedding_key: Results are stored in a new embedding in `obsm` with this key. Defaults to 'control_diff'.
             all_data: if True, do the computation in all data representations (X, all layers and all embeddings)
             copy: If True returns a new Anndata of same size with the new column; otherwise it updates the initial AnnData object.
 
+        Returns:
+            Updated AnnData object.
+
         Examples:
             Example usage with PseudobulkSpace:
+
             >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> ps = pt.tl.PseudobulkSpace()
-            >>> diff_adata = ps.compute_control_diff(mdata["rna"], target_col="gene_target", reference_key='NT')
+            >>> diff_adata = ps.compute_control_diff(mdata["rna"], target_col="gene_target", reference_key="NT")
         """
         if reference_key not in adata.obs[target_col].unique():
             raise ValueError(
                 f"Reference key {reference_key} not found in {target_col}. {reference_key} must be in obs column {target_col}."
             )
 
         if embedding_key is not None and embedding_key not in adata.obsm_keys():
@@ -65,85 +72,110 @@
         if layer_key is not None and layer_key not in adata.layers.keys():
             raise ValueError(f"Layer {layer_key!r} does not exist in the anndata.")
 
         if copy:
             adata = adata.copy()
 
         control_mask = adata.obs[target_col] == reference_key
-        num_control = control_mask.sum()
+        group_masks = (
+            [(adata.obs[group_col] == sample) for sample in adata.obs[group_col].unique()]
+            if group_col
+            else [[True] * adata.n_obs]
+        )
 
         if layer_key:
-            if num_control == 1:
-                control_expression = adata.layers[layer_key][control_mask, :]
-            else:
-                control_expression = np.mean(adata.layers[layer_key][control_mask, :], axis=0)
-            diff_matrix = adata.layers[layer_key] - control_expression
-            adata.layers[new_layer_key] = diff_matrix
+            adata.layers[new_layer_key] = np.zeros((adata.n_obs, adata.n_vars))
+            for mask in group_masks:
+                num_control = (control_mask & mask).sum()
+                if num_control == 1:
+                    control_expression = adata.layers[layer_key][(control_mask & mask), :]
+                elif num_control > 1:
+                    control_expression = np.mean(adata.layers[layer_key][(control_mask & mask), :], axis=0)
+                else:
+                    control_expression = np.zeros((1, adata.n_vars))
+                adata.layers[new_layer_key][mask, :] = adata.layers[layer_key][mask, :] - control_expression
 
         if embedding_key:
-            if num_control == 1:
-                control_expression = adata.obsm[embedding_key][control_mask, :]
-            else:
-                control_expression = np.mean(adata.obsm[embedding_key][control_mask, :], axis=0)
-            diff_matrix = adata.obsm[embedding_key] - control_expression
-            adata.obsm[new_embedding_key] = diff_matrix
+            adata.obsm[new_embedding_key] = np.zeros(adata.obsm[embedding_key].shape)
+            for mask in group_masks:
+                num_control = (control_mask & mask).sum()
+                if num_control == 1:
+                    control_expression = adata.obsm[embedding_key][(control_mask & mask), :]
+                elif num_control > 1:
+                    control_expression = np.mean(adata.obsm[embedding_key][(control_mask & mask), :], axis=0)
+                else:
+                    control_expression = np.zeros((1, adata.n_vars))
+                adata.obsm[new_embedding_key][mask, :] = adata.obsm[embedding_key][mask, :] - control_expression
 
         if (not layer_key and not embedding_key) or all_data:
-            if num_control == 1:
-                control_expression = adata.X[control_mask, :]
-            else:
-                control_expression = np.mean(adata.X[control_mask, :], axis=0)
-            diff_matrix = adata.X - control_expression
-            adata.X = diff_matrix
+            adata_x = np.zeros((adata.n_obs, adata.n_vars))
+            for mask in group_masks:
+                num_control = (control_mask & mask).sum()
+                if num_control == 1:
+                    control_expression = adata.X[(control_mask & mask), :]
+                elif num_control > 1:
+                    control_expression = np.mean(adata.X[(control_mask & mask), :], axis=0)
+                else:
+                    control_expression = np.zeros((1, adata.n_vars))
+                adata_x[mask, :] = adata.X[mask, :] - control_expression
+            adata.X = adata_x
 
         if all_data:
             layers_keys = list(adata.layers.keys())
             for local_layer_key in layers_keys:
                 if local_layer_key != layer_key and local_layer_key != new_layer_key:
-                    diff_matrix = adata.layers[local_layer_key] - np.mean(
-                        adata.layers[local_layer_key][control_mask, :], axis=0
-                    )
-                    adata.layers[local_layer_key + "_control_diff"] = diff_matrix
+                    adata.layers[local_layer_key + "_control_diff"] = np.zeros((adata.n_obs, adata.n_vars))
+                    for mask in group_masks:
+                        adata.layers[local_layer_key + "_control_diff"][mask, :] = adata.layers[local_layer_key][
+                            mask, :
+                        ] - np.mean(adata.layers[local_layer_key][(control_mask & mask), :], axis=0)
 
             embedding_keys = list(adata.obsm_keys())
             for local_embedding_key in embedding_keys:
                 if local_embedding_key != embedding_key and local_embedding_key != new_embedding_key:
-                    diff_matrix = adata.obsm[local_embedding_key] - np.mean(
-                        adata.obsm[local_embedding_key][control_mask, :], axis=0
-                    )
-                    adata.obsm[local_embedding_key + "_control_diff"] = diff_matrix
+                    adata.obsm[local_embedding_key + "_control_diff"] = np.zeros(adata.obsm[local_embedding_key].shape)
+                    for mask in group_masks:
+                        adata.obsm[local_embedding_key + "_control_diff"][mask, :] = adata.obsm[local_embedding_key][
+                            mask, :
+                        ] - np.mean(adata.obsm[local_embedding_key][(control_mask & mask), :], axis=0)
 
         self.control_diff_computed = True
 
         return adata
 
     def add(
         self,
         adata: AnnData,
         perturbations: Iterable[str],
         reference_key: str = "control",
         ensure_consistency: bool = False,
-        target_col: str = "perturbations",
-    ):
+        target_col: str = "perturbation",
+    ) -> tuple[AnnData, AnnData] | AnnData:
         """Add perturbations linearly. Assumes input of size n_perts x dimensionality
 
         Args:
             adata: Anndata object of size n_perts x dim.
             perturbations: Perturbations to add.
-            reference_key: perturbation source from which the perturbation summation starts.
+            reference_key: perturbation source from which the perturbation summation starts. Defaults to 'control'.
             ensure_consistency: If True, runs differential expression on all data matrices to ensure consistency of linear space.
-            target_col: .obs column name that stores the label of the perturbation applied to each cell. Defaults to 'perturbations'.
+            target_col: .obs column name that stores the label of the perturbation applied to each cell. Defaults to 'perturbation'.
+
+        Returns:
+            Anndata object of size (n_perts+1) x dim, where the last row is the addition of the specified perturbations.
+            If ensure_consistency is True, returns a tuple of (new_perturbation, adata) where adata is the AnnData object
+            provided as input but updated using compute_control_diff.
 
         Examples:
             Example usage with PseudobulkSpace:
+
             >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> ps = pt.tl.PseudobulkSpace()
             >>> ps_adata = ps.compute(mdata["rna"], target_col="gene_target", groups_col="gene_target")
-            >>> new_perturbation = ps.add(ps_adata, perturbations=["ATF2", "CD86"], reference_key='NT')
+            >>> new_perturbation = ps.add(ps_adata, perturbations=["ATF2", "CD86"], reference_key="NT")
         """
         new_pert_name = ""
         for perturbation in perturbations:
             if perturbation not in adata.obs_names:
                 raise ValueError(
                     f"Perturbation {perturbation} not found in adata.obs_names. {perturbation} must be in adata.obs_names."
                 )
@@ -208,43 +240,51 @@
         if "embeddings" in data.keys():
             key_name = key
             for key in data["embeddings"]:
                 if key.endswith("_control_diff"):
                     key_name = key.removesuffix("_control_diff")
                 new_perturbation.obsm[key_name] = data["embeddings"][key]
 
+        new_perturbation.obs[target_col] = new_perturbation.obs_names.astype("category")
+
         if ensure_consistency:
             return new_perturbation, adata
 
         return new_perturbation
 
     def subtract(
         self,
         adata: AnnData,
         perturbations: Iterable[str],
         reference_key: str = "control",
         ensure_consistency: bool = False,
-        target_col: str = "perturbations",
-    ):
+        target_col: str = "perturbation",
+    ) -> tuple[AnnData, AnnData] | AnnData:
         """Subtract perturbations linearly. Assumes input of size n_perts x dimensionality
 
         Args:
             adata: Anndata object of size n_perts x dim.
-            perturbations: Perturbations to subtract,
-            reference_key: Perturbation source from which the perturbation subtraction starts
+            perturbations: Perturbations to subtract.
+            reference_key: Perturbation source from which the perturbation subtraction starts. Defaults to 'control'.
             ensure_consistency: If True, runs differential expression on all data matrices to ensure consistency of linear space.
             target_col: .obs column name that stores the label of the perturbation applied to each cell. Defaults to 'perturbations'.
 
+        Returns:
+            Anndata object of size (n_perts+1) x dim, where the last row is the subtraction of the specified perturbations.
+            If ensure_consistency is True, returns a tuple of (new_perturbation, adata) where adata is the AnnData object
+            provided as input but updated using compute_control_diff.
+
         Examples:
             Example usage with PseudobulkSpace:
+
             >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> ps = pt.tl.PseudobulkSpace()
             >>> ps_adata = ps.compute(mdata["rna"], target_col="gene_target", groups_col="gene_target")
-            >>> new_perturbation = ps.add(ps_adata, reference_key="ATF2", perturbations=["BRD4", "CUL3"])
+            >>> new_perturbation = ps.subtract(ps_adata, reference_key="ATF2", perturbations=["BRD4", "CUL3"])
         """
         new_pert_name = reference_key + "-"
         for perturbation in perturbations:
             if perturbation not in adata.obs_names:
                 raise ValueError(
                     f"Perturbation {perturbation} not found in adata.obs_names. {perturbation} must be in adata.obs_names."
                 )
@@ -309,11 +349,63 @@
         if "embeddings" in data.keys():
             key_name = key
             for key in data["embeddings"]:
                 if key.endswith("_control_diff"):
                     key_name = key.removesuffix("_control_diff")
                 new_perturbation.obsm[key_name] = data["embeddings"][key]
 
+        new_perturbation.obs[target_col] = new_perturbation.obs_names.astype("category")
+
         if ensure_consistency:
             return new_perturbation, adata
 
         return new_perturbation
+
+    def label_transfer(
+        self,
+        adata: AnnData,
+        column: str = "perturbation",
+        target_val: str = "unknown",
+        n_neighbors: int = 5,
+        use_rep: str = "X_umap",
+    ) -> None:
+        """Impute missing values in the specified column using KNN imputation in the space defined by `use_rep`.
+
+        Args:
+            adata: The AnnData object containing single-cell data.
+            column: The column name in AnnData object to perform imputation on. Defaults to "perturbation".
+            target_val: The target value to impute. Defaults to "unknown".
+            n_neighbors: Number of neighbors to use for imputation. Defaults to 5.
+            use_rep: The key in `adata.obsm` where the embedding (UMAP, PCA, etc.) is stored. Defaults to 'X_umap'.
+
+        Examples:
+            >>> import pertpy as pt
+            >>> import scanpy as sc
+            >>> import numpy as np
+            >>> adata = sc.datasets.pbmc68k_reduced()
+            >>> rng = np.random.default_rng()
+            >>> adata.obs["perturbation"] = rng.choice(
+            ...     ["A", "B", "C", "unknown"], size=adata.n_obs, p=[0.33, 0.33, 0.33, 0.01]
+            ... )
+            >>> sc.pp.neighbors(adata)
+            >>> sc.tl.umap(adata)
+            >>> ps = pt.tl.PseudobulkSpace()
+            >>> ps.label_transfer(adata, n_neighbors=5, use_rep="X_umap")
+        """
+        if use_rep not in adata.obsm:
+            raise ValueError(f"Representation {use_rep} not found in the AnnData object.")
+
+        embedding = adata.obsm[use_rep]
+
+        nnd = NNDescent(embedding, n_neighbors=n_neighbors)
+        indices, _ = nnd.query(embedding, k=n_neighbors)
+
+        perturbations = np.array(adata.obs[column])
+        missing_mask = perturbations == target_val
+
+        for idx in np.where(missing_mask)[0]:
+            neighbor_indices = indices[idx]
+            neighbor_categories = perturbations[neighbor_indices]
+            most_common = pd.Series(neighbor_categories).mode()[0]
+            perturbations[idx] = most_common
+
+        adata.obs[column] = perturbations
```

### Comparing `pertpy-0.6.0/pertpy/tools/_perturbation_space/_simple.py` & `pertpy-0.7.0/pertpy/tools/_perturbation_space/_simple.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,34 +11,41 @@
 
 class CentroidSpace(PerturbationSpace):
     """Computes the centroids per perturbation of a pre-computed embedding."""
 
     def compute(
         self,
         adata: AnnData,
-        target_col: str = "perturbations",
+        target_col: str = "perturbation",
         layer_key: str = None,
         embedding_key: str = "X_umap",
+        keep_obs: bool = True,
     ) -> AnnData:  # type: ignore
         """Computes the centroids of a pre-computed embedding such as UMAP.
 
         Args:
             adata: Anndata object of size cells x genes
             target_col: .obs column that stores the label of the perturbation applied to each cell.
             layer_key: If specified pseudobulk computation is done by using the specified layer. Otherwise, computation is done with .X
             embedding_key: `obsm` key of the AnnData embedding to use for computation. Defaults to the 'X' matrix otherwise.
+            keep_obs: Whether .obs columns in the input AnnData should be kept in the output pseudobulk AnnData. Only .obs columns with the same value for
+                each cell of one perturbation are kept. Defaults to True.
+
+        Returns:
+            AnnData object with one observation per perturbation, storing the embedding data of the
+            centroid of the respective perturbation.
 
         Examples:
             Compute the centroids of a UMAP embedding of the papalexi_2021 dataset:
 
             >>> import pertpy as pt
             >>> import scanpy as sc
             >>> mdata = pt.dt.papalexi_2021()
             >>> sc.pp.pca(mdata["rna"])
-            >>> sc.pp.neighbors(mdata['rna'])
+            >>> sc.pp.neighbors(mdata["rna"])
             >>> sc.tl.umap(mdata["rna"])
             >>> cs = pt.tl.CentroidSpace()
             >>> cs_adata = cs.compute(mdata["rna"], target_col="gene_target")
         """
 
         X = None
         if layer_key is not None and embedding_key is not None:
@@ -80,47 +87,66 @@
                 points, key=lambda point: np.linalg.norm(point - centroid)
             )  # Find the point in the array closest to the centroid
             X[pert_index, :] = closest_point
             pert_index += 1
 
         ps_adata = AnnData(X=X)
         ps_adata.obs_names = index
+        ps_adata.obs[target_col] = index
+
+        if embedding_key is not None:
+            ps_adata.obsm[embedding_key] = X
+
+        if keep_obs:  # Save the values of the obs columns of interest in the ps_adata object
+            obs_df = adata.obs
+            obs_df = obs_df.groupby(target_col).agg(
+                lambda pert_group: np.nan if len(set(pert_group)) != 1 else list(set(pert_group))[0]
+            )
+            for obs_name in obs_df.columns:
+                if not obs_df[obs_name].isnull().values.any():
+                    mapping = {pert: obs_df.loc[pert][obs_name] for pert in index}
+                    ps_adata.obs[obs_name] = ps_adata.obs[target_col].map(mapping)
+
+        ps_adata.obs[target_col] = ps_adata.obs[target_col].astype("category")
 
         return ps_adata
 
 
 class PseudobulkSpace(PerturbationSpace):
     """Determines pseudobulks using decoupler."""
 
     def compute(
         self,
         adata: AnnData,
-        target_col: str = "perturbations",
+        target_col: str = "perturbation",
+        groups_col: str = None,
         layer_key: str = None,
         embedding_key: str = None,
         **kwargs,
     ) -> AnnData:  # type: ignore
         """Determines pseudobulks of an AnnData object. It uses Decoupler implementation.
 
         Args:
             adata: Anndata object of size cells x genes
             target_col: .obs column that stores the label of the perturbation applied to each cell.
+            groups_col: Optional .obs column that stores a grouping label to consider for pseudobulk computation.
+                The summarized expression per perturbation (target_col) and group (groups_col) is computed. Defaults to None.
             layer_key: If specified pseudobulk computation is done by using the specified layer. Otherwise, computation is done with .X
             embedding_key: `obsm` key of the AnnData embedding to use for computation. Defaults to the 'X' matrix otherwise.
             **kwargs: Are passed to decoupler's get_pseuobulk.
 
+        Returns:
+             AnnData object with one observation per perturbation.
+
         Examples:
-            >>> import pertpy as pp
+            >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> ps = pt.tl.PseudobulkSpace()
-            >>> ps_adata = ps.compute(mdata["rna"], target_col="gene_target", groups_col="gene_target")
+            >>> ps_adata = ps.compute(mdata["rna"], target_col="gene_target")
         """
-        if "groups_col" not in kwargs:
-            kwargs["groups_col"] = "perturbations"
-
         if layer_key is not None and embedding_key is not None:
             raise ValueError("Please, select just either layer or embedding for computation.")
 
         if layer_key is not None and layer_key not in adata.layers.keys():
             raise ValueError(f"Layer {layer_key!r} does not exist in the .layers attribute.")
 
         if target_col not in adata.obs:
@@ -131,15 +157,18 @@
                 raise ValueError(f"Embedding {embedding_key!r} does not exist in the .obsm attribute.")
             else:
                 adata_emb = AnnData(X=adata.obsm[embedding_key])
                 adata_emb.obs_names = adata.obs_names
                 adata_emb.obs = adata.obs
                 adata = adata_emb
 
-        ps_adata = dc.get_pseudobulk(adata, sample_col=target_col, layer=layer_key, **kwargs)  # type: ignore
+        adata.obs[target_col] = adata.obs[target_col].astype("category")
+        ps_adata = dc.get_pseudobulk(adata, sample_col=target_col, layer=layer_key, groups_col=groups_col, **kwargs)  # type: ignore
+
+        ps_adata.obs[target_col] = ps_adata.obs[target_col].astype("category")
 
         return ps_adata
 
 
 class KMeansSpace(ClusteringSpace):
     """Computes K-Means clustering of the expression values."""
 
@@ -160,14 +189,19 @@
             layer_key: if specified and exists in the adata, the clustering is done by using it. Otherwise, clustering is done with .X
             embedding_key: if specified and exists in the adata, the clustering is done with that embedding. Otherwise, clustering is done with .X
             cluster_key: name of the .obs column to store the cluster labels. Default 'k-means'
             copy: if True returns a new Anndata of same size with the new column; otherwise it updates the initial adata
             return_object: if True returns the clustering object
             **kwargs: Are passed to sklearn's KMeans.
 
+        Returns:
+            If return_object is True, the adata and the clustering object is returned.
+            Otherwise, only the adata is returned. The adata is updated with a new .obs column as specified in cluster_key,
+             that stores the cluster labels.
+
         Examples:
             >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> kmeans = pt.tl.KMeansSpace()
             >>> kmeans_adata = kmeans.compute(mdata["rna"], n_clusters=26)
         """
         if copy:
@@ -189,14 +223,15 @@
                 self.X = adata.layers[layer_key]
 
         else:
             self.X = adata.X
 
         clustering = KMeans(**kwargs).fit(self.X)
         adata.obs[cluster_key] = clustering.labels_
+        adata.obs[cluster_key] = adata.obs[cluster_key].astype("category")
 
         if return_object:
             return adata, clustering
 
         return adata
 
 
@@ -208,26 +243,31 @@
         adata: AnnData,
         layer_key: str = None,
         embedding_key: str = None,
         cluster_key: str = "dbscan",
         copy: bool = True,
         return_object: bool = False,
         **kwargs,
-    ) -> tuple[AnnData, object | AnnData]:
+    ) -> tuple[AnnData, object] | AnnData:
         """Computes a clustering using Density-based spatial clustering of applications (DBSCAN).
 
         Args:
             adata: Anndata object of size cells x genes
             layer_key: If specified and exists in the adata, the clustering is done by using it. Otherwise, clustering is done with .X
             embedding_key: if specified and exists in the adata, the clustering is done with that embedding. Otherwise, clustering is done with .X
             cluster_key: name of the .obs column to store the cluster labels. Defaults to 'dbscan'
             copy: if True returns a new Anndata of same size with the new column; otherwise it updates the initial adata
             return_object: if True returns the clustering object
             **kwargs: Are passed to sklearn's DBSCAN.
 
+        Returns:
+            If return_object is True, the adata and the clustering object is returned.
+            Otherwise, only the adata is returned. The adata is updated with a new .obs column as specified in cluster_key,
+            that stores the cluster labels.
+
         Examples:
             >>> import pertpy as pt
             >>> mdata = pt.dt.papalexi_2021()
             >>> dbscan = pt.tl.DBSCANSpace()
             >>> dbscan_adata = dbscan.compute(mdata["rna"])
         """
         if copy:
@@ -246,12 +286,13 @@
                 self.X = adata.layers[layer_key]
 
         else:
             self.X = adata.X
 
         clustering = DBSCAN(**kwargs).fit(self.X)
         adata.obs[cluster_key] = clustering.labels_
+        adata.obs[cluster_key] = adata.obs[cluster_key].astype("category")
 
         if return_object:
             return adata, clustering
 
         return adata
```

### Comparing `pertpy-0.6.0/pertpy/tools/_scgen/_base_components.py` & `pertpy-0.7.0/pertpy/tools/_scgen/_base_components.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/pertpy/tools/_scgen/_jax_scgenvae.py` & `pertpy-0.7.0/pertpy/tools/_scgen/_scgenvae.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/pertpy/tools/_scgen/_utils.py` & `pertpy-0.7.0/pertpy/tools/_scgen/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,15 @@
         .. code-block:: python
 
             import SCGEN
             import anndata
 
             train_data = anndata.read("./data/train.h5ad")
             test_data = anndata.read("./data/test.h5ad")
-            train_data_extracted_list = extractor(
-                train_data, "CD4T", "conditions", "cell_type", "control", "stimulated"
-            )
+            train_data_extracted_list = extractor(train_data, "CD4T", "conditions", "cell_type", "control", "stimulated")
     """
     cell_with_both_condition = data[data.obs[cell_type_key] == cell_type]
     condition_1 = data[(data.obs[cell_type_key] == cell_type) & (data.obs[condition_key] == ctrl_key)]
     condition_2 = data[(data.obs[cell_type_key] == cell_type) & (data.obs[condition_key] == stim_key)]
     training = data[~((data.obs[cell_type_key] == cell_type) & (data.obs[condition_key] == stim_key))]
 
     return [training, condition_1, condition_2, cell_with_both_condition]
```

### Comparing `pertpy-0.6.0/tests/preprocessing/test_grna_assignment.py` & `pertpy-0.7.0/tests/preprocessing/test_grna_assignment.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/tests/tools/r_result.csv` & `pertpy-0.7.0/tests/tools/r_result.csv`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/tests/tools/test_augur.py` & `pertpy-0.7.0/tests/tools/test_augur.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/tests/tools/test_cinemaot.py` & `pertpy-0.7.0/tests/tools/test_cinemaot.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/tests/tools/test_jax_scgen.py` & `pertpy-0.7.0/tests/tools/test_scgen.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,44 +8,43 @@
     adata = scvi.data.synthetic_iid()
     pt.tl.SCGEN.setup_anndata(
         adata,
         batch_key="batch",
         labels_key="labels",
     )
 
-    model = pt.tl.SCGEN(adata)
-    model.train(max_epochs=1, batch_size=32, early_stopping=True, early_stopping_patience=25)
+    scg = pt.tl.SCGEN(adata)
+    scg.train(max_epochs=1, batch_size=32, early_stopping=True, early_stopping_patience=25)
 
-    # batch Removal
-    model.batch_removal()
+    scg.batch_removal()
 
     # predict
-    pred, delta = model.predict(ctrl_key="batch_0", stim_key="batch_1", celltype_to_predict="label_0")
+    pred, delta = scg.predict(ctrl_key="batch_0", stim_key="batch_1", celltype_to_predict="label_0")
     pred.obs["batch"] = "pred"
 
     # reg mean and reg var
     ctrl_adata = adata[((adata.obs["labels"] == "label_0") & (adata.obs["batch"] == "batch_0"))]
     stim_adata = adata[((adata.obs["labels"] == "label_0") & (adata.obs["batch"] == "batch_1"))]
     eval_adata = AnnData.concatenate(ctrl_adata, stim_adata, pred, batch_key="concat_batches")
     label_0 = adata[adata.obs["labels"] == "label_0"]
     sc.tl.rank_genes_groups(label_0, groupby="batch", method="wilcoxon")
     diff_genes = label_0.uns["rank_genes_groups"]["names"]["batch_1"]
 
-    pt.pl.scg.reg_mean_plot(
+    scg.plot_reg_mean_plot(
         eval_adata,
         condition_key="batch",
         axis_keys={"x": "pred", "y": "batch_1"},
         gene_list=diff_genes[:10],
         labels={"x": "predicted", "y": "ground truth"},
         save=False,
         show=False,
         legend=False,
     )
 
-    pt.pl.scg.reg_var_plot(
+    scg.plot_reg_var_plot(
         eval_adata,
         condition_key="batch",
         axis_keys={"x": "pred", "y": "batch_1"},
         gene_list=diff_genes[:10],
         labels={"x": "predicted", "y": "ground truth"},
         save=False,
         show=False,
```

### Comparing `pertpy-0.6.0/tests/tools/test_milo.py` & `pertpy-0.7.0/tests/tools/test_milo.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,20 +244,23 @@
             ["ConditionA", "ConditionB"], size=sum(DA_cells), p=[0.2, 0.8]
         )
 
         # Simulate replicates
         adata.obs["replicate"] = rng.choice(["R1", "R2", "R3"], size=adata.n_obs)
         adata.obs["sample"] = adata.obs["replicate"] + adata.obs["condition"]
         milo_mdata = self.milo.count_nhoods(adata, sample_col="sample")
+
         return milo_mdata
 
     def test_add_nhood_expression_nhood_mean_range(self, add_nhood_expression_mdata):
         mdata = add_nhood_expression_mdata.copy()
         self.milo.add_nhood_expression(mdata)
+
         assert mdata["milo"].varm["expr"].shape[1] == mdata["rna"].n_vars
+
         mdata = add_nhood_expression_mdata.copy()
         self.milo.add_nhood_expression(mdata)
         nhood_ix = 10
         nhood_gex = mdata["milo"].varm["expr"][nhood_ix, :].toarray().ravel()
         nhood_cells = mdata["rna"].obs_names[mdata["rna"].obsm["nhoods"][:, nhood_ix].toarray().ravel() == 1]
         mean_gex = np.array(mdata["rna"][nhood_cells].X.mean(axis=0)).ravel()
         assert nhood_gex == pytest.approx(mean_gex, 0.0001)
```

### Comparing `pertpy-0.6.0/tests/tools/test_mixscape.py` & `pertpy-0.7.0/tests/tools/test_mixscape.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/tests/tools/_coda/test_sccoda.py` & `pertpy-0.7.0/tests/tools/_coda/test_sccoda.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/tests/tools/_coda/test_tasccoda.py` & `pertpy-0.7.0/tests/tools/_coda/test_tasccoda.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class TesttascCODA:
     tasccoda = pt.tl.Tasccoda()
 
     @pytest.fixture
     def smillie_adata(self):
-        smillie_adata = pt.dt.smillie()
+        smillie_adata = pt.dt.tasccoda_example()
         smillie_adata = sc.pp.subsample(smillie_adata, 0.1, copy=True)
 
         return smillie_adata
 
     def test_load(self, smillie_adata):
         mdata = self.tasccoda.load(
             smillie_adata,
```

### Comparing `pertpy-0.6.0/tests/tools/_distances/test_distance_tests.py` & `pertpy-0.7.0/tests/tools/_distances/test_distance_tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,20 @@
     "spearman_distance",
     "kendalltau_distance",
     "cosine_distance",
     "wasserstein",
     "mean_pairwise",
     "mmd",
     "r2_distance",
-    "kl_divergence",
+    "sym_kldiv",
     "t_test",
+    "ks_test",
+    "classifier_proba",
+    # "classifier_cp",
+    # "nbll",
 ]
 
 count_distances = ["nb_ll"]
 
 
 class TestPermutationTest:
     @fixture
```

### Comparing `pertpy-0.6.0/tests/tools/_distances/test_distances.py` & `pertpy-0.7.0/tests/tools/_distances/test_distances.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,40 @@
 import pertpy as pt
 import pytest
 import scanpy as sc
 from pandas import DataFrame, Series
 from pytest import fixture, mark
 
 actual_distances = [
+    # Euclidean distances and related
     "euclidean",
-    "mse",
     "mean_absolute_error",
+    "mean_pairwise",
+    "mse",
+    "edistance",
+    # Other
+    "cosine_distance",
+    "kendalltau_distance",
+    "mmd",
     "pearson_distance",
     "spearman_distance",
-    "kendalltau_distance",
-    "cosine_distance",
+    "t_test",
     "wasserstein",
 ]
-pseudo_distances = ["mean_pairwise", "mmd", "r2_distance", "kl_divergence", "t_test", "edistance"]
+semi_distances = ["r2_distance", "sym_kldiv", "ks_test"]
+non_distances = ["classifier_proba"]
+onesided_only = ["classifier_cp"]
 pseudo_counts_distances = ["nb_ll"]
+all_distances = actual_distances + semi_distances + non_distances  # + onesided_only + pseudo_counts_distances
 
 
 class TestDistances:
     @fixture
     def adata(self, request):
-        no_subsample_distances = ["kl_divergence", "t_test"]
+        no_subsample_distances = ["sym_kldiv", "t_test", "ks_test", "classifier_proba", "classifier_cp"]
         distance = request.node.callspec.params["distance"]
 
         adata = pt.dt.distance_example()
         if distance not in no_subsample_distances:
             adata = sc.pp.subsample(adata, 0.001, copy=True)
         else:
             adata = sc.pp.subsample(adata, 0.1, copy=True)
@@ -34,90 +43,92 @@
         adata.layers["lognorm"] = adata.X.copy()
         adata.layers["counts"] = np.round(adata.X.toarray()).astype(int)
         if "X_pca" not in adata.obsm.keys():
             sc.pp.pca(adata, n_comps=10)
 
         return adata
 
-    @mark.parametrize("distance", actual_distances)
+    @mark.parametrize("distance", all_distances)
+    def test_distance(self, adata, distance):
+        Distance = pt.tl.Distance(distance, obsm_key="X_pca")
+        df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
+
+        assert isinstance(df, DataFrame)
+
+    @mark.parametrize("distance", actual_distances + semi_distances)
     def test_distance_axioms(self, adata, distance):
-        # Test if distances are well-defined in accordance with metric axioms
+        # This is equivalent to testing for a semimetric, defined as fulfilling all axioms except triangle inequality.
         Distance = pt.tl.Distance(distance, obsm_key="X_pca")
         df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
 
-        # (M1) Positiv definiteness
+        # (M1) Definiteness
         assert all(np.diag(df.values) == 0)  # distance to self is 0
+
+        # (M2) Positivity
         assert len(df) == np.sum(df.values == 0)  # distance to other is not 0
         assert all(df.values.flatten() >= 0)  # distance is non-negative
 
-        # (M2) Symmetry
+        # (M3) Symmetry
         assert np.sum(df.values - df.values.T) == 0
-        assert df.columns.equals(df.index)
 
-        # (M3) Triangle inequality (we just probe this for a few random triplets)
+    @mark.parametrize("distance", actual_distances)
+    def test_triangle_inequality(self, adata, distance):
+        # Test if distances are well-defined in accordance with metric axioms
+        Distance = pt.tl.Distance(distance, obsm_key="X_pca")
+        df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
+
+        # (M4) Triangle inequality (we just probe this for a few random triplets)
         for _i in range(10):
             rng = np.random.default_rng()
             triplet = rng.choice(df.index, size=3, replace=False)
             assert df.loc[triplet[0], triplet[1]] + df.loc[triplet[1], triplet[2]] >= df.loc[triplet[0], triplet[2]]
 
-    @mark.parametrize("distance", actual_distances + pseudo_distances)
-    def test_distance(self, adata, distance):
-        Distance = pt.tl.Distance(distance, obsm_key="X_pca")
-        df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
-
-        assert isinstance(df, DataFrame)
-        assert df.columns.equals(df.index)
-        assert np.sum(df.values - df.values.T) == 0  # symmetry
-
-    @mark.parametrize("distance", actual_distances + pseudo_distances)
+    @mark.parametrize("distance", all_distances)
     def test_distance_layers(self, adata, distance):
         Distance = pt.tl.Distance(distance, layer_key="lognorm")
-        df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
+        df = Distance.pairwise(adata, groupby="perturbation")
 
         assert isinstance(df, DataFrame)
         assert df.columns.equals(df.index)
         assert np.sum(df.values - df.values.T) == 0  # symmetry
 
-    # SP: this is giving error "numpy.linalg.LinAlgError: Singular matrix"
-    # @mark.parametrize("distance", actual_distances + pseudo_counts_distances)
-    # def test_distance_counts(self, adata, distance):
-    #     Distance = pt.tl.Distance(distance, layer_key="counts")
-    #     df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
-    #     assert isinstance(df, DataFrame)
-    #     assert df.columns.equals(df.index)
-    #     assert np.sum(df.values - df.values.T) == 0
+    @mark.parametrize("distance", actual_distances + pseudo_counts_distances)
+    def test_distance_counts(self, adata, distance):
+        Distance = pt.tl.Distance(distance, layer_key="counts")
+        df = Distance.pairwise(adata, groupby="perturbation")
+        assert isinstance(df, DataFrame)
+        assert df.columns.equals(df.index)
+        assert np.sum(df.values - df.values.T) == 0
 
-    @mark.parametrize("distance", actual_distances)
+    @mark.parametrize("distance", all_distances)
     def test_mutually_exclusive_keys(self, adata, distance):
         with pytest.raises(ValueError):
             _ = pt.tl.Distance(distance, layer_key="counts", obsm_key="X_pca")
 
-    @mark.parametrize("distance", actual_distances + pseudo_distances)
+    @mark.parametrize("distance", all_distances)
     def test_distance_output_type(self, distance):
         # Test if distances are outputting floats
         Distance = pt.tl.Distance(distance, obsm_key="X_pca")
         rng = np.random.default_rng()
         X = rng.normal(size=(100, 10))
         Y = rng.normal(size=(100, 10))
         d = Distance(X, Y)
         assert isinstance(d, float)
 
-    @mark.parametrize("distance", actual_distances + pseudo_distances)
+    @mark.parametrize("distance", all_distances)
     def test_distance_pairwise(self, adata, distance):
         # Test consistency of pairwise distance results
         Distance = pt.tl.Distance(distance, obsm_key="X_pca")
-        df = Distance.pairwise(adata, groupby="perturbation", show_progressbar=True)
+        df = Distance.pairwise(adata, groupby="perturbation")
 
         assert isinstance(df, DataFrame)
         assert df.columns.equals(df.index)
         assert np.sum(df.values - df.values.T) == 0  # symmetry
 
-    @mark.parametrize("distance", actual_distances + pseudo_distances)
+    @mark.parametrize("distance", all_distances + onesided_only)
     def test_distance_onesided(self, adata, distance):
         # Test consistency of one-sided distance results
         Distance = pt.tl.Distance(distance, obsm_key="X_pca")
         selected_group = adata.obs.perturbation.unique()[0]
-        df = Distance.onesided_distances(
-            adata, groupby="perturbation", selected_group=selected_group, show_progressbar=True
-        )
+        df = Distance.onesided_distances(adata, groupby="perturbation", selected_group=selected_group)
         assert isinstance(df, Series)
         assert df.loc[selected_group] == 0  # distance to self is 0
```

### Comparing `pertpy-0.6.0/tests/tools/_metadata/test_cell_line.py` & `pertpy-0.7.0/tests/metadata/test_cell_line.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,86 +8,70 @@
 
 NUM_CELLS = 100
 NUM_GENES = 100
 NUM_CELLS_PER_ID = NUM_CELLS // 4
 
 
 class TestMetaData:
-    pt_metadata = pt.tl.CellLineMetaData()
+    pt_metadata = pt.md.CellLine()
 
     @pytest.fixture
     def adata(self) -> AnnData:
         rng = np.random.default_rng(seed=1)
 
         X = rng.normal(0, 1, (NUM_CELLS, NUM_GENES))
         X = np.where(X < 0, 0, X)
 
-        cell_line = {
-            "DepMap_ID": ["ACH-000016"] * NUM_CELLS_PER_ID
-            + ["ACH-000049"] * NUM_CELLS_PER_ID
-            + ["ACH-001208"] * NUM_CELLS_PER_ID
-            + ["ACH-000956"] * NUM_CELLS_PER_ID
-        }
-        cell_line = pd.DataFrame(cell_line)
-        obs = pd.concat([cell_line], axis=1)
-        obs = obs.set_index(pd.Index([str(i) for i in range(NUM_GENES)]))
-        obs.index.rename("index", inplace=True)
-        obs["perturbation"] = "Midostaurin"
-
-        var_data = {"gene_name": ["gene" + str(i) for i in range(1, NUM_GENES + 1)]}
-        var = pd.DataFrame(var_data)
-        var = var.set_index("gene_name", drop=False)
-        var.index.rename("index", inplace=True)
+        obs = pd.DataFrame(
+            {
+                "DepMap_ID": ["ACH-000016", "ACH-000049", "ACH-001208", "ACH-000956"] * NUM_CELLS_PER_ID,
+                "perturbation": ["Midostaurin"] * NUM_CELLS_PER_ID * 4,
+            },
+            index=[str(i) for i in range(NUM_GENES)],
+        )
+
+        var_data = {"gene_name": [f"gene{i}" for i in range(1, NUM_GENES + 1)]}
+        var = pd.DataFrame(var_data).set_index("gene_name", drop=False).rename_axis("index")
 
         X = sparse.csr_matrix(X)
         adata = anndata.AnnData(X=X, obs=obs, var=var)
 
         return adata
 
     def test_cell_line_annotation(self, adata):
-        self.pt_metadata.annotate_cell_lines(adata=adata)
-        assert (
-            len(adata.obs.columns) == len(self.pt_metadata.cell_line_meta.columns) + 1
-        )  # due to the perturbation column
-        assert set(self.pt_metadata.cell_line_meta.columns).issubset(adata.obs)
-        stripped_cell_line_name = (
-            ["SLR21"] * NUM_CELLS_PER_ID
-            + ["HEKTE"] * NUM_CELLS_PER_ID
-            + ["TK10"] * NUM_CELLS_PER_ID
-            + ["22RV1"] * NUM_CELLS_PER_ID
-        )
-
-        assert stripped_cell_line_name == list(adata.obs["stripped_cell_line_name"])
+        self.pt_metadata.annotate(adata=adata)
+        assert len(adata.obs.columns) == len(self.pt_metadata.depmap.columns) + 1  # due to the perturbation column
+        stripped_cell_line_name = ["SLR21", "HEKTE", "TK10", "22RV1"] * NUM_CELLS_PER_ID
+        assert stripped_cell_line_name == list(adata.obs["StrippedCellLineName"])
 
     def test_gdsc_annotation(self, adata):
-        self.pt_metadata.annotate_cell_lines(adata)
-        self.pt_metadata.annotate_from_gdsc(adata, query_id="stripped_cell_line_name")
-        assert "drug_name" in adata.obs
+        self.pt_metadata.annotate(adata)
+        self.pt_metadata.annotate_from_gdsc(adata, query_id="StrippedCellLineName")
         assert "ln_ic50" in adata.obs
 
     def test_protein_expression_annotation(self, adata):
-        self.pt_metadata.annotate_cell_lines(adata)
-        self.pt_metadata.annotate_protein_expression(adata, query_id="stripped_cell_line_name")
+        self.pt_metadata.annotate(adata)
+        self.pt_metadata.annotate_protein_expression(adata, query_id="StrippedCellLineName")
 
         assert len(adata.obsm) == 1
         assert adata.obsm["proteomics_protein_intensity"].shape == (
             NUM_GENES,
-            len(self.pt_metadata.proteomics_data.uniprot_id.unique()),
+            len(self.pt_metadata.proteomics.uniprot_id.unique()),
         )
 
     def test_bulk_rna_expression_annotation(self, adata):
-        self.pt_metadata.annotate_cell_lines(adata)
-        self.pt_metadata.annotate_bulk_rna_expression(adata, query_id="DepMap_ID", cell_line_source="broad")
+        self.pt_metadata.annotate(adata)
+        self.pt_metadata.annotate_bulk_rna(adata, query_id="DepMap_ID", cell_line_source="broad")
 
         assert len(adata.obsm) == 1
-        assert adata.obsm["bulk_rna_expression_broad"].shape == (
+        assert adata.obsm["bulk_rna_broad"].shape == (
             NUM_GENES,
             self.pt_metadata.bulk_rna_broad.shape[1],
         )
 
-        self.pt_metadata.annotate_bulk_rna_expression(adata, query_id="stripped_cell_line_name")
+        self.pt_metadata.annotate_bulk_rna(adata, query_id="StrippedCellLineName")
 
         assert len(adata.obsm) == 2
-        assert adata.obsm["bulk_rna_expression_sanger"].shape == (
+        assert adata.obsm["bulk_rna_sanger"].shape == (
             NUM_GENES,
             self.pt_metadata.bulk_rna_sanger.shape[1],
         )
```

### Comparing `pertpy-0.6.0/tests/tools/_perturbation_space/test_discriminator_classifier.py` & `pertpy-0.7.0/tests/tools/_perturbation_space/test_simple_cluster_space.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 import numpy as np
 import pandas as pd
 import pertpy as pt
 from anndata import AnnData
 
 
-def test_discriminator_classifier():
-    X = np.zeros((20, 5))
+def test_clustering():
+    X = np.zeros((10, 5))
 
     pert_index = [
         "control",
         "target1",
         "target1",
         "target2",
         "target2",
         "target1",
         "target1",
         "target2",
         "target2",
         "target2",
-        "control",
-        "target1",
-        "target1",
-        "target2",
-        "target2",
-        "target1",
-        "target1",
-        "target2",
-        "target2",
-        "target2",
     ]
 
     for i, value in enumerate(pert_index):
         if value == "control":
             X[i, :] = 0
         elif value == "target1":
             X[i, :] = 10
         elif value == "target2":
             X[i, :] = 30
 
     obs = pd.DataFrame({"perturbations": pert_index})
 
     adata = AnnData(X, obs=obs)
 
-    # Compute the embeddings using the classifier
-    ps = pt.tl.DiscriminatorClassifierSpace()
-    classifier_ps = ps.load(adata)
-    classifier_ps.train(max_epochs=5)
-    pert_embeddings = classifier_ps.get_embeddings()
-
-    # The embeddings should cluster in 3 perfects clusters since the perturbations are easily separable
+    # Compute clustering at observation level
     ps = pt.tl.KMeansSpace()
-    adata = ps.compute(pert_embeddings, n_clusters=3, copy=True)
-    results = ps.evaluate_clustering(adata, true_label_col="perturbations", cluster_col="k-means")
+    adata = ps.compute(adata, n_clusters=3, copy=True)
+
+    ps = pt.tl.DBSCANSpace()
+    adata = ps.compute(adata, min_samples=1, copy=True)
+
+    results = ps.evaluate_clustering(adata, true_label_col="perturbations", cluster_col="k-means", metric="l1")
     np.testing.assert_equal(len(results), 3)
     np.testing.assert_allclose(results["nmi"], 0.99, rtol=0.1)
     np.testing.assert_allclose(results["ari"], 0.99, rtol=0.1)
     np.testing.assert_allclose(results["asw"], 0.99, rtol=0.1)
+
+    results = ps.evaluate_clustering(adata, true_label_col="perturbations", cluster_col="dbscan", metric="l1")
+    np.testing.assert_equal(len(results), 3)
+    np.testing.assert_allclose(results["nmi"], 0.99, rtol=0.1)
+    np.testing.assert_allclose(results["ari"], 0.99, rtol=0.1)
+    np.testing.assert_allclose(results["asw"], 0.99, rtol=0.1)
+
+    np.testing.assert_allclose(results["nmi"], 0.99, rtol=0.1)
+    np.testing.assert_allclose(results["ari"], 0.99, rtol=0.1)
+    np.testing.assert_allclose(results["asw"], 0.99, rtol=0.1)
```

### Comparing `pertpy-0.6.0/tests/tools/_perturbation_space/test_simple_perturbation_space.py` & `pertpy-0.7.0/tests/tools/_perturbation_space/test_simple_perturbation_space.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 import numpy as np
 import pandas as pd
 import pertpy as pt
 import pytest
+import scanpy as sc
 from anndata import AnnData
 
 
-def test_differential_response():
-    rng = np.random.default_rng()
+@pytest.fixture
+def adata(rng):
+    X = rng.random((69, 50))
+    adata = AnnData(X)
+    perturbations = np.array(["control", "target1", "target2"] * 22 + ["unknown"] * 3)
+    adata.obs["perturbation"] = perturbations
+    sc.pp.pca(adata)
+    sc.pp.neighbors(adata, use_rep="X")
+    sc.tl.umap(adata)
+
+    return adata
+
+
+@pytest.fixture
+def adata_simple(rng):
     X = rng.random(size=(10, 5))
     obs = pd.DataFrame(
         {
-            "perturbations": [
+            "perturbation": [
                 "control",
                 "target1",
                 "target1",
                 "target2",
                 "target2",
                 "target1",
                 "target1",
@@ -22,89 +36,63 @@
                 "target2",
                 "target2",
             ]
         }
     )
     adata = AnnData(X, obs=obs)
 
-    # Compute the differential response
+    return adata
+
+
+def test_differential_response(adata_simple):
     ps = pt.tl.PseudobulkSpace()
-    ps_adata = ps.compute_control_diff(adata, copy=True)
+    ps_adata = ps.compute_control_diff(adata_simple, target_col="perturbation", copy=True)
 
-    # Test that the differential response was computed correctly
-    expected_diff_matrix = adata.X - adata.X[0, :]
+    expected_diff_matrix = adata_simple.X - adata_simple.X[0, :]
     np.testing.assert_allclose(ps_adata.X, expected_diff_matrix, rtol=1e-4)
 
-    # Check that the function raises an error if the reference key is not found
     with pytest.raises(ValueError):
         ps.compute_control_diff(
-            adata,
-            target_col="perturbations",
+            adata_simple,
+            target_col="perturbation",
             reference_key="not_found",
             layer_key="counts",
             new_layer_key="counts_diff",
             embedding_key="X_pca",
             new_embedding_key="pca_diff",
             copy=True,
         )
 
 
-def test_pseudobulk_response():
-    rng = np.random.default_rng()
-    X = rng.random(size=(10, 5))
-    obs = pd.DataFrame(
-        {
-            "perturbations": [
-                "control",
-                "target1",
-                "target1",
-                "target2",
-                "target2",
-                "target1",
-                "target1",
-                "target2",
-                "target2",
-                "target2",
-            ]
-        }
-    )
-    adata = AnnData(X, obs=obs)
-
-    # Compute the pseudobulk
+def test_pseudobulk_response(adata_simple):
     ps = pt.tl.PseudobulkSpace()
-    psadata = ps.compute(adata, mode="mean", min_cells=0, min_counts=0)
+    psadata = ps.compute(adata_simple, mode="mean", min_cells=0, min_counts=0)
 
-    # Test that the pseudobulk response was computed correctly
-    adata_target1 = adata[adata.obs.perturbations == "target1"].X.mean(0)
+    adata_target1 = adata_simple[adata_simple.obs.perturbation == "target1"].X.mean(0)
     np.testing.assert_allclose(adata_target1, psadata["target1"].X[0], rtol=1e-4)
 
-    # Test in UMAP space
-    adata.obsm["X_umap"] = X
+    adata_simple.obsm["X_umap"] = adata_simple.X
 
-    # Compute the pseudobulk
     ps = pt.tl.PseudobulkSpace()
-    psadata = ps.compute(adata, embedding_key="X_umap", mode="mean", min_cells=0, min_counts=0)
+    psadata = ps.compute(adata_simple, embedding_key="X_umap", mode="mean", min_cells=0, min_counts=0)
 
-    # Test that the pseudobulk response was computed correctly
-    adata_target1 = adata[adata.obs.perturbations == "target1"].obsm["X_umap"].mean(0)
+    adata_target1 = adata_simple[adata_simple.obs.perturbation == "target1"].obsm["X_umap"].mean(0)
     np.testing.assert_allclose(adata_target1, psadata["target1"].X[0], rtol=1e-4)
 
-    # Check that the function raises an error if the layer key is not found
     with pytest.raises(ValueError):
         ps.compute(
-            adata,
-            target_col="perturbations",
+            adata_simple,
+            target_col="perturbation",
             layer_key="not_found",
         )
 
-    # Check that the function raises an error if the layer key and embedding key are used at the same time
     with pytest.raises(ValueError):
         ps.compute(
-            adata,
-            target_col="perturbations",
+            adata_simple,
+            target_col="perturbation",
             embedding_key="not_found",
             layer_key="not_found",
         )
 
 
 def test_centroid_umap_response():
     X = np.zeros((10, 5))
@@ -126,59 +114,54 @@
         if value == "control":
             X[i, :] = 0
         elif value == "target1":
             X[i, :] = 10
         elif value == "target2":
             X[i, :] = 30
 
-    obs = pd.DataFrame({"perturbations": pert_index})
+    obs = pd.DataFrame({"perturbation": pert_index})
 
     adata = AnnData(X, obs=obs)
     adata.obsm["X_umap"] = X
 
-    # Compute the centroids
     ps = pt.tl.CentroidSpace()
     psadata = ps.compute(adata, embedding_key="X_umap")
 
-    # Test that the centroids response was computed correctly
-    adata_target1 = adata[adata.obs.perturbations == "target1"].obsm["X_umap"].mean(0)
+    adata_target1 = adata[adata.obs.perturbation == "target1"].obsm["X_umap"].mean(0)
     np.testing.assert_allclose(adata_target1, psadata["target1"].X[0], rtol=1e-4)
 
     ps = pt.tl.CentroidSpace()
-    psadata = ps.compute(adata)  # if nothing specific, compute with X, and X and X_umap are the same
+    psadata = ps.compute(adata)
 
-    # Test that the centroids response was computed correctly
-    adata_target1 = adata[adata.obs.perturbations == "target1"].obsm["X_umap"].mean(0)
+    adata_target1 = adata[adata.obs.perturbation == "target1"].obsm["X_umap"].mean(0)
     np.testing.assert_allclose(adata_target1, psadata["target1"].X[0], rtol=1e-4)
 
-    # Check that the function raises an error if the embedding key is not found
     with pytest.raises(ValueError):
         ps.compute(
             adata,
-            target_col="perturbations",
+            target_col="perturbation",
             embedding_key="not_found",
         )
 
-    # Check that the function raises an error if the layer key and embedding key are used at the same time
     with pytest.raises(ValueError):
         ps.compute(
             adata,
-            target_col="perturbations",
+            target_col="perturbation",
             embedding_key="not_found",
             layer_key="not_found",
         )
 
 
 def test_linear_operations():
     """Tests add/subtract and other linear operations."""
     rng = np.random.default_rng()
     X = rng.random(size=(10, 5))
     obs = pd.DataFrame(
         {
-            "perturbations": [
+            "perturbation": [
                 "control",
                 "target1",
                 "target1",
                 "target2",
                 "target2",
                 "target1",
                 "target1",
@@ -187,79 +170,79 @@
                 "target2",
             ]
         }
     )
     adata = AnnData(X, obs=obs)
     adata.obsm["X_umap"] = X
 
-    # Compute pseudobulk
     ps = pt.tl.PseudobulkSpace()
     psadata = ps.compute(adata, mode="mean", min_cells=0, min_counts=0)
 
     psadata_umap = ps.compute(adata, mode="mean", min_cells=0, min_counts=0, embedding_key="X_umap")
     psadata.obsm["X_umap"] = psadata_umap.X
 
-    # Perform summation
     ps_adata, data_compare = ps.add(psadata, perturbations=["target1", "target2"], ensure_consistency=True)
 
-    # Test in X
     test = data_compare["control"].X + data_compare["target1"].X + data_compare["target2"].X
     np.testing.assert_allclose(test, ps_adata["target1+target2"].X, rtol=1e-4)
 
-    # Test in UMAP embedding
     test = (
         data_compare["control"].obsm["X_umap_control_diff"]
         + data_compare["target1"].obsm["X_umap_control_diff"]
         + data_compare["target2"].obsm["X_umap_control_diff"]
     )
     np.testing.assert_allclose(test, ps_adata["target1+target2"].obsm["X_umap"], rtol=1e-4)
 
-    # Perform subtraction
     ps_adata, data_compare = ps.subtract(
         psadata, reference_key="target1", perturbations=["target2"], ensure_consistency=True
     )
 
-    # Test in X
     test = data_compare["target1"].X - data_compare["target2"].X
     np.testing.assert_allclose(test, ps_adata["target1-target2"].X, rtol=1e-4)
 
-    # Operations after control diff, do the results match?
     ps_adata = ps.compute_control_diff(psadata, copy=True)
 
-    # Do summation
     ps_adata2 = ps.add(ps_adata, perturbations=["target1", "target2"])
 
-    # Test in X
     test = ps_adata["control"].X + ps_adata["target1"].X + ps_adata["target2"].X
     np.testing.assert_allclose(test, ps_adata2["target1+target2"].X, rtol=1e-4)
 
-    # Do subtract
     ps_adata2 = ps.subtract(ps_adata, reference_key="target1", perturbations=["target1"])
     ps_vector = ps_adata2["target1-target1"].X
     np.testing.assert_allclose(ps_adata2["control"].X, ps_adata2["target1-target1"].X, rtol=1e-4)
 
     ps_adata2, data_compare = ps.subtract(
         ps_adata, reference_key="target1", perturbations=["target1"], ensure_consistency=True
     )
     ps_inner_vector = ps_adata2["target1-target1"].X
 
-    # Compare process data vs pseudobulk before, should be the same
     np.testing.assert_allclose(ps_inner_vector, ps_vector, rtol=1e-4)
 
-    # Check result in UMAP
     np.testing.assert_allclose(
         data_compare["control"].obsm["X_umap_control_diff"], ps_adata2["target1-target1"].obsm["X_umap"], rtol=1e-4
     )
 
-    # Check that the function raises an error if the perturbation is not found
     with pytest.raises(ValueError):
         ps.add(
             ps_adata,
             perturbations=["target1", "target3"],
         )
 
-    # Check that the function raises an error if some key is not found
     with pytest.raises(ValueError):
         ps.add(
             ps_adata,
             perturbations=["target1", "target3"],
         )
+
+
+def test_label_transfer():
+    rng = np.random.default_rng()
+    X = rng.standard_normal((69, 50))
+    adata = AnnData(X)
+    perturbations = np.array(["A", "B", "C"] * 22 + ["unknown"] * 3)
+    adata.obs["perturbation"] = perturbations
+    sc.pp.neighbors(adata, use_rep="X")
+    sc.tl.umap(adata)
+
+    ps = pt.tl.PseudobulkSpace()
+    ps.label_transfer(adata, n_neighbors=5, use_rep="X_umap")
+    assert "unknown" not in adata.obs["perturbation"]
```

### Comparing `pertpy-0.6.0/.gitignore` & `pertpy-0.7.0/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -149,7 +149,9 @@
 cache
 
 # Apple stuff
 .DS_Store
 
 lightning_logs/*
 */lightning_logs/*
+
+node_modules
```

### Comparing `pertpy-0.6.0/LICENSE` & `pertpy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pertpy-0.6.0/README.md` & `pertpy-0.7.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Build](https://github.com/theislab/pertpy/actions/workflows/build.yml/badge.svg)](https://github.com/theislab/pertpy/actions/workflows/build.yml)
-[![Codecov](https://codecov.io/gh/theislab/pertpy/branch/master/graph/badge.svg)](https://codecov.io/gh/theislab/pertpy)
+[![codecov](https://codecov.io/gh/theislab/pertpy/graph/badge.svg?token=1dTpIPBShv)](https://codecov.io/gh/theislab/pertpy)
 [![License](https://img.shields.io/github/license/theislab/pertpy)](https://opensource.org/licenses/Apache2.0)
 [![PyPI](https://img.shields.io/pypi/v/pertpy.svg)](https://pypi.org/project/pertpy/)
 [![Python Version](https://img.shields.io/pypi/pyversions/pertpy)](https://pypi.org/project/pertpy)
 [![Read the Docs](https://img.shields.io/readthedocs/pertpy/latest.svg?label=Read%20the%20Docs)](https://pertpy.readthedocs.io/)
 [![Test](https://github.com/theislab/pertpy/actions/workflows/test.yml/badge.svg)](https://github.com/theislab/pertpy/actions/workflows/test.yml)
 [![PyPI](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 # pertpy
 
-![pertpy-wide1](https://user-images.githubusercontent.com/21954664/235677503-0c72f90d-3f6d-4a16-a1ff-ff8c11a540fb.png)
+![fig1](https://github.com/theislab/pertpy/assets/99650244/182fa9c3-6d23-4002-b86a-82bf2a243377)
 
 ## Documentation
 
 Please read the [documentation](https://pertpy.readthedocs.io/en/latest).
 
 ## Installation
 
 You can install _pertpy_ via [pip] from [PyPI]:
 
 ```console
-$ pip install pertpy
+pip install pertpy
+```
+
+if you want to use scCODA please install it as:
+
+```console
+pip install pertpy[coda]
 ```
 
 [pip]: https://pip.pypa.io/
 [pypi]: https://pypi.org/
 [usage]: https://pertpy.readthedocs.io/en/latest/usage/usage.html
```

### Comparing `pertpy-0.6.0/pyproject.toml` & `pertpy-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "pertpy"
-version = "0.6.0"
+version = "0.7.0"
 description = "Perturbation Analysis in the scverse ecosystem."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = {file = "LICENSE"}
 authors = [
     {name = "Lukas Heumos"},
     {name = "Yuge Ji"},
     {name = "Alejandro Tejada"},
     {name = "Johannes Köster"},
     {name = "Emma Dann"},
     {name = "Xinyue Zhang"},
     {name = "Xichen Wu"},
     {name = "Amir Moinfar"},
     {name = "Sergei Rybakov"},
     {name = "Tessa Green"},
     {name = "Stefan Peidli"},
     {name = "Antonia Schumacher"},
+    {name = "Lilly May"},
 ]
 maintainers = [
     {name = "Lukas Heumos", email = "lukas.heumos@posteo.net"},
 ]
 urls.Documentation = "https://pertpy.readthedocs.io"
 urls.Source = "https://github.com/theislab/pertpy"
 urls.Home-page = "https://github.com/theislab/pertpy"
+
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Development Status :: 4 - Beta",
+    "Environment :: Console",
+    "Framework :: Jupyter",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "Natural Language :: English",
+    "Operating System :: MacOS :: MacOS X",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering :: Bio-Informatics",
+    "Topic :: Scientific/Engineering :: Visualization",
+]
+
 dependencies = [
-    "anndata",
     "rich",
     "scanpy[leiden]",
     "muon",
     "requests",
-    "ipywidgets",
     "scikit-misc",
-    "plotnine",
     "scipy",
     "scvi-tools",
     "adjusttext",
     "toytree",
     "arviz",
     "numpyro",
     "decoupler",
     "ott-jax",
     "sparsecca",
-    "numba",
     "openpyxl",
+    "pubchempy",
+    "pyarrow",
+    "blitzgsea"
 ]
 
 [project.optional-dependencies]
 coda = [
     "ete3",
     "pyqt5"  # remove this after ete4 got released
 ]
@@ -79,28 +97,28 @@
     "nbsphinx",
     "nbsphinx-link",
     "ipykernel",
     "ipython",
 ]
 test = [
     "pytest",
-    "pytest-cov",
+    "coverage",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.coverage.run]
-source = ["pertpy"]
+source_pkgs = ["pertpy"]
 omit = [
     "**/test_*.py",
 ]
 
 [tool.pytest.ini_options]
-testpaths = "pertpy/tests"
+testpaths = "tests"
 xfail_strict = true
 addopts = [
     "--import-mode=importlib",  # allow using test files with same name
 ]
 markers = [
     "conda: marks a subset of tests to be ran on the Bioconda CI.",
     "extra: marks tests that require extra dependencies."
@@ -108,14 +126,19 @@
 minversion = 6.0
 norecursedirs = [ '.*', 'build', 'dist', '*.egg', 'data', '__pycache__']
 
 
 [tool.ruff]
 src = ["src"]
 line-length = 120
+
+[tool.ruff.format]
+docstring-code-format = true
+
+[tool.ruff.lint]
 select = [
     "F",  # Errors detected by Pyflakes
     "E",  # Error detected by Pycodestyle
     "W",  # Warning detected by Pycodestyle
     "I",  # isort
     #"D",  # pydocstyle
     "B",  # flake8-bugbear
@@ -158,18 +181,18 @@
     "F401",
     # camcelcase imported as lowercase
     "N813",
     # module import not at top level of file
     "E402",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "docs/*" = ["I"]
 "tests/*" = ["D"]
 "*/__init__.py" = ["F401"]
 
 [tool.mypy]
 strict = false
 pretty = true
```

