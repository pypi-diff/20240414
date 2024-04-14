# Comparing `tmp/econdata-1.0.7.tar.gz` & `tmp/econdata-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econdata-1.0.7.tar", last modified: Tue Oct 17 20:08:40 2023, max compression
+gzip compressed data, was "econdata-1.0.9.tar", last modified: Sun Oct 22 21:58:22 2023, max compression
```

## Comparing `econdata-1.0.7.tar` & `econdata-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-10-17 20:08:40.580895 econdata-1.0.7/
--rw-rw-rw-   0        0        0     7621 2023-10-17 20:08:40.580895 econdata-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7033 2023-10-17 19:15:26.000000 econdata-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-10-17 20:08:40.581892 econdata-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      908 2023-10-17 19:16:45.000000 econdata-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-17 20:08:40.566107 econdata-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-10-17 20:08:40.575067 econdata-1.0.7/src/econdata/
--rw-rw-rw-   0        0        0     6390 2023-10-17 17:26:14.000000 econdata-1.0.7/src/econdata/BCRP.py
--rw-rw-rw-   0        0        0     4034 2023-10-17 17:26:14.000000 econdata-1.0.7/src/econdata/FRED.py
--rw-rw-rw-   0        0        0     4272 2023-10-17 17:26:14.000000 econdata-1.0.7/src/econdata/IMF.py
--rw-rw-rw-   0        0        0     2154 2023-10-17 17:26:14.000000 econdata-1.0.7/src/econdata/OECD.py
--rw-rw-rw-   0        0        0     2853 2023-10-17 18:43:39.000000 econdata-1.0.7/src/econdata/WB.py
--rw-rw-rw-   0        0        0     3717 2023-10-17 18:59:41.000000 econdata-1.0.7/src/econdata/YFinance.py
--rw-rw-rw-   0        0        0        0 2023-10-17 17:26:14.000000 econdata-1.0.7/src/econdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-17 20:08:40.578899 econdata-1.0.7/src/econdata.egg-info/
--rw-rw-rw-   0        0        0     7621 2023-10-17 20:08:40.000000 econdata-1.0.7/src/econdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2023-10-17 20:08:40.000000 econdata-1.0.7/src/econdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-17 20:08:40.000000 econdata-1.0.7/src/econdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-10-17 20:08:40.000000 econdata-1.0.7/src/econdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-10-17 20:08:40.000000 econdata-1.0.7/src/econdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-22 21:58:22.802850 econdata-1.0.9/
+-rw-rw-rw-   0        0        0     8679 2023-10-22 21:58:22.801852 econdata-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8060 2023-10-22 21:56:54.000000 econdata-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-10-22 21:58:22.802850 econdata-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-10-22 21:57:43.000000 econdata-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-22 21:58:22.787459 econdata-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-10-22 21:58:22.796088 econdata-1.0.9/src/econdata/
+-rw-rw-rw-   0        0        0     6477 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/BCRP.py
+-rw-rw-rw-   0        0        0     4034 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/FRED.py
+-rw-rw-rw-   0        0        0     4294 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/IMF.py
+-rw-rw-rw-   0        0        0     2154 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/OECD.py
+-rw-rw-rw-   0        0        0     4014 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/WB.py
+-rw-rw-rw-   0        0        0     3717 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/YFinance.py
+-rw-rw-rw-   0        0        0        0 2023-10-22 21:55:03.000000 econdata-1.0.9/src/econdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-22 21:58:22.800855 econdata-1.0.9/src/econdata.egg-info/
+-rw-rw-rw-   0        0        0     8679 2023-10-22 21:58:22.000000 econdata-1.0.9/src/econdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2023-10-22 21:58:22.000000 econdata-1.0.9/src/econdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-22 21:58:22.000000 econdata-1.0.9/src/econdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-10-22 21:58:22.000000 econdata-1.0.9/src/econdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-10-22 21:58:22.000000 econdata-1.0.9/src/econdata.egg-info/top_level.txt
```

### Comparing `econdata-1.0.7/PKG-INFO` & `econdata-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.7
+Version: 1.0.9
 Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: yfinance
 Requires-Dist: requests
 Requires-Dist: warn
+Requires-Dist: more-itertools
 
 # Econdata
 **Econdata** es una librería para la extracción de series de tiempo de las principales instituciones económicas para el Perú. En la versión actual se cuenta con las siguientes instituciones:
 1. Banco Central de Reserva del Perú (BCRP)
 2. Banco Mundial (WB) 
 3. Federal Reserve Economic Data (FRED)
 4. Fondo Monetario Internacional (IMF)
 5. Organización para la Cooperación y el Desarrollo Económicos (OECD)
 6. Yahoo! Finance (YFinance)
 
 
 El anuncio fue realizado en LinkedIn, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
+## Tabla de contenido
+- [Instalación](#instalación)
+- [Métodos](#métodos)
+- [Getting started](#getting-started)
+    - [Ejemplo: Extracción de datos del BCRP](#ejemplo-extracción-de-datos-del-bcrp)
+    - [Ejemplo: Extracción de datos de Banco Mundial](#ejemplo-extracción-de-datos-de-banco-mundial)
+    - [Ejemplo: Extracción de datos de Yahoo! Finance](#ejemplo-extracción-de-datos-de-yahoo-finance)
+- [Contenido adicional](#contenido-adicional)
+- [Créditos](#créditos)
+
 
 ## Instalación
 Para instalar la versión más reciente de econdata desde [PyPI](https://pypi.org/project/econdata/):
 ```python
 pip install econdata
 ```
 
 La librería requiere de las siguientes dependencias:
 * pandas
 * numpy
 * yfinance
 * requests
-* warn
+* warnings
+* itertools
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```text
 get_data()
 ```
@@ -119,60 +131,63 @@
 
 WB.search(
     consulta=['gdp', 'per', 'capita']
 )
 ```
 
 ```text
+                                                               title
 id                                                                  
 NY.GDP.PCAP.CD                          GDP per capita (current US$)
 NY.GDP.PCAP.CN                          GDP per capita (current LCU)
 NY.GDP.PCAP.KD                    GDP per capita (constant 2015 US$)
 NY.GDP.PCAP.KD.ZG                   GDP per capita growth (annual %)
 NY.GDP.PCAP.KN                         GDP per capita (constant LCU)
 NY.GDP.PCAP.PP.CD      GDP per capita, PPP (current international $)
 NY.GDP.PCAP.PP.KD  GDP per capita, PPP (constant 2017 internation...
 PA.NUS.PPP         PPP can be used to convert national accounts d...
-PA.NUS.PRVT.PP     PPP can be used to convert national accounts d...
 SE.XPD.PRIM.PC.ZS  Government expenditure per student, primary (%...
 SE.XPD.SECO.PC.ZS  Government expenditure per student, secondary ...
 SE.XPD.TERT.PC.ZS  Government expenditure per student, tertiary (...
 ```
 
 Tras obtener el código de la serie (```NY.GDP.PCAP.PP.KD```), se puede solicitar la data para un rango de periodos:
 
 ```python
 df = WB.get_data(
-    {
+    countries = {
         'CO': 'Colombia',
         'CL': 'Chile',
         'PE': 'Perú'
     },
-    indicator = 'NY.GDP.PCAP.PP.KD',
+    indicators = {
+        'NY.GDP.PCAP.PP.KD': 'Real GDP per capita'
+    },
     fechaini = '2012',
     fechafin = '2022'
 )
 
 df
 ```
 
 ```text
-          Colombia         Chile          Perú
-time                                          
-2012  12934.965752  23467.978726  11084.873937
-2013  13465.075044  24011.591014  11620.644447
-2014  13938.231517  24197.183280  11773.944135
-2015  14215.688252  24464.745662  12015.187156
-2016  14358.168218  24599.374633  12321.318154
-2017  14334.914608  24546.912421  12442.746462
-2018  14426.434382  25071.990069  12696.236289
-2019  14616.135124  24809.860974  12735.168278
-2020  13358.298083  22970.550435  11187.343790
-2021  14661.213244  25412.752073  12533.841417
-2022  15651.582058  25886.121356  12743.942391
+                Colombia               Chile                Perú
+     Real GDP per capita Real GDP per capita Real GDP per capita
+time                                                            
+2012        12934.965752        23467.978726        11084.873937
+2013        13465.075044        24011.591014        11620.644447
+2014        13938.231517        24197.183280        11773.944135
+2015        14215.688252        24464.745662        12015.187156
+2016        14358.168218        24599.374633        12321.318154
+2017        14334.914608        24546.912421        12442.746462
+2018        14426.434382        25071.990069        12696.236289
+2019        14616.135124        24809.860974        12735.168278
+2020        13358.298083        22970.550435        11187.343790
+2021        14661.213244        25412.752073        12533.841417
+2022        15651.582058        25886.121356        12743.942391
 ```
 
 
 ### Ejemplo: Extracción de datos de Yahoo! Finance
 Iniciaremos con la consulta de la cotización de _Apple_ y _Microsoft_:
 
 ```python
@@ -227,14 +242,15 @@
 ```
 
 
 ## Contenido adicional
 Para más información revisar los siguientes links:
 * Más códigos de _test_ están disponibles [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
 * El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
-* Revisar un proyecto de la creación de un dashboard de indicadores peruanos elaborado con la librería, disponible [aquí](https://github.com/mauricioalvaradoo/indicators).
+* Proyecto: creación de modelo de Nowcasting de forecast del PBI real peruano, disponible [aquí](https://github.com/mauricioalvaradoo/nowcasting).
+* Proyecto: creación de un dashboard de indicadores peruanos elaborado con la librería, disponible [aquí](https://github.com/mauricioalvaradoo/indicators).
 
 
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo). email: mauricio.alvarado@pucp.edu.pe
-* [Andrei Romero](https://github.com/Ixtalia)
+* [Andrei Romero](https://github.com/noanroes). email: noandroes@gmail.com
```

### Comparing `econdata-1.0.7/README.md` & `econdata-1.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -6,27 +6,38 @@
 4. Fondo Monetario Internacional (IMF)
 5. Organización para la Cooperación y el Desarrollo Económicos (OECD)
 6. Yahoo! Finance (YFinance)
 
 
 El anuncio fue realizado en LinkedIn, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
+## Tabla de contenido
+- [Instalación](#instalación)
+- [Métodos](#métodos)
+- [Getting started](#getting-started)
+    - [Ejemplo: Extracción de datos del BCRP](#ejemplo-extracción-de-datos-del-bcrp)
+    - [Ejemplo: Extracción de datos de Banco Mundial](#ejemplo-extracción-de-datos-de-banco-mundial)
+    - [Ejemplo: Extracción de datos de Yahoo! Finance](#ejemplo-extracción-de-datos-de-yahoo-finance)
+- [Contenido adicional](#contenido-adicional)
+- [Créditos](#créditos)
+
 
 ## Instalación
 Para instalar la versión más reciente de econdata desde [PyPI](https://pypi.org/project/econdata/):
 ```python
 pip install econdata
 ```
 
 La librería requiere de las siguientes dependencias:
 * pandas
 * numpy
 * yfinance
 * requests
-* warn
+* warnings
+* itertools
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```text
 get_data()
 ```
@@ -102,60 +113,63 @@
 
 WB.search(
     consulta=['gdp', 'per', 'capita']
 )
 ```
 
 ```text
+                                                               title
 id                                                                  
 NY.GDP.PCAP.CD                          GDP per capita (current US$)
 NY.GDP.PCAP.CN                          GDP per capita (current LCU)
 NY.GDP.PCAP.KD                    GDP per capita (constant 2015 US$)
 NY.GDP.PCAP.KD.ZG                   GDP per capita growth (annual %)
 NY.GDP.PCAP.KN                         GDP per capita (constant LCU)
 NY.GDP.PCAP.PP.CD      GDP per capita, PPP (current international $)
 NY.GDP.PCAP.PP.KD  GDP per capita, PPP (constant 2017 internation...
 PA.NUS.PPP         PPP can be used to convert national accounts d...
-PA.NUS.PRVT.PP     PPP can be used to convert national accounts d...
 SE.XPD.PRIM.PC.ZS  Government expenditure per student, primary (%...
 SE.XPD.SECO.PC.ZS  Government expenditure per student, secondary ...
 SE.XPD.TERT.PC.ZS  Government expenditure per student, tertiary (...
 ```
 
 Tras obtener el código de la serie (```NY.GDP.PCAP.PP.KD```), se puede solicitar la data para un rango de periodos:
 
 ```python
 df = WB.get_data(
-    {
+    countries = {
         'CO': 'Colombia',
         'CL': 'Chile',
         'PE': 'Perú'
     },
-    indicator = 'NY.GDP.PCAP.PP.KD',
+    indicators = {
+        'NY.GDP.PCAP.PP.KD': 'Real GDP per capita'
+    },
     fechaini = '2012',
     fechafin = '2022'
 )
 
 df
 ```
 
 ```text
-          Colombia         Chile          Perú
-time                                          
-2012  12934.965752  23467.978726  11084.873937
-2013  13465.075044  24011.591014  11620.644447
-2014  13938.231517  24197.183280  11773.944135
-2015  14215.688252  24464.745662  12015.187156
-2016  14358.168218  24599.374633  12321.318154
-2017  14334.914608  24546.912421  12442.746462
-2018  14426.434382  25071.990069  12696.236289
-2019  14616.135124  24809.860974  12735.168278
-2020  13358.298083  22970.550435  11187.343790
-2021  14661.213244  25412.752073  12533.841417
-2022  15651.582058  25886.121356  12743.942391
+                Colombia               Chile                Perú
+     Real GDP per capita Real GDP per capita Real GDP per capita
+time                                                            
+2012        12934.965752        23467.978726        11084.873937
+2013        13465.075044        24011.591014        11620.644447
+2014        13938.231517        24197.183280        11773.944135
+2015        14215.688252        24464.745662        12015.187156
+2016        14358.168218        24599.374633        12321.318154
+2017        14334.914608        24546.912421        12442.746462
+2018        14426.434382        25071.990069        12696.236289
+2019        14616.135124        24809.860974        12735.168278
+2020        13358.298083        22970.550435        11187.343790
+2021        14661.213244        25412.752073        12533.841417
+2022        15651.582058        25886.121356        12743.942391
 ```
 
 
 ### Ejemplo: Extracción de datos de Yahoo! Finance
 Iniciaremos con la consulta de la cotización de _Apple_ y _Microsoft_:
 
 ```python
@@ -210,14 +224,15 @@
 ```
 
 
 ## Contenido adicional
 Para más información revisar los siguientes links:
 * Más códigos de _test_ están disponibles [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
 * El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
-* Revisar un proyecto de la creación de un dashboard de indicadores peruanos elaborado con la librería, disponible [aquí](https://github.com/mauricioalvaradoo/indicators).
+* Proyecto: creación de modelo de Nowcasting de forecast del PBI real peruano, disponible [aquí](https://github.com/mauricioalvaradoo/nowcasting).
+* Proyecto: creación de un dashboard de indicadores peruanos elaborado con la librería, disponible [aquí](https://github.com/mauricioalvaradoo/indicators).
 
 
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo). email: mauricio.alvarado@pucp.edu.pe
-* [Andrei Romero](https://github.com/Ixtalia)
+* [Andrei Romero](https://github.com/noanroes). email: noandroes@gmail.com
```

### Comparing `econdata-1.0.7/setup.py` & `econdata-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='econdata',
-    version = '1.0.7',
+    version = '1.0.9',
     author = 'Mauricio Alvarado, Andrei Romero',
     description = 'Extracción de series de tiempo de las principales instituciones económicas para el Perú',
     long_description = long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/mauricioalvaradoo/econdata',
     classifiers = [
         'Programming Language :: Python :: 3',
@@ -20,12 +20,11 @@
     # packages=setuptools.find_packages(),
     python_requires='>=3.6',
     install_requires = [
         'pandas',
         'numpy',
         'yfinance',
         'requests',
-        'warn'
+        'warn',
+        'more-itertools'
     ]
-)
-
-
+)
```

### Comparing `econdata-1.0.7/src/econdata/BCRP.py` & `econdata-1.0.9/src/econdata/BCRP.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     ''' Importar multiples series de la API del BCRP.
     Considerar que las series deben ser de la misma frecuencia.
     
     Parámetros
     ----------
     series: dict
         Diccionario de los códigos y nombres de las series.
-    fechaini: datetime
+    fechaini: str
         Fecha de inicio de la serie.
-    fechafin: datetime
+    fechafin: str
         Fecha de fin de la serie.
         
     Retorno
     ----------
     df: pd.DataFrame
         Series consultadas.
     
@@ -109,14 +109,17 @@
                     df.index = pd.period_range(newanio+fechaini[4:], fechafin, freq='Q')
                 except:  
                     try: # Aumentando un año para series en var. % y hasta fechafin Q4 
                         newanio = str( int(fechaini[:4])+1 )
                         df.index = pd.period_range(newanio+fechaini[4:], fechafin[:4]+'Q4', freq='Q')
                     except:
                         pass
+    if keys[0][-1] == 'A':
+        df.index = pd.to_datetime(df.index, format='%Y').year
+    
     
     df.sort_index(inplace=True) # Ordenamiento de fechas
 
     return df
```

### Comparing `econdata-1.0.7/src/econdata/FRED.py` & `econdata-1.0.9/src/econdata/FRED.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.7/src/econdata/IMF.py` & `econdata-1.0.9/src/econdata/IMF.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     '''
     
     base = 'https://www.imf.org/external/datamapper/api/v1/'
     
     # Filtros
     filters = '/'.join(countries.keys()) if countries is not None else None
     dates = [str(y) for y in range(int(fechaini), int(fechafin)+1)] if fechaini is not None and fechafin is not None else None
-    dates = [str(y) for y in range(int(fechaini), 2029)] if fechaini is not None and fechafin is None else dates
-    dates = [str(y) for y in range(1980, int(fechafin)+1)] if fechaini is None and fechafin is not None else dates
+    dates = [str(y) for y in range(int(fechaini), 2029)]            if fechaini is not None and fechafin is     None else dates
+    dates = [str(y) for y in range(1980, int(fechafin)+1)]          if fechaini is     None and fechafin is not None else dates
     dates = ','.join(dates) if dates is not None else None
     
     url = f'{base}{indicator}'
     
     if filters:
         url += f'/{filters}'      
     if dates:
@@ -145,10 +145,8 @@
             pass
     
         df.set_index('Código', inplace=True)
     
         return df     
         
     except:
-        return print('Revisa bien el tipo!')
-
-
+        return print('Revisa bien el tipo!')
```

### Comparing `econdata-1.0.7/src/econdata/OECD.py` & `econdata-1.0.9/src/econdata/OECD.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.7/src/econdata/YFinance.py` & `econdata-1.0.9/src/econdata/YFinance.py`

 * *Files identical despite different names*

### Comparing `econdata-1.0.7/src/econdata.egg-info/PKG-INFO` & `econdata-1.0.9/src/econdata.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,61 @@
 Metadata-Version: 2.1
 Name: econdata
-Version: 1.0.7
+Version: 1.0.9
 Summary: Extracción de series de tiempo de las principales instituciones económicas para el Perú
 Home-page: https://github.com/mauricioalvaradoo/econdata
 Author: Mauricio Alvarado, Andrei Romero
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: yfinance
 Requires-Dist: requests
 Requires-Dist: warn
+Requires-Dist: more-itertools
 
 # Econdata
 **Econdata** es una librería para la extracción de series de tiempo de las principales instituciones económicas para el Perú. En la versión actual se cuenta con las siguientes instituciones:
 1. Banco Central de Reserva del Perú (BCRP)
 2. Banco Mundial (WB) 
 3. Federal Reserve Economic Data (FRED)
 4. Fondo Monetario Internacional (IMF)
 5. Organización para la Cooperación y el Desarrollo Económicos (OECD)
 6. Yahoo! Finance (YFinance)
 
 
 El anuncio fue realizado en LinkedIn, y está disponible [aquí](https://www.linkedin.com/posts/mauricioalvaradoo_github-mauricioalvaradooecondata-extracci%C3%B3n-activity-7053798889950179328-wl5w?utm_source=share&utm_medium=member_desktop). 
 
+## Tabla de contenido
+- [Instalación](#instalación)
+- [Métodos](#métodos)
+- [Getting started](#getting-started)
+    - [Ejemplo: Extracción de datos del BCRP](#ejemplo-extracción-de-datos-del-bcrp)
+    - [Ejemplo: Extracción de datos de Banco Mundial](#ejemplo-extracción-de-datos-de-banco-mundial)
+    - [Ejemplo: Extracción de datos de Yahoo! Finance](#ejemplo-extracción-de-datos-de-yahoo-finance)
+- [Contenido adicional](#contenido-adicional)
+- [Créditos](#créditos)
+
 
 ## Instalación
 Para instalar la versión más reciente de econdata desde [PyPI](https://pypi.org/project/econdata/):
 ```python
 pip install econdata
 ```
 
 La librería requiere de las siguientes dependencias:
 * pandas
 * numpy
 * yfinance
 * requests
-* warn
+* warnings
+* itertools
 
 
 ## Métodos
 Para cada institución se tiene dos métodos comunes. El primero sirve para extraer las series dado un rango de peridos:
 ```text
 get_data()
 ```
@@ -119,60 +131,63 @@
 
 WB.search(
     consulta=['gdp', 'per', 'capita']
 )
 ```
 
 ```text
+                                                               title
 id                                                                  
 NY.GDP.PCAP.CD                          GDP per capita (current US$)
 NY.GDP.PCAP.CN                          GDP per capita (current LCU)
 NY.GDP.PCAP.KD                    GDP per capita (constant 2015 US$)
 NY.GDP.PCAP.KD.ZG                   GDP per capita growth (annual %)
 NY.GDP.PCAP.KN                         GDP per capita (constant LCU)
 NY.GDP.PCAP.PP.CD      GDP per capita, PPP (current international $)
 NY.GDP.PCAP.PP.KD  GDP per capita, PPP (constant 2017 internation...
 PA.NUS.PPP         PPP can be used to convert national accounts d...
-PA.NUS.PRVT.PP     PPP can be used to convert national accounts d...
 SE.XPD.PRIM.PC.ZS  Government expenditure per student, primary (%...
 SE.XPD.SECO.PC.ZS  Government expenditure per student, secondary ...
 SE.XPD.TERT.PC.ZS  Government expenditure per student, tertiary (...
 ```
 
 Tras obtener el código de la serie (```NY.GDP.PCAP.PP.KD```), se puede solicitar la data para un rango de periodos:
 
 ```python
 df = WB.get_data(
-    {
+    countries = {
         'CO': 'Colombia',
         'CL': 'Chile',
         'PE': 'Perú'
     },
-    indicator = 'NY.GDP.PCAP.PP.KD',
+    indicators = {
+        'NY.GDP.PCAP.PP.KD': 'Real GDP per capita'
+    },
     fechaini = '2012',
     fechafin = '2022'
 )
 
 df
 ```
 
 ```text
-          Colombia         Chile          Perú
-time                                          
-2012  12934.965752  23467.978726  11084.873937
-2013  13465.075044  24011.591014  11620.644447
-2014  13938.231517  24197.183280  11773.944135
-2015  14215.688252  24464.745662  12015.187156
-2016  14358.168218  24599.374633  12321.318154
-2017  14334.914608  24546.912421  12442.746462
-2018  14426.434382  25071.990069  12696.236289
-2019  14616.135124  24809.860974  12735.168278
-2020  13358.298083  22970.550435  11187.343790
-2021  14661.213244  25412.752073  12533.841417
-2022  15651.582058  25886.121356  12743.942391
+                Colombia               Chile                Perú
+     Real GDP per capita Real GDP per capita Real GDP per capita
+time                                                            
+2012        12934.965752        23467.978726        11084.873937
+2013        13465.075044        24011.591014        11620.644447
+2014        13938.231517        24197.183280        11773.944135
+2015        14215.688252        24464.745662        12015.187156
+2016        14358.168218        24599.374633        12321.318154
+2017        14334.914608        24546.912421        12442.746462
+2018        14426.434382        25071.990069        12696.236289
+2019        14616.135124        24809.860974        12735.168278
+2020        13358.298083        22970.550435        11187.343790
+2021        14661.213244        25412.752073        12533.841417
+2022        15651.582058        25886.121356        12743.942391
 ```
 
 
 ### Ejemplo: Extracción de datos de Yahoo! Finance
 Iniciaremos con la consulta de la cotización de _Apple_ y _Microsoft_:
 
 ```python
@@ -227,14 +242,15 @@
 ```
 
 
 ## Contenido adicional
 Para más información revisar los siguientes links:
 * Más códigos de _test_ están disponibles [aquí](https://github.com/mauricioalvaradoo/econdata/blob/master/test.py).
 * El video del anuncio de la librería y la demo está disponible [aquí](https://www.youtube.com/watch?v=etaqHMDfvtE).
-* Revisar un proyecto de la creación de un dashboard de indicadores peruanos elaborado con la librería, disponible [aquí](https://github.com/mauricioalvaradoo/indicators).
+* Proyecto: creación de modelo de Nowcasting de forecast del PBI real peruano, disponible [aquí](https://github.com/mauricioalvaradoo/nowcasting).
+* Proyecto: creación de un dashboard de indicadores peruanos elaborado con la librería, disponible [aquí](https://github.com/mauricioalvaradoo/indicators).
 
 
 ## Créditos
 * [Mauricio Alvarado](https://github.com/mauricioalvaradoo). email: mauricio.alvarado@pucp.edu.pe
-* [Andrei Romero](https://github.com/Ixtalia)
+* [Andrei Romero](https://github.com/noanroes). email: noandroes@gmail.com
```

