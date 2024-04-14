# Comparing `tmp/pdfly-0.3.1.tar.gz` & `tmp/pdfly-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfly-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pdfly-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pdfly-0.3.1.tar` & `pdfly-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,60 @@
--rw-r--r--   0        0        0      160 2024-03-29 08:15:04.114267 pdfly-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2591 2024-03-29 08:15:04.114267 pdfly-0.3.1/.github/workflows/github-ci.yaml
--rw-r--r--   0        0        0     3040 2024-03-29 08:15:04.114267 pdfly-0.3.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1987 2024-03-29 08:15:04.114267 pdfly-0.3.1/.gitignore
--rw-r--r--   0        0        0       94 2024-03-29 08:15:04.114267 pdfly-0.3.1/.gitmodules
--rw-r--r--   0        0        0      168 2024-03-29 08:15:04.114267 pdfly-0.3.1/.isort.cfg
--rw-r--r--   0        0        0     1463 2024-03-29 08:15:04.114267 pdfly-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      542 2024-03-29 08:15:04.114267 pdfly-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1654 2024-03-29 08:15:04.114267 pdfly-0.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     1670 2024-03-29 08:15:04.114267 pdfly-0.3.1/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1514 2024-03-29 08:15:04.114267 pdfly-0.3.1/LICENSE
--rw-r--r--   0        0        0      744 2024-03-29 08:15:04.114267 pdfly-0.3.1/Makefile
--rw-r--r--   0        0        0     4262 2024-03-29 08:15:04.114267 pdfly-0.3.1/README.md
--rw-r--r--   0        0        0      634 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/Makefile
--rw-r--r--   0        0        0     4160 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/conf.py
--rw-r--r--   0        0        0      704 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/make.bat
--rw-r--r--   0        0        0     6520 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/meta/project-governance.md
--rw-r--r--   0        0        0     1272 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/user/installation.md
--rw-r--r--   0        0        0     3493 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/user/subcommand-cat.md
--rw-r--r--   0        0        0     5673 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/user/subcommand-meta.md
--rw-r--r--   0        0        0     2024 2024-03-29 08:15:04.114267 pdfly-0.3.1/docs/user/subcommand-x2pdf.md
--rw-r--r--   0        0        0    10213 2024-03-29 08:15:04.114267 pdfly-0.3.1/make_release.py
--rw-r--r--   0        0        0       31 2024-03-29 08:15:04.114267 pdfly-0.3.1/mypy.ini
--rw-r--r--   0        0        0      164 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/__init__.py
--rw-r--r--   0        0        0      114 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/__main__.py
--rw-r--r--   0        0        0       87 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/_utils.py
--rw-r--r--   0        0        0       22 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/_version.py
--rw-r--r--   0        0        0     3600 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/cat.py
--rw-r--r--   0        0        0     5080 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/cli.py
--rw-r--r--   0        0        0      611 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/compress.py
--rw-r--r--   0        0        0      846 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/extract_images.py
--rw-r--r--   0        0        0     6276 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/metadata.py
--rw-r--r--   0        0        0     2416 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/pagemeta.py
--rw-r--r--   0        0        0      726 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/up2.py
--rw-r--r--   0        0        0     1400 2024-03-29 08:15:04.114267 pdfly-0.3.1/pdfly/x2pdf.py
--rw-r--r--   0        0        0     5627 2024-03-29 08:15:04.114267 pdfly-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       89 2024-03-29 08:15:04.118267 pdfly-0.3.1/requirements/ci.in
--rw-r--r--   0        0        0     1463 2024-03-29 08:15:04.118267 pdfly-0.3.1/requirements/ci.txt
--rw-r--r--   0        0        0      107 2024-03-29 08:15:04.118267 pdfly-0.3.1/requirements/dev.in
--rw-r--r--   0        0        0     3425 2024-03-29 08:15:04.118267 pdfly-0.3.1/requirements/dev.txt
--rw-r--r--   0        0        0      112 2024-03-29 08:15:04.118267 pdfly-0.3.1/requirements/docs.in
--rw-r--r--   0        0        0     1644 2024-03-29 08:15:04.118267 pdfly-0.3.1/requirements/docs.txt
--rw-r--r--   0        0        0   360285 2024-03-29 08:15:04.118267 pdfly-0.3.1/resources/GeoBase_NHNC1_Data_Model_UML_EN.pdf
--rw-r--r--   0        0        0    97097 2024-03-29 08:15:04.118267 pdfly-0.3.1/resources/baleines.jpg
--rw-r--r--   0        0        0     5395 2024-03-29 08:15:04.118267 pdfly-0.3.1/resources/box.pdf
--rw-r--r--   0        0        0   100898 2024-03-29 08:15:04.118267 pdfly-0.3.1/resources/jpeg.pdf
--rw-r--r--   0        0        0   920238 2024-03-29 08:15:04.122267 pdfly-0.3.1/resources/pythonknight.png
-drwxr-xr-x   0        0        0        0 2024-03-29 08:15:04.122267 pdfly-0.3.1/sample-files/
--rw-r--r--   0        0        0      519 2024-03-29 08:15:04.122267 pdfly-0.3.1/setup.cfg
--rw-r--r--   0        0        0      463 2024-03-29 08:15:04.122267 pdfly-0.3.1/setup.py
--rw-r--r--   0        0        0       23 2024-03-29 08:15:04.122267 pdfly-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2021 2024-03-29 08:15:04.122267 pdfly-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     6254 2024-03-29 08:15:04.122267 pdfly-0.3.1/tests/test_cat.py
--rw-r--r--   0        0        0      661 2024-03-29 08:15:04.122267 pdfly-0.3.1/tests/test_cli.py
--rw-r--r--   0        0        0      774 2024-03-29 08:15:04.122267 pdfly-0.3.1/tests/test_extract_images.py
--rw-r--r--   0        0        0      626 2024-03-29 08:15:04.122267 pdfly-0.3.1/tests/test_x2pdf.py
--rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 pdfly-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      160 2024-04-14 17:37:54.509092 pdfly-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1149 2024-04-14 17:37:54.509092 pdfly-0.3.2/.github/workflows/create-github-release.yaml
+-rw-r--r--   0        0        0     2591 2024-04-14 17:37:54.509092 pdfly-0.3.2/.github/workflows/github-ci.yaml
+-rw-r--r--   0        0        0      707 2024-04-14 17:37:54.509092 pdfly-0.3.2/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0        0        0     1703 2024-04-14 17:37:54.509092 pdfly-0.3.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1987 2024-04-14 17:37:54.509092 pdfly-0.3.2/.gitignore
+-rw-r--r--   0        0        0       94 2024-04-14 17:37:54.509092 pdfly-0.3.2/.gitmodules
+-rw-r--r--   0        0        0      168 2024-04-14 17:37:54.509092 pdfly-0.3.2/.isort.cfg
+-rw-r--r--   0        0        0     1463 2024-04-14 17:37:54.509092 pdfly-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      542 2024-04-14 17:37:54.509092 pdfly-0.3.2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1858 2024-04-14 17:37:54.509092 pdfly-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1670 2024-04-14 17:37:54.509092 pdfly-0.3.2/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1514 2024-04-14 17:37:54.509092 pdfly-0.3.2/LICENSE
+-rw-r--r--   0        0        0      744 2024-04-14 17:37:54.509092 pdfly-0.3.2/Makefile
+-rw-r--r--   0        0        0     4262 2024-04-14 17:37:54.509092 pdfly-0.3.2/README.md
+-rw-r--r--   0        0        0      634 2024-04-14 17:37:54.509092 pdfly-0.3.2/docs/Makefile
+-rw-r--r--   0        0        0     4160 2024-04-14 17:37:54.509092 pdfly-0.3.2/docs/conf.py
+-rw-r--r--   0        0        0      704 2024-04-14 17:37:54.509092 pdfly-0.3.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-14 17:37:54.509092 pdfly-0.3.2/docs/make.bat
+-rw-r--r--   0        0        0     6520 2024-04-14 17:37:54.509092 pdfly-0.3.2/docs/meta/project-governance.md
+-rw-r--r--   0        0        0     1272 2024-04-14 17:37:54.513092 pdfly-0.3.2/docs/user/installation.md
+-rw-r--r--   0        0        0     3493 2024-04-14 17:37:54.513092 pdfly-0.3.2/docs/user/subcommand-cat.md
+-rw-r--r--   0        0        0     5673 2024-04-14 17:37:54.513092 pdfly-0.3.2/docs/user/subcommand-meta.md
+-rw-r--r--   0        0        0     2024 2024-04-14 17:37:54.513092 pdfly-0.3.2/docs/user/subcommand-x2pdf.md
+-rw-r--r--   0        0        0    10213 2024-04-14 17:37:54.513092 pdfly-0.3.2/make_release.py
+-rw-r--r--   0        0        0       31 2024-04-14 17:37:54.513092 pdfly-0.3.2/mypy.ini
+-rw-r--r--   0        0        0      164 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/__main__.py
+-rw-r--r--   0        0        0       87 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/_utils.py
+-rw-r--r--   0        0        0       22 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/_version.py
+-rw-r--r--   0        0        0     3600 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/cat.py
+-rw-r--r--   0        0        0     5080 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/cli.py
+-rw-r--r--   0        0        0      611 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/compress.py
+-rw-r--r--   0        0        0      846 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/extract_images.py
+-rw-r--r--   0        0        0     6276 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/metadata.py
+-rw-r--r--   0        0        0     2416 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/pagemeta.py
+-rw-r--r--   0        0        0      726 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/up2.py
+-rw-r--r--   0        0        0     1400 2024-04-14 17:37:54.513092 pdfly-0.3.2/pdfly/x2pdf.py
+-rw-r--r--   0        0        0     5627 2024-04-14 17:37:54.513092 pdfly-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-04-14 17:37:54.513092 pdfly-0.3.2/requirements/ci.in
+-rw-r--r--   0        0        0     1463 2024-04-14 17:37:54.513092 pdfly-0.3.2/requirements/ci.txt
+-rw-r--r--   0        0        0      107 2024-04-14 17:37:54.513092 pdfly-0.3.2/requirements/dev.in
+-rw-r--r--   0        0        0     3425 2024-04-14 17:37:54.513092 pdfly-0.3.2/requirements/dev.txt
+-rw-r--r--   0        0        0      112 2024-04-14 17:37:54.513092 pdfly-0.3.2/requirements/docs.in
+-rw-r--r--   0        0        0     1644 2024-04-14 17:37:54.513092 pdfly-0.3.2/requirements/docs.txt
+-rw-r--r--   0        0        0   360285 2024-04-14 17:37:54.513092 pdfly-0.3.2/resources/GeoBase_NHNC1_Data_Model_UML_EN.pdf
+-rw-r--r--   0        0        0    97097 2024-04-14 17:37:54.513092 pdfly-0.3.2/resources/baleines.jpg
+-rw-r--r--   0        0        0     5395 2024-04-14 17:37:54.513092 pdfly-0.3.2/resources/box.pdf
+-rw-r--r--   0        0        0   100898 2024-04-14 17:37:54.517092 pdfly-0.3.2/resources/jpeg.pdf
+-rw-r--r--   0        0        0   920238 2024-04-14 17:37:54.517092 pdfly-0.3.2/resources/pythonknight.png
+drwxr-xr-x   0        0        0        0 2024-04-14 17:37:54.517092 pdfly-0.3.2/sample-files/
+-rw-r--r--   0        0        0      519 2024-04-14 17:37:54.517092 pdfly-0.3.2/setup.cfg
+-rw-r--r--   0        0        0      463 2024-04-14 17:37:54.517092 pdfly-0.3.2/setup.py
+-rw-r--r--   0        0        0       23 2024-04-14 17:37:54.517092 pdfly-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-14 17:37:54.517092 pdfly-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     6254 2024-04-14 17:37:54.517092 pdfly-0.3.2/tests/test_cat.py
+-rw-r--r--   0        0        0      661 2024-04-14 17:37:54.517092 pdfly-0.3.2/tests/test_cli.py
+-rw-r--r--   0        0        0      774 2024-04-14 17:37:54.517092 pdfly-0.3.2/tests/test_extract_images.py
+-rw-r--r--   0        0        0      626 2024-04-14 17:37:54.517092 pdfly-0.3.2/tests/test_x2pdf.py
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 pdfly-0.3.2/PKG-INFO
```

### Comparing `pdfly-0.3.1/.github/workflows/github-ci.yaml` & `pdfly-0.3.2/.github/workflows/github-ci.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/.github/workflows/release.yaml` & `pdfly-0.3.2/.github/workflows/release.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # This action assumes that there is a REL-commit which already has a
 # Markdown-formatted git tag. Hence the CHANGELOG is already adjusted
 # and it's decided what should be in the release.
 # This action only ensures the release is done with the proper contents
 # and that it's announced with a Github release.
-name: Publish Python Package to PyPI
+name: Create git tag
 on:
   push:
     branches:
       - main
 
 permissions:
   contents: write
 
 jobs:
   build_and_publish:
     name: Publish a new version
     runs-on: ubuntu-latest
     if: "${{ startsWith(github.event.head_commit.message, 'REL: ') }}"
     steps:
-      # Ensure it's on PyPI
       - name: Checkout Repository
         uses: actions/checkout@v4
 
       - name: Extract version from commit message
         id: extract_version
         run: |
           VERSION=$(echo "${{ github.event.head_commit.message }}" | grep -oP '(?<=REL: )\d+\.\d+\.\d+')
@@ -42,45 +41,7 @@
         run: |
           VERSION="${{ steps.extract_version.outputs.version }}"
           MESSAGE="${{ steps.extract_message.outputs.message }}"
           git config user.name github-actions
           git config user.email github-actions@github.com
           git tag "$VERSION" -m "$MESSAGE"
           git push origin $VERSION
-
-      - name: Set up Python
-        uses: actions/setup-python@v5
-        with:
-          python-version: 3.x
-
-      - name: Install Flit
-        run: |
-          python -m pip install --upgrade pip
-          pip install flit
-
-      - name: Publish Package to PyPI🚀
-        env:
-          FLIT_USERNAME: '__token__'
-          FLIT_PASSWORD: ${{ secrets.FLIT_PASSWORD }}
-        run: |
-          flit publish
-
-      # Create the Github Page
-      - name: Prepare variables
-        id: prepare_variables
-        run: |
-          git fetch --tags --force
-          latest_tag=$(git describe --tags --abbrev=0)
-          echo "latest_tag=$(git describe --tags --abbrev=0)" >> "$GITHUB_ENV"
-          echo "date=$(date +'%Y-%m-%d')" >> "$GITHUB_ENV"
-          EOF=$(dd if=/dev/urandom bs=15 count=1 status=none | base64)
-          echo "tag_body<<$EOF" >> "$GITHUB_ENV"
-          git --no-pager tag -l "${latest_tag}" --format='%(contents:body)' >> "$GITHUB_ENV"
-          echo "$EOF" >> "$GITHUB_ENV"
-      - name: Create GitHub Release 🚀
-        uses: softprops/action-gh-release@v1
-        with:
-          tag_name: ${{ env.latest_tag }}
-          name: Version ${{ env.latest_tag }}, ${{ env.date }}
-          draft: false
-          prerelease: false
-          body: ${{ env.tag_body }}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pdfly-0.3.1/.gitignore` & `pdfly-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/.pre-commit-config.yaml` & `pdfly-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/.readthedocs.yaml` & `pdfly-0.3.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/CHANGELOG.md` & `pdfly-0.3.2/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG
 
+## Version 0.3.2, 2024-04-14
+
+### Developer Experience (DEV)
+-  Decouple git tag / PyPI release / Github release page (#49, #50)
+
+
+[Full Changelog](https://github.com/py-pdf/pdfly/compare/0.3.1...0.3.2)
+
 ## Version 0.3.1, 2024-03-29
 
 ### Maintenance (MAINT)
 -  Update pypdf usage (#48)
 
 ### Developer Experience (DEV)
 -  Release via REL commit (#48)
```

### Comparing `pdfly-0.3.1/CONTRIBUTORS.md` & `pdfly-0.3.2/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/LICENSE` & `pdfly-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/Makefile` & `pdfly-0.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/README.md` & `pdfly-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/Makefile` & `pdfly-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/conf.py` & `pdfly-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/index.rst` & `pdfly-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/make.bat` & `pdfly-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/meta/project-governance.md` & `pdfly-0.3.2/docs/meta/project-governance.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/user/installation.md` & `pdfly-0.3.2/docs/user/installation.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/user/subcommand-cat.md` & `pdfly-0.3.2/docs/user/subcommand-cat.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/user/subcommand-meta.md` & `pdfly-0.3.2/docs/user/subcommand-meta.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/docs/user/subcommand-x2pdf.md` & `pdfly-0.3.2/docs/user/subcommand-x2pdf.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/make_release.py` & `pdfly-0.3.2/make_release.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/cat.py` & `pdfly-0.3.2/pdfly/cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/cli.py` & `pdfly-0.3.2/pdfly/cli.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/compress.py` & `pdfly-0.3.2/pdfly/compress.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/extract_images.py` & `pdfly-0.3.2/pdfly/extract_images.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/metadata.py` & `pdfly-0.3.2/pdfly/metadata.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/pagemeta.py` & `pdfly-0.3.2/pdfly/pagemeta.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/up2.py` & `pdfly-0.3.2/pdfly/up2.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pdfly/x2pdf.py` & `pdfly-0.3.2/pdfly/x2pdf.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/pyproject.toml` & `pdfly-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/requirements/ci.txt` & `pdfly-0.3.2/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/requirements/dev.txt` & `pdfly-0.3.2/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/requirements/docs.txt` & `pdfly-0.3.2/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/resources/GeoBase_NHNC1_Data_Model_UML_EN.pdf` & `pdfly-0.3.2/resources/GeoBase_NHNC1_Data_Model_UML_EN.pdf`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/resources/baleines.jpg` & `pdfly-0.3.2/resources/baleines.jpg`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/resources/box.pdf` & `pdfly-0.3.2/resources/box.pdf`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/resources/jpeg.pdf` & `pdfly-0.3.2/resources/jpeg.pdf`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/resources/pythonknight.png` & `pdfly-0.3.2/resources/pythonknight.png`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/setup.cfg` & `pdfly-0.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/tests/conftest.py` & `pdfly-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/tests/test_cat.py` & `pdfly-0.3.2/tests/test_cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/tests/test_cli.py` & `pdfly-0.3.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/tests/test_extract_images.py` & `pdfly-0.3.2/tests/test_extract_images.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/tests/test_x2pdf.py` & `pdfly-0.3.2/tests/test_x2pdf.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.3.1/PKG-INFO` & `pdfly-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.3.1
+Version: 0.3.2
 Summary: A pure-python CLI application to manipulate PDF files
 Author-email: Martin Thoma <info@martin-thoma.de>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

