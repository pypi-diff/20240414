# Comparing `tmp/ferramentas-basicas-pln-0.9.9.7.tar.gz` & `tmp/ferramentas-basicas-pln-0.9.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferramentas-basicas-pln-0.9.9.7.tar", last modified: Sun Apr  7 23:49:07 2024, max compression
+gzip compressed data, was "ferramentas-basicas-pln-0.9.9.8.tar", last modified: Sun Apr 14 19:03:45 2024, max compression
```

## Comparing `ferramentas-basicas-pln-0.9.9.7.tar` & `ferramentas-basicas-pln-0.9.9.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 23:49:07.755163 ferramentas-basicas-pln-0.9.9.7/
--rw-rw-rw-   0        0        0    13948 2024-04-07 23:49:07.755163 ferramentas-basicas-pln-0.9.9.7/PKG-INFO
--rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 23:49:07.749157 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln/
--rw-rw-rw-   0        0        0     1032 2024-04-07 02:06:59.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln/__init__.py
--rw-rw-rw-   0        0        0    43908 2024-04-07 23:48:52.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln/main.py
-drwxrwxrwx   0        0        0        0 2024-04-07 23:49:07.754162 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/
--rw-rw-rw-   0        0        0    13948 2024-04-07 23:49:07.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-07 23:49:07.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 23:49:07.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-07 23:49:07.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-07 23:49:07.000000 ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 23:49:07.755163 ferramentas-basicas-pln-0.9.9.7/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-04-07 23:48:57.000000 ferramentas-basicas-pln-0.9.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:03:45.952534 ferramentas-basicas-pln-0.9.9.8/
+-rw-rw-rw-   0        0        0    13948 2024-04-14 19:03:45.952534 ferramentas-basicas-pln-0.9.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 19:03:45.945526 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln/
+-rw-rw-rw-   0        0        0     1032 2024-04-07 02:06:59.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln/__init__.py
+-rw-rw-rw-   0        0        0    43909 2024-04-14 19:03:00.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln/main.py
+drwxrwxrwx   0        0        0        0 2024-04-14 19:03:45.951532 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/
+-rw-rw-rw-   0        0        0    13948 2024-04-14 19:03:45.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-14 19:03:45.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 19:03:45.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-14 19:03:45.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-14 19:03:45.000000 ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 19:03:45.953534 ferramentas-basicas-pln-0.9.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-04-14 19:03:38.000000 ferramentas-basicas-pln-0.9.9.8/setup.py
```

### Comparing `ferramentas-basicas-pln-0.9.9.7/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9.7
+Version: 0.9.9.8
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.7 Summary:
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.8 Summary:
 Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
 Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
```

### Comparing `ferramentas-basicas-pln-0.9.9.7/README.md` & `ferramentas-basicas-pln-0.9.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln/__init__.py` & `ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln/__init__.py`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln/main.py` & `ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unicodedata
 import re
 import string
 from typing import Generator
 
 STRING_CARACTERES_ESPECIAIS_PADRAO = string.punctuation
 
-CARACTERES_NORMAIS : str = string.printable + 'áàâãéèêíìîóòôõúùûüç' + 'áàâãéèêíìîóòôõúùûüç'.upper() + '\xa0' # + '\xa0' representa o "espaço em branco não quebrável" em hexadecimal
+CARACTERES_NORMAIS : str = string.printable + 'áàâãéèêíìîóòôõúùûüç' + 'áàâãéèêíìîóòôõúùûüç'.upper()
 
 LISTA_STOPWORDS_PADRAO_FREQUENCIA : list = ['a','à','as','às','ao','aos','da','das','na','nas','numa','numas',
                                             'o','os','ou','do','dos','no','nos',
                                             'de','e','é','ser','será','serão','são','está','estão','foi','em','num','nuns',
                                             'são','sem','mais','menos',
                                             'um','uma','uns','umas',
                                             'sua','suas','seu','seus',
@@ -138,14 +138,16 @@
     ### Parâmetros:
     - :parâmetro texto: String contendo o texto que você quer limpar.
 
     ### Retornos:
     - :retorno: String limpa dos caracteres "mais que especiais" (emojis, dígitos estranhos, 
     formas que não se encontram no teclado, etc).
     """
+    # lista_replace = ['\xa0','\x0b','\x0c']
+    texto = texto.replace('\xa0',' ')
     for caracter_estranho in [c for c in texto if c not in CARACTERES_NORMAIS]:
         texto = texto.replace(caracter_estranho,'')
     return texto
 
 def removerEspacosEmBrancoExtras(texto : str) -> str:
     """
     ### Objetivo
```

### Comparing `ferramentas-basicas-pln-0.9.9.7/ferramentas_basicas_pln.egg-info/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.8/ferramentas_basicas_pln.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9.7
+Version: 0.9.9.8
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.7 Summary:
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.8 Summary:
 Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
 Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
```

### Comparing `ferramentas-basicas-pln-0.9.9.7/setup.py` & `ferramentas-basicas-pln-0.9.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open(r'README.md','r',encoding='utf-8') as f:
     descricao_longa = f.read()
 
 setup(
     name='ferramentas-basicas-pln',
-    version='0.9.9.7',
+    version='0.9.9.8',
     packages=find_packages(),
     install_requires = ['regex'],
     description='Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.',
     long_description=descricao_longa,
     long_description_content_type="text/markdown",
     author='Igor Caetano de Souza',
     project_urls={
```

