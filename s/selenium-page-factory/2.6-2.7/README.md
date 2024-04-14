# Comparing `tmp/selenium-page-factory-2.6.tar.gz` & `tmp/selenium-page-factory-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\selenium-page-factory-2.6.tar", last modified: Sun Mar 19 05:30:39 2023, max compression
+gzip compressed data, was "dist\selenium-page-factory-2.7.tar", last modified: Sun Apr 14 06:20:19 2024, max compression
```

## Comparing `selenium-page-factory-2.6.tar` & `selenium-page-factory-2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 05:30:39.375200 selenium-page-factory-2.6/
--rw-rw-rw-   0        0        0     3985 2023-03-19 05:30:39.375200 selenium-page-factory-2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2703 2023-03-19 05:25:07.000000 selenium-page-factory-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-03-19 05:30:39.375200 selenium-page-factory-2.6/selenium_page_factory.egg-info/
--rw-rw-rw-   0        0        0     3985 2023-03-19 05:30:38.000000 selenium-page-factory-2.6/selenium_page_factory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-03-19 05:30:38.000000 selenium-page-factory-2.6/selenium_page_factory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 05:30:38.000000 selenium-page-factory-2.6/selenium_page_factory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-19 05:30:38.000000 selenium-page-factory-2.6/selenium_page_factory.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-03-19 05:30:38.000000 selenium-page-factory-2.6/selenium_page_factory.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-19 05:30:39.375200 selenium-page-factory-2.6/seleniumpagefactory/
--rw-rw-rw-   0        0        0    11664 2023-03-19 05:16:05.000000 selenium-page-factory-2.6/seleniumpagefactory/Pagefactory.py
--rw-rw-rw-   0        0        0     1249 2023-03-19 05:15:41.000000 selenium-page-factory-2.6/seleniumpagefactory/__init__.py
--rw-rw-rw-   0        0        0       42 2023-03-19 05:30:39.375200 selenium-page-factory-2.6/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-03-19 05:22:50.000000 selenium-page-factory-2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-19 05:30:39.375200 selenium-page-factory-2.6/tests/
--rw-rw-rw-   0        0        0       55 2019-09-05 09:44:12.000000 selenium-page-factory-2.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1215 2019-09-05 09:38:14.000000 selenium-page-factory-2.6/tests/selenium_unitest.py
--rw-rw-rw-   0        0        0     1997 2020-08-24 12:19:06.000000 selenium-page-factory-2.6/tests/test_selenium.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:20:19.811805 selenium-page-factory-2.7/
+-rw-rw-rw-   0        0        0     4155 2024-04-14 06:20:19.811805 selenium-page-factory-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-04-14 06:16:05.000000 selenium-page-factory-2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 06:20:19.796205 selenium-page-factory-2.7/selenium_page_factory.egg-info/
+-rw-rw-rw-   0        0        0     4155 2024-04-14 06:20:18.000000 selenium-page-factory-2.7/selenium_page_factory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-14 06:20:18.000000 selenium-page-factory-2.7/selenium_page_factory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 06:20:18.000000 selenium-page-factory-2.7/selenium_page_factory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 06:20:18.000000 selenium-page-factory-2.7/selenium_page_factory.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-14 06:20:18.000000 selenium-page-factory-2.7/selenium_page_factory.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 06:20:19.796205 selenium-page-factory-2.7/seleniumpagefactory/
+-rw-rw-rw-   0        0        0    12126 2024-04-14 06:18:15.000000 selenium-page-factory-2.7/seleniumpagefactory/Pagefactory.py
+-rw-rw-rw-   0        0        0     1249 2024-04-14 06:17:44.000000 selenium-page-factory-2.7/seleniumpagefactory/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-04-14 06:20:19.811805 selenium-page-factory-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      851 2024-04-14 05:44:15.000000 selenium-page-factory-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 06:20:19.811805 selenium-page-factory-2.7/tests/
+-rw-rw-rw-   0        0        0       55 2019-09-05 09:44:12.000000 selenium-page-factory-2.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1215 2019-09-05 09:38:14.000000 selenium-page-factory-2.7/tests/selenium_unitest.py
+-rw-rw-rw-   0        0        0     1997 2020-08-24 12:19:06.000000 selenium-page-factory-2.7/tests/test_selenium.py
```

### Comparing `selenium-page-factory-2.6/PKG-INFO` & `selenium-page-factory-2.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-page-factory
-Version: 2.6
+Version: 2.7
 Summary: Python library provides page factory approach to implement page object model in selenium
 Home-page: https://github.com/NayakwadiS/selenium-page-factory
 Author: Sujit Nayakwadi
 Author-email: nayakwadi_sujit@rediffmail.com
 License: MIT
 Description: A Page Factory is one way of implementing a Page Object Model. In order to support the Page Object pattern.
         As in Java we are using @findBy, here we are declaring all web element in dictionary.
@@ -14,14 +14,15 @@
         Main Features
         =============
         
         * Initialise all the webElements declared in Point at a time.
         * All WebElements methods are re-define to add extra features eg- click method extended to have explicit wait for element to be clickable.
         * Cent percent unittest coverage.
         * Added Selenium 4 support for ActionChains methods
+        * Supports Selenium 4 ActionChains methods
         * Raised custom Page factory exceptions
         
         Installation
         =============
         
         ```shell
           pip install selenium-page-factory
@@ -90,14 +91,18 @@
               <td >context_click</td>
               <td >execute_script</td> 
             </tr>
         	<tr>
               <td >click_and_hold</td>
               <td >release</td> 
             </tr>
+        	<tr>
+              <td >hover_with_offset</td>
+              <td >Coming soon...</td> 
+            </tr>
           </tbody>
         </table>
         
          Note: 
          Every WebElement will be created after verifying it's Presence and visibility on Page at Run-Time.
```

### Comparing `selenium-page-factory-2.6/README.md` & `selenium-page-factory-2.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Main Features
 =============
 
 * Initialise all the webElements declared in Point at a time.
 * All WebElements methods are re-define to add extra features eg- click method extended to have explicit wait for element to be clickable.
 * Cent percent unittest coverage.
 * Added Selenium 4 support for ActionChains methods
+* Supports Selenium 4 ActionChains methods
 * Raised custom Page factory exceptions
 
 Installation
 =============
 
 ```shell
   pip install selenium-page-factory
@@ -82,14 +83,18 @@
       <td >context_click</td>
       <td >execute_script</td> 
     </tr>
 	<tr>
       <td >click_and_hold</td>
       <td >release</td> 
     </tr>
+	<tr>
+      <td >hover_with_offset</td>
+      <td >Coming soon...</td> 
+    </tr>
   </tbody>
 </table>
 
  Note: 
  Every WebElement will be created after verifying it's Presence and visibility on Page at Run-Time.
```

### Comparing `selenium-page-factory-2.6/selenium_page_factory.egg-info/PKG-INFO` & `selenium-page-factory-2.7/selenium_page_factory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-page-factory
-Version: 2.6
+Version: 2.7
 Summary: Python library provides page factory approach to implement page object model in selenium
 Home-page: https://github.com/NayakwadiS/selenium-page-factory
 Author: Sujit Nayakwadi
 Author-email: nayakwadi_sujit@rediffmail.com
 License: MIT
 Description: A Page Factory is one way of implementing a Page Object Model. In order to support the Page Object pattern.
         As in Java we are using @findBy, here we are declaring all web element in dictionary.
@@ -14,14 +14,15 @@
         Main Features
         =============
         
         * Initialise all the webElements declared in Point at a time.
         * All WebElements methods are re-define to add extra features eg- click method extended to have explicit wait for element to be clickable.
         * Cent percent unittest coverage.
         * Added Selenium 4 support for ActionChains methods
+        * Supports Selenium 4 ActionChains methods
         * Raised custom Page factory exceptions
         
         Installation
         =============
         
         ```shell
           pip install selenium-page-factory
@@ -90,14 +91,18 @@
               <td >context_click</td>
               <td >execute_script</td> 
             </tr>
         	<tr>
               <td >click_and_hold</td>
               <td >release</td> 
             </tr>
+        	<tr>
+              <td >hover_with_offset</td>
+              <td >Coming soon...</td> 
+            </tr>
           </tbody>
         </table>
         
          Note: 
          Every WebElement will be created after verifying it's Presence and visibility on Page at Run-Time.
```

### Comparing `selenium-page-factory-2.6/seleniumpagefactory/Pagefactory.py` & `selenium-page-factory-2.7/seleniumpagefactory/Pagefactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import *
 from selenium.webdriver import ActionChains
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support.ui import Select
 
+
 class PageFactoryException(Exception):
     """Base class for exceptions in this module."""
     pass
+
+
 class ElementNotFoundException(PageFactoryException):
     """Raised when the element is not found in the page. (Using ` EC.presence_of_element_located` function from within __getattr__ method)."""
+
+
 class ElementNotVisibleException(PageFactoryException):
     """Raised when the element is not visible in the page. (Using `EC.visibility_of_element_located` function from within __getattr__ method)."""
 
 
 class PageFactory(object):
     timeout = 10
     highlight = False
-    mobile_test = False     #Added for Mobile support
+    mobile_test = False  # Added for Mobile support
 
     TYPE_OF_LOCATORS = {
         'css': By.CSS_SELECTOR,
         'id': By.ID,
         'name': By.NAME,
         'xpath': By.XPATH,
         'link_text': By.LINK_TEXT,
@@ -41,40 +46,40 @@
             self.driver = instance.driver
 
     def __getattr__(self, loc):
 
         if self.mobile_test == True:
             if loc in self.locators.keys():
                 element = self.find_element_by_accessibility_id(self.locators[loc][1])
-                return element             
+                return element
         else:
             if loc in self.locators.keys():
                 locator = (self.TYPE_OF_LOCATORS[self.locators[loc][0].lower()], self.locators[loc][1])
                 try:
                     element = WebDriverWait(self.driver, self.timeout).until(
                         EC.presence_of_element_located(locator)
                     )
                 except (StaleElementReferenceException, NoSuchElementException, TimeoutException) as e:
                     raise ElementNotFoundException(
                         "An exception of type " + type(e).__name__ +
                         " occurred. With Element -: " + loc +
                         " - locator: (" + locator[0] + ", " + locator[1] + ")"
                     )
-    
+
                 try:
                     element = WebDriverWait(self.driver, self.timeout).until(
                         EC.visibility_of_element_located(locator)
                     )
                 except (StaleElementReferenceException, NoSuchElementException, TimeoutException) as e:
                     raise ElementNotVisibleException(
                         "An exception of type " + type(e).__name__ +
                         " occurred. With Element -: " + loc +
                         " - locator: (" + locator[0] + ", " + locator[1] + ")"
                     )
-    
+
                 element = self.get_web_element(*locator)
                 element._locator = locator
                 return element
         return super().__getattr__(loc)
 
     def get_web_element(self, *loc):
         element = self.driver.find_element(*loc)
@@ -211,14 +216,24 @@
         Added support for Selenium 4
         :param: None
         :return: webElement
         """
         ActionChains(self.parent).release(on_element=self)
         return self
 
+    def hover_with_offset(self, x, y):
+        """
+        Move the mouse by an offset of the specified element. Offsets are relative to the top-left corner of the element.
+        Added support for Selenium 4
+        :param: x and y offset
+        :return: webElement
+        """
+        ActionChains(self.parent).move_to_element_with_offset(to_element=self, xoffset=x, yoffset=y)
+        return self
+
     def set_text(self, value):
         """
         type text in input box
         :param: Text to be Enter
         :return: webElement
         """
         self.element_to_be_clickable()
@@ -324,14 +339,15 @@
 
 
 WebElement.click_button = PageFactory.click_button
 WebElement.double_click = PageFactory.double_click
 WebElement.context_click = PageFactory.context_click
 WebElement.click_and_hold = PageFactory.click_and_hold
 WebElement.release = PageFactory.release
+WebElement.hover_with_offset = PageFactory.hover_with_offset
 WebElement.element_to_be_clickable = PageFactory.element_to_be_clickable
 WebElement.invisibility_of_element_located = PageFactory.invisibility_of_element_located
 WebElement.visibility_of_element_located = PageFactory.visibility_of_element_located
 WebElement.set_text = PageFactory.set_text
 WebElement.get_text = PageFactory.get_text
 WebElement.hover = PageFactory.hover
 WebElement.clear_text = PageFactory.clear_text
```

### Comparing `selenium-page-factory-2.6/seleniumpagefactory/__init__.py` & `selenium-page-factory-2.7/seleniumpagefactory/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
     The MIT License (MIT)
-    Copyright (c) 2023 Sujit Nayakwadi
+    Copyright (c) 2024 Sujit Nayakwadi
     Permission is hereby granted, free of charge, to any person obtaining a copy
     of this software and associated documentation files (the "Software"), to deal
     in the Software without restriction, including without limitation the rights
     to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
     copies of the Software, and to permit persons to whom the Software is
     furnished to do so, subject to the following conditions:
     The above copyright notice and this permission notice shall be included in all
@@ -13,9 +13,9 @@
     IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
     FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
     AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
     LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
     OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
     SOFTWARE.
 """
-__VERSION__='2.6'
+__VERSION__='2.7'
 from seleniumpagefactory.Pagefactory import PageFactory
```

### Comparing `selenium-page-factory-2.6/setup.py` & `selenium-page-factory-2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="selenium-page-factory",
-    version="2.6",
+    version="2.7",
     author = "Sujit Nayakwadi",
     author_email="nayakwadi_sujit@rediffmail.com",
     description="Python library provides page factory approach to implement page object model in selenium",
     license="MIT",
     keywords="selenium, page object model, pom, pages, page factory",
     install_requires=['selenium'],
     url="https://github.com/NayakwadiS/selenium-page-factory",
```

### Comparing `selenium-page-factory-2.6/tests/selenium_unitest.py` & `selenium-page-factory-2.7/tests/selenium_unitest.py`

 * *Files identical despite different names*

### Comparing `selenium-page-factory-2.6/tests/test_selenium.py` & `selenium-page-factory-2.7/tests/test_selenium.py`

 * *Files identical despite different names*

