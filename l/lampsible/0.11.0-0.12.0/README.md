# Comparing `tmp/lampsible-0.11.0.tar.gz` & `tmp/lampsible-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lampsible-0.11.0.tar", last modified: Mon Mar 11 22:22:16 2024, max compression
+gzip compressed data, was "lampsible-0.12.0.tar", last modified: Sun Apr 14 18:43:00 2024, max compression
```

## Comparing `lampsible-0.11.0.tar` & `lampsible-0.12.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/
--rw-rw-r--   0 brian     (1000) brian     (1000)       54 2024-03-11 22:21:34.000000 lampsible-0.11.0/.gitignore
--rw-rw-r--   0 brian     (1000) brian     (1000)    11358 2024-03-11 22:21:34.000000 lampsible-0.11.0/LICENSE
--rw-r--r--   0 brian     (1000) brian     (1000)     5756 2024-03-11 22:22:16.954510 lampsible-0.11.0/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     4922 2024-03-11 22:21:34.000000 lampsible-0.11.0/README.md
--rw-rw-r--   0 brian     (1000) brian     (1000)     1123 2024-03-11 22:21:34.000000 lampsible-0.11.0/pyproject.toml
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-03-11 22:22:16.954510 lampsible-0.11.0/setup.cfg
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.946510 lampsible-0.11.0/src/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/
--rw-rw-r--   0 brian     (1000) brian     (1000)        0 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12779 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/arg_validator.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      681 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/constants.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14332 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/lampsible.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/
--rw-rw-r--   0 brian     (1000) brian     (1000)       66 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/ansible-galaxy-requirements.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      811 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/apache.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      854 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/lamp-stack.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      383 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/mysql.yml
--rw-rw-r--   0 brian     (1000) brian     (1000)      331 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/php.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.946510 lampsible-0.11.0/src/lampsible/project/roles/apache-conf/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/apache-conf/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      391 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apache-conf/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/apache-conf/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      948 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.946510 lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      517 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1591 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
--rw-rw-r--   0 brian     (1000) brian     (1000)     6489 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.946510 lampsible-0.11.0/src/lampsible/project/roles/apache2/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/apache2/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      133 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apache2/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/apt-update/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/apt-update/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)       67 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/apt-update/tasks/main.yaml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/domain-for-wordpress/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/domain-for-wordpress/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      910 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/fail2ban/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/fail2ban/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      299 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/fail2ban/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/fail2ban/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      971 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/mysql/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/mysql/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1371 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/mysql/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/php/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/php/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      969 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/php/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      495 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)     7260 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
--rw-rw-r--   0 brian     (1000) brian     (1000)    73018 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/pip/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/pip/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)       63 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/pip/tasks/main.yaml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/ssl-certbot/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/ssl-certbot/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      900 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/ssl-certbot/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/ssl-selfsigned/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/ssl-selfsigned/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)      994 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.950510 lampsible-0.11.0/src/lampsible/project/roles/wordpress/
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/wordpress/tasks/
--rw-rw-r--   0 brian     (1000) brian     (1000)     3268 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/wordpress/tasks/main.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible/project/roles/wordpress/templates/
--rw-rw-r--   0 brian     (1000) brian     (1000)      582 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/roles/wordpress/templates/.htaccess
--rw-rw-r--   0 brian     (1000) brian     (1000)     1518 2024-03-11 22:21:34.000000 lampsible-0.11.0/src/lampsible/project/wordpress.yml
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-03-11 22:22:16.954510 lampsible-0.11.0/src/lampsible.egg-info/
--rw-r--r--   0 brian     (1000) brian     (1000)     5756 2024-03-11 22:22:16.000000 lampsible-0.11.0/src/lampsible.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)     1749 2024-03-11 22:22:16.000000 lampsible-0.11.0/src/lampsible.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-03-11 22:22:16.000000 lampsible-0.11.0/src/lampsible.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-03-11 22:22:16.000000 lampsible-0.11.0/src/lampsible.egg-info/entry_points.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       28 2024-03-11 22:22:16.000000 lampsible-0.11.0/src/lampsible.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-03-11 22:22:16.000000 lampsible-0.11.0/src/lampsible.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       54 2024-04-14 18:38:32.000000 lampsible-0.12.0/.gitignore
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11358 2024-04-14 18:38:32.000000 lampsible-0.12.0/LICENSE
+-rw-r--r--   0 brian     (1000) brian     (1000)     3831 2024-04-14 18:43:00.527672 lampsible-0.12.0/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2977 2024-04-14 18:38:32.000000 lampsible-0.12.0/README.md
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1135 2024-04-14 18:38:32.000000 lampsible-0.12.0/pyproject.toml
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2024-04-14 18:43:00.527672 lampsible-0.12.0/setup.cfg
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.519672 lampsible-0.12.0/src/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/
+-rw-rw-r--   0 brian     (1000) brian     (1000)        0 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    13680 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/arg_validator.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      681 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/constants.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    17401 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/lampsible.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       94 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/ansible-galaxy-requirements.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      944 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/apache.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      987 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/lamp-stack.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      383 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/mysql.yml
+-rw-rw-r--   0 brian     (1000) brian     (1000)      331 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/php.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.519672 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      391 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      948 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      517 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1507 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6434 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/apache2/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apache2/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      322 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apache2/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/apt-update/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/apt-update/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       67 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/apt-update/tasks/main.yaml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      752 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      299 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      971 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/mysql/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/mysql/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1371 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/mysql/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/php/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/php/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      969 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/php/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      495 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7260 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73018 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/pip/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/pip/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       63 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/pip/tasks/main.yaml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/ssl-certbot/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/ssl-certbot/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      265 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/ssl-certbot/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      881 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.523672 lampsible-0.12.0/src/lampsible/project/roles/wordpress/
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/wordpress/tasks/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3268 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/wordpress/tasks/main.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible/project/roles/wordpress/templates/
+-rw-rw-r--   0 brian     (1000) brian     (1000)      582 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/roles/wordpress/templates/.htaccess
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1651 2024-04-14 18:38:32.000000 lampsible-0.12.0/src/lampsible/project/wordpress.yml
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2024-04-14 18:43:00.527672 lampsible-0.12.0/src/lampsible.egg-info/
+-rw-r--r--   0 brian     (1000) brian     (1000)     3831 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1749 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       55 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/entry_points.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       33 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)       10 2024-04-14 18:43:00.000000 lampsible-0.12.0/src/lampsible.egg-info/top_level.txt
```

### Comparing `lampsible-0.11.0/LICENSE` & `lampsible-0.12.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/README.md` & `lampsible-0.12.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: lampsible
+Version: 0.12.0
+Summary: Deploy and set up LAMP stacks with Ansible
+Author-email: "Brian St. Hilaire" <brian.st-hilaire@sanctus-tech.com>
+Project-URL: Homepage, https://github.com/saint-hilaire/lampsible
+Project-URL: Issues, https://github.com/saint-hilaire/lampsible/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Framework :: Ansible
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ansible-core
+Requires-Dist: ansible-runner
+Requires-Dist: fqdn
+
 # Lampsible
 
 ## About
 
 Lampsible - LAMP stacks with Ansible and a super simple CLI. You can use this tool to set up a
 LAMP stack with Ansible. That is, on a given Linux server, install Apache, MySQL, PHP,
 and some web application of your choice. Under the hood, it utilizes Ansible, a
@@ -46,15 +68,15 @@
 Some flags which you'll likely also want to use:
 
 * `--apache-vhost-name`
 * `--database-username`
 * `--php-version` (You'll need this on older Ubuntu versions, because they don't support PHP 8 out of the box)
 * `--wordpress-version`
 * `--ssl-certbot`
-* `--ssl-selfsigned` (See the note below about Certbot)
+* `--ssl-selfsigned`
 
 Run `lampsible --help` for a full list of options.
 
 ### Sample usage
 
 ```
 lampsible sampleuser your.server.com lamp-stack \
@@ -67,64 +89,27 @@
 they are created as well - otherwise they won't be created. You don't need to enter a database
 password, as it's generally insecure to do so over the CLI. Lampsible will prompt you for a password.)
 
 <br>
 
 ```
 lampsible sampleuser your.server.com wordpress \
-    --ssl-selfsigned
+    --ssl-certbot \
+    --email-for-ssl you@yourdomain.com
 ```
 (Along with the underlying LAMP stack, this installs WordPress on your server,
-and also sets up a self signed SSL certificate, so you have a secure connection
-to finish setting up your WordPress site. You don't have to provide any database
+and also sets up SSL via Certbot. You don't have to provide any database
 or Apache configurations - they will either be generated automatically,
 or you will be prompted to enter them.)
 
 
 **WARNING!** Never set up a WordPress site without immediately navigating to that site
 in your browser and finishing the "famous 5 minute WordPress installation",
 in which you enter the credentials for the admin user!
 Otherwise, someone else will do that for you, and use your server to host malicious content!
 
-### Note about Certbot
-
-Certbot is not completely working at the moment. It works, but you have to do
-part of the process directly on the remote server. There is also a little bit
-of difficutly with WordPress at the moment, because immediately after Lampsible
-finishes installing WordPress, (but before you finish the _"famous 5-minute install"_
-in the browser), the tables of the WP database won't exist yet, but in order for Certbot to
-work, they need to exist.
-
-For this reason, to install a fully functional, secure, production ready WordPress site,
-the workflow will need to look something like this:
-
-* First, install WordPress with the along with an self signed SSL certificate, so you have an
-  encrypted connection over which you can securely provide your admin credentials.
-```
-lampsible remoteuser your.server.com wordpress --ssl-selfsigned --apache-server-admin you@yourdomain.com
-```
-
-* Next, finish setting up WordPress by browsing to your new site and completing
-  the _"famous 5 minute install"_ - it takes a lot less than 5 minutes, but it
-  is **very important** that you do this immediately, because otherwise someone could
-  hijack your site by doing this step for you.
-
-* Now, rerun the lampsible command from before, but with the
-  `--ssl-certbot` flag instead of `--ssl-selfsigned`.
-```
-lampsible remoteuser your.server.com wordpress --ssl-certbot --apache-server-admin you@yourdomain.com
-```
-
-* Finally, SSH into your remote server, then, as root, run `certbot`.
-  Note that for WordPress sites, you'll have to enable SSL
-  not just for your.server.com but also www.your.server.com.
-  When Certbot prompts you to select a virtual host for which to to enable SSL,
-  select `wordpress-ssl.conf`. (That is assuming that you did not provide
-  an `--apache-vhost-name` of your own - in any case, pick the one with the `-ssl` in its name).
-
-
 ## Contributing 
 
 This tool is very much still in beta stage. If you want to help me improve this,
 I'll be very happy, just shoot me a message :-)
```

### Comparing `lampsible-0.11.0/pyproject.toml` & `lampsible-0.12.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,24 +3,25 @@
     "setuptools>=69.0",
     "setuptools-scm>=8.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lampsible"
-version = "0.11.0"
+version = "0.12.0"
 authors = [
     {name="Brian St. Hilaire", email="brian.st-hilaire@sanctus-tech.com"}
 ]
 description = "Deploy and set up LAMP stacks with Ansible"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "ansible-core",
     "ansible-runner",
+    "fqdn",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Framework :: Ansible",
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
```

### Comparing `lampsible-0.11.0/src/lampsible/arg_validator.py` & `lampsible-0.12.0/src/lampsible/arg_validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from re import match
 from copy import copy
 from secrets import token_hex
 from warnings import warn
 from getpass import getpass
+from fqdn import FQDN
 from lampsible.constants import *
 
 
 class ArgValidator():
 
     def __init__(self, args):
         self.args = args
@@ -22,15 +24,15 @@
     # TODO: I don't find this very elegant.
     def get_apache_custom_conf_name(self):
         try:
             return self.apache_custom_conf_name
         except AttributeError:
             return ''
 
-    
+
     # TODO: Improve/remove this when we fix Certbot.
     def get_domain_for_wordpress(self):
         try:
             return self.domain_for_wordpress
         except AttributeError:
             return ''
 
@@ -80,14 +82,25 @@
             or (
                 self.args.action == 'wordpress'
                 and not self.args.wordpress_insecure_allow_xmlrpc
             )
         )
 
 
+    def get_certbot_domains_string(self):
+        try:
+            return '-d {}'.format(' -d '.join(self.args.domains_for_ssl))
+        except TypeError:
+            return ''
+
+
+    def get_certbot_test_cert_string(self):
+        return '--test-cert' if self.args.test_cert else ''
+
+
     def handle_defaults(
         self,
         default_args,
         ask_user=False,
         verbose=False
     ):
         """Handles defaults in various cases, optionally setting values with
@@ -168,52 +181,52 @@
         else:
             print('Passwords don\'t match. Please try again.')
             return self.get_pass_and_check(prompt, min_length)
 
 
     def validate_apache_args(self):
 
+        server_name = self.args.host
+        try:
+            assert FQDN(server_name).is_valid
+        except AssertionError:
+            server_name = DEFAULT_APACHE_SERVER_NAME
+
         base_vhost_dict = {
             'base_vhost_file': '{}.conf'.format(DEFAULT_APACHE_VHOST_NAME),
             'document_root':  self.args.apache_document_root,
             'vhost_name':     self.args.apache_vhost_name,
-            # TODO: Temporarily disabled because it does not play
-            # nicely with Certbot.
-            # 'server_name':    self.args.apache_server_name,
+            'server_name':    server_name,
             'server_admin':   self.args.apache_server_admin,
+            'allow_override': self.get_apache_allow_override(),
         }
 
         if self.args.action == 'wordpress':
 
             if self.args.apache_document_root == DEFAULT_APACHE_DOCUMENT_ROOT:
                 base_vhost_dict['document_root'] = '{}/wordpress'.format(
                     DEFAULT_APACHE_DOCUMENT_ROOT)
             if self.args.apache_vhost_name == DEFAULT_APACHE_VHOST_NAME:
                 base_vhost_dict['vhost_name'] = 'wordpress'
 
         self.apache_vhosts = [base_vhost_dict]
 
-        if self.args.ssl_selfsigned or self.args.ssl_certbot:
+        if self.args.ssl_selfsigned:
 
             ssl_vhost_dict = copy(base_vhost_dict)
 
             ssl_vhost_dict['base_vhost_file'] = 'default-ssl.conf'
             ssl_vhost_dict['vhost_name']      += '-ssl'
 
             self.apache_vhosts.append(ssl_vhost_dict)
-            self.apache_custom_conf_name = 'ssl-params'
 
-        # if ssl_action:
-        #     # TODO: Does not work for Certbot, unless the client is
-        #     # run with the flag --register-unsafely-without-email.
-        #     # TODO: This method has been refactored, so this is now broken.
-        #     self.handle_defaults([{
-        #         'arg_name': 'email_for_ssl',
-        #         'cli_default_value': self.args.apache_server_admin,
-        #     }], False, True)
+            if self.args.ssl_selfsigned:
+                self.apache_custom_conf_name = 'ssl-params'
+
+        return 0
 
 
     def validate_database_args(self):
 
         # TODO: Sanity check database username and database name.
 
         if self.args.database_engine != DEFAULT_DATABASE_ENGINE \
@@ -221,15 +234,16 @@
             or self.args.php_my_admin:
 
             raise NotImplementedError()
 
         if self.args.database_password \
             and not self.args.insecure_cli_password:
 
-            exit('It\'s insecure to pass passwords via CLI args! If you are sure that you want to do this, rerun this command with the --insecure-cli-password flag.')
+            print('It\'s insecure to pass passwords via CLI args! If you are sure that you want to do this, rerun this command with the --insecure-cli-password flag.')
+            return 1
 
         # TODO: Add some option like --wordpress-defaults, to improve user
         # experience. Otherwise, the user would always be asked about defaulting
         # to 'wordpress' and 'wp_' for database name and table prefix, which
         # might be a little annoying.
         if self.args.action == 'wordpress':
             self.handle_defaults([
@@ -252,66 +266,96 @@
 
         if self.args.database_username and not self.args.database_password:
             self.args.database_password = self.get_pass_and_check(
                 'Please enter a database password: ',
                 7
             )
 
+        return 0
+
 
     def validate_ssl_args(self):
 
         if self.args.ssl_certbot:
-            if self.args.ssl_selfsigned:
-                warn('Warning: Got --ssl-certbot, but also got --ssl-selfsigned. Ignoring --ssl-selfsigned and using --ssl-certbot.')
             ssl_action = 'certbot'
         elif self.args.ssl_selfsigned:
-            warn('Warning! Creating a self signed certificate to handle the site\'s encryption. This is less secure and will appear untrustworthy to any visitors. Only use this for testing environments.')
             ssl_action = 'selfsigned'
         else:
-            warn('WARNING! Your site will not have any encryption enabled! This is very insecure, as passwords and other sensitive data will be transmitted in clear text. DO NOT use this on any remote host or over any partially untrusted network. ONLY use this for local, secure, private and trusted networks, ideally only for local development servers.')
             ssl_action = None
 
-        # TODO: Improve this when we fix Certbot.
         if ssl_action == 'certbot':
             self.handle_defaults([
                 {
                     'arg_name': 'domains_for_ssl',
                     'cli_default_value': None,
-                    'override_default_value': self.args.hosts.split(','),
+                    'override_default_value': [self.args.host],
                 },
                 {
                     'arg_name': 'email_for_ssl',
-                    'cli_default_value': self.args.apache_server_admin,
+                    'cli_default_value': None,
+                    'override_default_value': self.args.apache_server_admin,
                 },
             ])
+
+            if not match(r"[^@]+@[^@]+\.[^@]+", self.args.email_for_ssl):
+                print("FATAL! --email-for-ssl needs to be valid. Got '{}'. Aborting.".format(
+                    self.args.email_for_ssl))
+                return 1
+
             if self.args.action == 'wordpress':
-                self.args.domains_for_ssl.append(
-                    'www.{}'.format(self.args.domains_for_ssl[0])
-                )
-                self.domain_for_wordpress = self.args.domains_for_ssl[-1]
+                if self.args.host[:4] == 'www.':
+                    www_domain = self.args.host
+                else:
+                    www_domain = 'www.{}'.format(self.args.host)
+
+                if www_domain not in self.args.domains_for_ssl:
+                    self.args.domains_for_ssl.append(www_domain)
+
+                self.domain_for_wordpress = www_domain
+
+        return 0
 
 
     def validate_php_args(self):
         # TODO: If we can get the ansible_facts back into a Python variable,
         # we can validate this stuff too.
         # NOTE:
         # * Ubuntu versions 20 and older do not support PHP versions 8.0 or newer
         # * Ubuntu 22 does not support PHP 8.0. PHP 8.1 is supported.
         # To work around the above points, you would have to manually configure the
         # APT repository.
         if self.args.skip_php_extensions:
-            warn('Will not install common PHP extensions. WordPress, Laravel, and other common CMS or frameworks will probably not work.')
+            print('Will not install common PHP extensions. WordPress, Laravel, and other common CMS or frameworks will probably not work.')
+
+        return 0
 
 
     def print_warnings(self):
         if self.args.insecure_skip_fail2ban:
             print('Warning! Will not install fail2ban! Your site will potentially be vulnerable to various brute force attacks. You should only pass the \'--insecure-skip-fail2ban\' flag if you have a good reason to do so. On production servers, always install fail2ban!')
+
         if self.args.wordpress_insecure_allow_xmlrpc:
             print('Warning! Your WordPress site\'s xmlrpc.php endpoint will be enabled - this is insecure! The endpoint xmlrpc.php is a feature from older WordPress versions which allowed programmatic access to the WordPress backend. Although it has numerous known security vulnerabilities, namely a brute force and a DoS vulnerability, it is still, for some reason, enabled by default in current WordPress versions. Lampsible will, by default, block this endpoint with an .htaccess configuration, unless you specify otherwise, which you just did. You should not be doing this, unless you have some good reason to do so!')
 
+        if self.args.ssl_certbot and self.args.ssl_selfsigned:
+            print('Warning: Got --ssl-certbot, but also got --ssl-selfsigned. Ignoring --ssl-selfsigned and using --ssl-certbot.')
+        elif self.args.ssl_selfsigned:
+            print('Warning! Creating a self signed certificate to handle the site\'s encryption. This is less secure and will appear untrustworthy to any visitors. Only use this for testing environments.')
+        elif not (self.args.ssl_selfsigned or self.args.ssl_certbot):
+            print('WARNING! Your site will not have any encryption enabled! This is very insecure, as passwords and other sensitive data will be transmitted in clear text. DO NOT use this on any remote host or over any partially untrusted network. ONLY use this for local, secure, private and trusted networks, ideally only for local development servers.')
+
 
     def validate_args(self):
-        self.validate_apache_args()
-        self.validate_database_args()
-        self.validate_ssl_args()
-        self.validate_php_args()
+        validate_methods = [
+            'validate_apache_args',
+            'validate_database_args',
+            'validate_ssl_args',
+            'validate_php_args',
+        ]
+        for method_name in validate_methods:
+            method = getattr(self, method_name)
+            result = method()
+            if result != 0:
+                return result
+
         self.print_warnings()
+        return 0
```

### Comparing `lampsible-0.11.0/src/lampsible/constants.py` & `lampsible-0.12.0/src/lampsible/constants.py`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/lampsible.py` & `lampsible-0.12.0/src/lampsible/lampsible.py`

 * *Files 20% similar despite different names*

```diff
@@ -74,83 +74,128 @@
     #         },
     #     },
     # }
     # with open(os.path.join(private_data_dir, 'inventory', 'hosts'), 'w') as fh:
     #     fh.write(yaml.dump(inventory))
 
 
-def prepare_inventory(users, hosts):
-    # TODO: Funny thing... doing hosts and users this way works for the
-    # ansible_runner module when we use it in this script, but does not work
-    # for the ansible-runner as a CLI tool... even though in the venv 
-    # they should be the same versions.
-    hosts_ls = hosts.split(',')
-    users_ls = users.split(',')
-    l = len(hosts_ls)
-    if len(users_ls) != l:
-        raise NotImplementedError('For now, you have to pass users and hosts as lists that match one to one exactly. This will be improved in a future version.')
-
-    if l > 1: 
-        hosts = ['{}@{}'.format(users_ls[i], hosts_ls[i]) for i in range(l)]
-        return ','.join(hosts)
-    elif l == 1:
-        return '{}@{},'.format(users_ls[0], hosts_ls[0])
-    else:
-        raise ValueError('Got bad value for --users or --hosts.')
-    
-    # TODO: Passing an inventory directly as a dictionary to Ansible is currenlty
-    # not possible... unfortunately! It should be...
-    # hosts = {hosts_ls[i]: users_ls[i] for i in range(l)}
+def prepare_inventory(user, host):
+    ########
+    # TODO #
+    ########
+
+    # Dealing with inventories can be tricky.
+    # This is a big part of what will have to be refactored in the future.
+    # Ideally, it should be possible to pass the inventories to Ansible,
+    # along with all sorts of variables, as a dictionary. However,
+    # that appears not to be possible at the moment. If it truly is not
+    # possible, this might be a worthwhile improvment to Ansible itself.
+    # See the code below.
 
+    # hosts = {hosts_ls[i]: users_ls[i] for i in range(l)}
     # inventory = {
     #     'ungrouped': {
     #         'hosts': {
     #             host: {'ansible_user': user} for host, user in hosts.items()
     #         },
+    #         # various variables here...
     #     },
     # }
 
-    # return inventory
+    # Without dictionaries, it would mean that we would have to create
+    # some temporary files on the local filesystem to handle all the
+    # inventory configuration. This is OK, but IMO not ideal. In any case,
+    # I don't want to implement that into this project, but rather, into some
+    # "Python-Ansible-Runner" library.
+
+    # So for the time being, there are no "inventories-per-dictionary" (might
+    # require changes to Ansible itself), nor "inventory-per-tmp-file" (won't
+    # implement in this codebase, but rather in other library).
+
+    # It's possible to pass "work around" the need for the "local inventory
+    # file" by passing a comma separated list to Ansible. The commented out
+    # code below does exactly that. However, dealing with multiple users and
+    # hosts this way introduces unnecessary and unwieldy complexities, which
+    # most of the time wouldn't be needed by a tool as simple as Lampsible
+    # anyway. Funny thing... doing hosts and users this way works for the
+    # ansible_runner module when we use it in this script, but does not work
+    # for the ansible-runner as a CLI tool... even though in the venv 
+    # they should be the same versions.
+
+    # hosts_ls = hosts.split(',')
+    # users_ls = users.split(',')
+    # l = len(hosts_ls)
+    # if len(users_ls) != l:
+    #     raise NotImplementedError('For now, you have to pass users and hosts as lists that match one to one exactly. This will be improved in a future version.')
+
+    # if l > 1: 
+    #     hosts = ['{}@{}'.format(users_ls[i], hosts_ls[i]) for i in range(l)]
+    #     return ','.join(hosts)
+    # elif l == 1:
+    #     return '{}@{},'.format(users_ls[0], hosts_ls[0])
+    # else:
+    #     raise ValueError('Got bad value for --users or --hosts.')
+
+    # For these reasons, we confine ourselves for now to the simple
+    # "one user, one host" inventory. Note the comma at the end of the
+    # inventory string - that is needed, in order for Ansible to process it
+    # this way.
+
+    # To do the inventories "The Right Way", I want to find out, if it maybe
+    # isn't possible to configure the entire invetory in one single
+    # dictionary, and pass that directly to Ansible-Runner - and possibly
+    # contribute those changes to the maintainers of Ansible itself. Failing
+    # that, I want to implement some small library to handle tasks like
+    # 'writing Anisble inventory file temporarily to local filesystem', which
+    # would then be required by this application. 
+
+    # Another thing that will be important in the future is for the web-
+    # and database-servers to run on different hosts.
+    return '{}@{},'.format(user, host)
 
 
 def cleanup_private_data_dir(path):
     # TODO: Do this the right way.
     # TODO: Implement some safety measures to avoid data destruction.
     os.system('rm -r ' + path)
 
 
 # TODO: See GH Issue #4. Currently the user is always prompted  for this.
 # The user should only be prompted for this, when the requirements are not met.
 def ensure_ansible_galaxy_dependencies(galaxy_requirements_file):
-    ok_to_install = input("I have to download and install the Ansible Galaxy dependencies 'community.mysql' and 'community.crypto' into {}. Is this OK (yes/no)? ".format(
+    ok_to_install = input("I have to download and install the Ansible Galaxy dependencies 'community.general', 'community.mysql' and 'community.crypto' into {}. Is this OK (yes/no)? ".format(
         os.path.join(USER_HOME_DIR, '.ansible/')
     )).lower()
     while ok_to_install != 'yes' and ok_to_install != 'no':
         ok_to_install = input("Please type 'yes' or 'no': ")
     if ok_to_install == 'yes':
         run_command(
             executable_cmd='ansible-galaxy',
             cmdline_args=['collection', 'install', '-r', galaxy_requirements_file],
         )
+        # run_command(
+        #     executable_cmd='ansible-galaxy',
+        #     cmdline_args=['role', 'install', '-r', galaxy_requirements_file],
+        # )
         return 0
     else:
         print('Cannot run Ansible plays without Galaxy requirements. Aborting.')
         return 1
 
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog='lampsible',
         description='Deploy and set up LAMP Stacks with Ansible',
         epilog='Currently in development...',
     )
     # TODO
-    parser.add_argument('users')
-    parser.add_argument('hosts')
+    parser.add_argument('user')
+    parser.add_argument('host')
 
     # TODO: Validation
     parser.add_argument('action', choices=[
         # LAMP-Stack basics
         'lamp-stack',
         'apache',
         'mysql',
@@ -179,18 +224,14 @@
     )
 
     # APACHE
     ########
     # TODO: Apache configs, versions, etc? Nginx or others?
     parser.add_argument('--apache-vhost-name',
         default=DEFAULT_APACHE_VHOST_NAME)
-    # TODO: Temporarily disabled because it does not play
-    # nicely with Certbot.
-    # parser.add_argument('--apache-server-name',
-    #     default=DEFAULT_APACHE_SERVER_NAME)
     parser.add_argument('--apache-server-admin',
         default=DEFAULT_APACHE_SERVER_ADMIN)
     parser.add_argument('--apache-document-root',
         default=DEFAULT_APACHE_DOCUMENT_ROOT)
 
     # DATABASE
     #######
@@ -236,26 +277,43 @@
     parser.add_argument('--project-dir',      default=DEFAULT_PROJECT_DIR)
     parser.add_argument('--keep-private-data-dir', action='store_true')
 
     # SSL
     #####
     parser.add_argument('--ssl-certbot', action='store_true')
     parser.add_argument('--ssl-selfsigned', action='store_true')
-    parser.add_argument('--email-for-ssl', default=DEFAULT_APACHE_SERVER_ADMIN)
+    parser.add_argument('--email-for-ssl')
     parser.add_argument('--domains-for-ssl')
+    parser.add_argument('--test-cert', action='store_true')
+
+    # TODO: This is intended as a temporary workaround.
+    # Ideally, we implement https://github.com/saint-hilaire/lampsible/issues/14
+    # and then there should be no need to configure the length of time for
+    # which Ansible pauses to allow the user to perform this step (unless
+    # the user wants to do it in the browser, via some
+    # --wordpress-interactive-install?)
+    # Failing that, it would be quite good if a future version of
+    # Ansible Runner can improve the handling of user input in the context
+    # of paused Playbooks (see issues
+    # https://github.com/ansible/ansible-runner/issues/1075
+    # and https://github.com/ansible/ansible-runner/issues/756):
+    parser.add_argument('--wordpress-5-minute-install-seconds', default=120)
 
     # MISC
     ######
     parser.add_argument('--insecure-cli-password', action='store_true')
     parser.add_argument('--insecure-skip-fail2ban', action='store_true')
 
     args = parser.parse_args()
 
     validator = ArgValidator(args)
-    validator.validate_args()
+    result = validator.validate_args()
+    if result != 0:
+        print('FATAL! validator.validate_args returned non zero return code. Aborting.')
+        return 1
     args = validator.get_args()
 
     # TODO: Let arg_validator handle private_data_dir, project_dir,
     # inventory and playbook as well, but for now, this will do.
     private_data_dir = init_private_data_dir(args.private_data_dir)
     # TODO: Where to put this?
     # Putting it directly into the package build seems the more simple and
@@ -265,15 +323,15 @@
     # configurable by the user. In this case, ~/.lampsible could be the
     # default value, but if users override this, they could provide their own
     # playbooks.
     # For now, let's simply bring the directory directly into the package
     # build.
     project_dir = init_project_dir(args.project_dir)
 
-    inventory = prepare_inventory(args.users, args.hosts)
+    inventory = prepare_inventory(args.user, args.host)
     # Now inventory is something like 'user1@host1,user2@host2' 
     # or 'user1@host1,'
 
     galaxy_result = ensure_ansible_galaxy_dependencies(os.path.join(
         project_dir, 'ansible-galaxy-requirements.yml'))
 
     # TODO: SyntaxWarning: "is" with a literal. Did you mean "=="?
@@ -308,50 +366,44 @@
     playbook = '{}.yml'.format(args.action)
     if not os.path.exists(os.path.join(project_dir, playbook)):
         # TODO: In the future we will have to change how this is validated.
         raise NotImplementedError()
 
     apache_vhosts = validator.get_apache_vhosts()
     apache_custom_conf_name = validator.get_apache_custom_conf_name()
-    apache_allow_override = validator.get_apache_allow_override()
 
     wordpress_auth_vars = validator.get_wordpress_auth_vars()
 
-    # TODO
-    # if roles and len(roles) > 1:
-    #     roles = ','.join(roles) 
-    # elif roles:
-    #     roles = roles.pop()
-
     rc = RunnerConfig(
         private_data_dir=private_data_dir,
         project_dir=project_dir,
 
         inventory=inventory,
 
         extravars={
             'apache_vhosts': apache_vhosts,
             'apache_custom_conf_name': apache_custom_conf_name,
-            'apache_allow_override': apache_allow_override,
             'database_username': args.database_username,
             'database_password': args.database_password,
             'database_host': args.database_host,
             'database_name': args.database_name,
             'database_table_prefix': args.database_table_prefix,
             'php_version': args.php_version,
             'skip_php_extensions': args.skip_php_extensions,
             'wordpress_version': args.wordpress_version,
             'wordpress_auth_vars': wordpress_auth_vars,
             'wordpress_insecure_allow_xmlrpc': args.wordpress_insecure_allow_xmlrpc,
             'ssl_certbot': args.ssl_certbot,
             'ssl_selfsigned': args.ssl_selfsigned,
             'email_for_ssl': args.email_for_ssl,
-            'domains_for_ssl': args.domains_for_ssl,
+            'certbot_domains_string': validator.get_certbot_domains_string(),
+            'certbot_test_cert_string': validator.get_certbot_test_cert_string(),
             # TODO: Improve this when we fix Certbot.
             'domain_for_wordpress': validator.get_domain_for_wordpress(),
+            'wordpress_5_minute_install_seconds': args.wordpress_5_minute_install_seconds,
             'insecure_skip_fail2ban': args.insecure_skip_fail2ban,
         },
         playbook=playbook,
     )
 
     if args.ssh_key_file:
         try:
```

### Comparing `lampsible-0.11.0/src/lampsible/project/apache.yml` & `lampsible-0.12.0/src/lampsible/project/apache.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,24 +12,25 @@
         - apache2
 
     - name: Conditionally include SSL role
       include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
-    # TODO
+    # It's important that this runs after the selfsigned certificates,
+    # if those are being used, but before Certbot, if that's being used.
+    - name: Include Apache virtual host role
+      include_role:
+        name: apache-vhosts
+
     - name: Conditionally include SSL role
       include_role:
         name: ssl-certbot
       when: ssl_certbot
 
-    - name: Include Apache virtual host role
-      include_role:
-        name: apache-vhosts
-
     - name: Conditionally include custom Apache configuration
       include_role:
         name: apache-conf
       when: ssl_selfsigned
 
     - name: Conditionally include fail2ban role
       include_role:
```

### Comparing `lampsible-0.11.0/src/lampsible/project/lamp-stack.yml` & `lampsible-0.12.0/src/lampsible/project/lamp-stack.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,25 @@
         - mysql
 
     - name: Conditionally include SSL role
       include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
-    # TODO
+    # It's important that this runs after the selfsigned certificates,
+    # if those are being used, but before Certbot, if that's being used.
+    - name: Include Apache virtual host role
+      include_role:
+        name: apache-vhosts
+
     - name: Conditionally include SSL role
       include_role:
         name: ssl-certbot
       when: ssl_certbot
 
-    - name: Include Apache virtual host role
-      include_role:
-        name: apache-vhosts
-
     - name: Conditionally include custom Apache configuration
       include_role:
         name: apache-conf
       when: ssl_selfsigned
 
     - name: Conditionally include fail2ban role
       include_role:
```

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2` & `lampsible-0.12.0/src/lampsible/project/roles/apache-conf/templates/ssl-params.conf.j2`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml` & `lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2` & `lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/000-default.conf.j2`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 	# The ServerName directive sets the request scheme, hostname and port that
 	# the server uses to identify itself. This is used when creating
 	# redirection URLs. In the context of virtual hosts, the ServerName
 	# specifies what hostname must appear in the request's Host: header to
 	# match this virtual host. For the default virtual host (this file) this
 	# value is not decisive as it is used as a last resort host regardless.
 	# However, you must set it for any further virtual host explicitly.
-	#ServerName www.example.com
-	{#
-	TODO: For now, not including a ServerName configuration until I figure
-	out how to make it play nicely with Certbot.
-	#}
+	ServerName {{ item.server_name }}
+	ServerAlias *.{{ item.server_name }}
 
 	ServerAdmin {{ item.server_admin }}
 	DocumentRoot {{ item.document_root }}
 
 	# Available loglevels: trace8, ..., trace1, debug, info, notice, warn,
 	# error, crit, alert, emerg.
 	# It is also possible to configure the loglevel for particular
@@ -26,15 +23,15 @@
 
 	# For most configuration files from conf-available/, which are
 	# enabled or disabled at a global level, it is possible to
 	# include a line for only one particular virtual host. For example the
 	# following line enables the CGI configuration for this host only
 	# after it has been globally disabled with "a2disconf".
 	#Include conf-available/serve-cgi-bin.conf
-	{% if apache_allow_override %}
+	{% if item.allow_override %}
 	<Directory {{ item.document_root }}>
 		Options FollowSymLinks
 		AllowOverride All
 		Require all granted
 	</Directory>
 	{% endif %}
 </VirtualHost>
```

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2` & `lampsible-0.12.0/src/lampsible/project/roles/apache-vhosts/templates/default-ssl.conf.j2`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 <VirtualHost *:443>
 	ServerAdmin {{ item.server_admin }}
 
 	DocumentRoot {{ item.document_root }}
 
-	{#
-	TODO: For now, not including a ServerName configuration until I figure
-	out how to make it play nicely with Certbot.
-	#}
+	ServerName {{ item.server_name }}
+	ServerAlias *.{{ item.server_name }}
 
 	# Available loglevels: trace8, ..., trace1, debug, info, notice, warn,
 	# error, crit, alert, emerg.
 	# It is also possible to configure the loglevel for particular
 	# modules, e.g.
 	#LogLevel info ssl:warn
 
@@ -99,15 +97,15 @@
 	#SSLOptions +FakeBasicAuth +ExportCertData +StrictRequire
 	<FilesMatch "\.(?:cgi|shtml|phtml|php)$">
 		SSLOptions +StdEnvVars
 	</FilesMatch>
 	<Directory /usr/lib/cgi-bin>
 		SSLOptions +StdEnvVars
 	</Directory>
-	{% if apache_allow_override %}
+	{% if item.allow_override %}
 	<Directory {{ item.document_root }}>
 		Options FollowSymLinks
 		AllowOverride All
 		Require all granted
 	</Directory>
 	{% endif %}
```

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml` & `lampsible-0.12.0/src/lampsible/project/roles/domain-for-wordpress/tasks/main.yml`

 * *Files 16% similar despite different names*

```diff
@@ -6,11 +6,11 @@
     query: "UPDATE {{ database_table_prefix }}options SET option_value = %s WHERE option_name IN ('siteurl', 'home')"
     positional_args:
       - "http://{{ domain_for_wordpress }}"
     login_unix_socket: /run/mysqld/mysqld.sock
   ignore_errors: true
 
 - debug:
-    msg: Tried to supply WordPress domain configuration via raw MySQL command. If this failed, it was because no tables exist, because WordPress has not been fully set up yet. Please finish setting up WordPress via web browser, then run this playbook again. Make sure to do so via an encrypted connection (you should run this script with --ssl-selfsigned), then, once WordPress is fully set up, rerun this script with --ssl-certbot. My apologies for the inconvenience, this will be improved in a future version.
+    msg: Tried to supply WordPress domain configuration via raw MySQL command. If this failed, it was because no tables exist, because WordPress has not been fully set up yet. Please complete the Famous 5 Minute WordPress Installation in your web browser, then run this playbook again. Make sure to do so over an encrypted connection, that is via HTTPS!
 
 - pause:
     seconds: 5
```

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2` & `lampsible-0.12.0/src/lampsible/project/roles/fail2ban/templates/jail.local.j2`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/mysql/tasks/main.yml` & `lampsible-0.12.0/src/lampsible/project/roles/mysql/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/php/tasks/main.yml` & `lampsible-0.12.0/src/lampsible/project/roles/php/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf` & `lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/apache2.conf`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini` & `lampsible-0.12.0/src/lampsible/project/roles/phpmyadmin/templates/php.ini`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml` & `lampsible-0.12.0/src/lampsible/project/roles/ssl-selfsigned/tasks/main.yml`

 * *Files 14% similar despite different names*

```diff
@@ -26,16 +26,11 @@
     privatekey_path: /etc/ssl/private/selfsigned.key
     csr_path: /etc/ssl/csr/selfsigned.csr
     provider: selfsigned
 
 - name: Create Diffie-Hellman group for forward secrecy
   raw: openssl dhparam -out /etc/ssl/certs/dhparam.pem 2048
 
-- name: Enable Apache module SSL
-  raw: a2enmod ssl
-- name: Enable Apache module headers
-  raw: a2enmod headers
-
 - name: Restart Apache
   service:
     name: apache2
     state: reloaded
```

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/wordpress/tasks/main.yml` & `lampsible-0.12.0/src/lampsible/project/roles/wordpress/tasks/main.yml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # dealing with WordPress. It is particularly challenging that WordPress needs
 # to be 'installed' by the user by submitting the usual '5 Minute Install'
 # form, that is, HTML form via HTTP... But maybe the options that WordPress
 # expects from that form submission can also somehow be supplied via
 # Ansible parameters... This would solve a lot of problems!
 #################################################################
 
-- name: Download Wordpress
+- name: Download WordPress
   unarchive:
     src: "https://wordpress.org/wordpress-{{ wordpress_version }}.tar.gz"
     dest: "/var/www/html/"
     remote_src: yes
 
 - name: Create WordPress database
   community.mysql.mysql_db:
```

### Comparing `lampsible-0.11.0/src/lampsible/project/roles/wordpress/templates/.htaccess` & `lampsible-0.12.0/src/lampsible/project/roles/wordpress/templates/.htaccess`

 * *Files identical despite different names*

### Comparing `lampsible-0.11.0/src/lampsible/project/wordpress.yml` & `lampsible-0.12.0/src/lampsible/project/wordpress.yml`

 * *Files 20% similar despite different names*

```diff
@@ -15,36 +15,35 @@
         - wordpress
 
     - name: Conditionally include SSL role
       include_role:
         name: ssl-selfsigned
       when: ssl_selfsigned
 
-    # TODO
+    # It's important that this runs after the selfsigned certificates,
+    # if those are being used, but before Certbot, if that's being used.
+    - name: Include Apache virtual host role
+      include_role:
+        name: apache-vhosts
+
     - name: Conditionally include SSL role
       include_role:
         name: ssl-certbot
       when: ssl_certbot
 
-    # TODO: This only works if WordPress has been finished setting up
-    # via the manual "5 minute install", because otherwise, the database
-    # table that this role tries to update wouldn't exist.
-    # So to fully install WordPress, you have to install it first without
-    # --ssl-certbot - but absolutely with --ssl-selfsigned, because you're sending
-    # credentials over the network! - then, when that's taken care of, run the
-    # script once again with --ssl-certbot.
+    - pause:
+        seconds: "{{ wordpress_5_minute_install_seconds }}"
+        prompt: "Please navigate to your site right now to complete the 'Famous 5 Minute WordPress Installation'. This is required for the next step of the script to suceed (setting some configurations in the database), and it's also important for security reasons that you do this right away. You have exactly {{ wordpress_5_minute_install_seconds }} seconds to complete this step."
+      when: ssl_certbot
+
     - name: Conditionally include WordPress domain configuration - needed for SSL
       include_role:
         name: domain-for-wordpress
       when: ssl_certbot
 
-    - name: Include Apache virtual host role
-      include_role:
-        name: apache-vhosts
-
     - name: Conditionally include custom Apache configuration
       include_role:
         name: apache-conf
       when: ssl_selfsigned
 
     - name: Conditionally include fail2ban role
       include_role:
```

### Comparing `lampsible-0.11.0/src/lampsible.egg-info/SOURCES.txt` & `lampsible-0.12.0/src/lampsible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

