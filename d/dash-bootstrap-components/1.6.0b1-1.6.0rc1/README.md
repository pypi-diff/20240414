# Comparing `tmp/dash-bootstrap-components-1.6.0b1.tar.gz` & `tmp/dash_bootstrap_components-1.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-bootstrap-components-1.6.0b1.tar", last modified: Wed Feb  7 23:02:04 2024, max compression
+gzip compressed data, was "dash_bootstrap_components-1.6.0rc1.tar", last modified: Sun Apr 14 18:11:43 2024, max compression
```

## Comparing `dash-bootstrap-components-1.6.0b1.tar` & `dash_bootstrap_components-1.6.0rc1.tar`

### file list

```diff
@@ -1,100 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:02:04.625978 dash-bootstrap-components-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-07 23:02:04.625978 dash-bootstrap-components-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:02:04.605977 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:02:04.621977 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/
--rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Accordion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/AccordionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Breadcrumb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Button.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ButtonGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardFooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardImg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardImgOverlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Carousel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Checklist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Col.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/DropdownMenu.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/DropdownMenuItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Fade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/FormFeedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/FormFloating.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/FormText.py
--rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/InputGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/InputGroupText.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ListGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ListGroupItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Modal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalFooter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalTitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Nav.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavLink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Navbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavbarBrand.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavbarSimple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavbarToggler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Offcanvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Popover.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/PopoverBody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/PopoverHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/RadioButton.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/RadioItems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Row.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Tab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Tabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Textarea.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Toast.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   227416 2024-02-07 23:01:45.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   362451 2024-02-07 23:01:48.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_table.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/themes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:02:04.625978 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-02-07 23:02:04.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-02-07 23:02:04.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 23:02:04.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-07 23:02:04.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-07 23:02:04.000000 dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/landing-page.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-02-07 23:02:04.625978 dash-bootstrap-components-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 23:02:04.625978 dash-bootstrap-components-1.6.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_components_as_props.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_navlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_popover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_positional_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_tooltip.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-07 23:01:08.000000 dash-bootstrap-components-1.6.0b1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10706 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.261799 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     4722 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Accordion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/AccordionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Breadcrumb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ButtonGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardFooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImgOverlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Carousel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checklist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Col.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6043 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenuItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Fade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFeedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFloating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormText.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14945 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroupText.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroupItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Modal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalFooter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalTitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Nav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavLink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Navbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarBrand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarSimple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarToggler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Offcanvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Popover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverBody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioButton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioItems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6626 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Textarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   235048 2024-04-14 18:11:28.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   362389 2024-04-14 18:11:31.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 18:11:43.000000 dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/landing-page.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-14 18:11:43.281799 dash_bootstrap_components-1.6.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:11:43.277799 dash_bootstrap_components-1.6.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_components_as_props.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_navlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_popover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 18:10:52.000000 dash_bootstrap_components-1.6.0rc1/tests/test_xss_links.py
```

### Comparing `dash-bootstrap-components-1.6.0b1/LICENSE` & `dash_bootstrap_components-1.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/PKG-INFO` & `dash_bootstrap_components-1.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.6.0b1
+Version: 1.6.0rc1
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.0b1 Summary:
-Bootstrap themed components for use in Plotly Dash Home-page: https://dash-
-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.0rc1
+Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
+dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `dash-bootstrap-components-1.6.0b1/README.md` & `dash_bootstrap_components-1.6.0rc1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
   <a href="https://dash-bootstrap-components.opensource.faculty.ai/">
-    <img src="https://cdn.opensource.faculty.ai/dbc/assets/logo.svg" alt="dash-bootstrap-components logo" width="200" height="200">
+    <img src="./readme-images/logo.png" alt="dash-bootstrap-components logo" width="200" height="200">
   </a>
 </p>
 
 <h3 align="center">Dash Bootstrap Components</h3>
 
 <p align="center">
   Bootstrap components for Plotly Dash
@@ -79,52 +79,20 @@
 
 For more information on how to link local or external CSS, check out the
 [Dash documentation][dash-docs-external].
 
 ### Build the layout
 
 With CSS linked, you can start building your app's layout with our Bootstrap
-components. See our [_documentation_][docs-components] for a full list of
-available components, which include:
-
-#### Standard row and column-based layouts
+components. These include layout components for organising the content of your app on the page, as well as UI components like navbars, cards, alerts and many more.
 
 ![layout](./readme-images/layout.png)
 
----
-
-#### Cards
-
-![cards](./readme-images/cards.png)
-
----
-
-#### Tabs
-
-![tabs](./readme-images/tabs.png)
-
----
-
-#### Forms
-
-![forms](./readme-images/forms.png)
-
----
-
-#### Dropdown menus
-
-<img src="./readme-images/dropdown.png" width="200"/>
-
----
-
-#### Tooltips
-
-<img src="./readme-images/tooltips.png" width="400"/>
-
-... and many more.
+See our [_documentation_][docs-components] for a full list of available
+components.
 
 ## Contributing
 
 We welcome contributions to _dash-bootstrap-components_. If you find a bug or
 something is unclear please [submit a bug report][bug-report], if you have ideas
 for new features please feel free to make a [feature request][feature-request].
 
@@ -132,15 +100,15 @@
 [contributing guide][contribution-guide], which contains instructions on how to
 build and install _dash-bootstrap-components_ locally, how to check your code
 will pass our linting checks, and how to submit the pull request itself.
 
 ## Copyright and license
 
 Code and documentation is copyright [Faculty Science Ltd.][faculty]
-2018-2022, and released under the [Apache 2.0 license](./LICENSE)
+2018-2024, and released under the [Apache 2.0 license](./LICENSE)
 
 [dash-homepage]: https://dash.plotly.com/
 [dash-docs-external]: https://dash.plotly.com/external-resources
 [bootstrap-homepage]: https://getbootstrap.com/
 [dbc-repo]: https://github.com/facultyai/dash-bootstrap-components
 [reactstrap-homepage]: https://reactstrap.github.io/
 [docs-homepage]: https://dash-bootstrap-components.opensource.faculty.ai
```

#### html2text {}

```diff
@@ -21,34 +21,32 @@
 to be styled properly, you must link to a stylesheet yourself. For convenience,
 links to [BootstrapCDN][bootstrapcdn] for each theme are available through the
 `themes` module, which can be used as follows: ```python import dash import
 dash_bootstrap_components as dbc app = dash.Dash(external_stylesheets=
 [dbc.themes.BOOTSTRAP]) ``` For more information on how to link local or
 external CSS, check out the [Dash documentation][dash-docs-external]. ### Build
 the layout With CSS linked, you can start building your app's layout with our
-Bootstrap components. See our [_documentation_][docs-components] for a full
-list of available components, which include: #### Standard row and column-based
-layouts ![layout](./readme-images/layout.png) --- #### Cards ![cards](./readme-
-images/cards.png) --- #### Tabs ![tabs](./readme-images/tabs.png) --- ####
-Forms ![forms](./readme-images/forms.png) --- #### Dropdown menus [./readme-
-images/dropdown.png]--- #### Tooltips [./readme-images/tooltips.png]... and
-many more. ## Contributing We welcome contributions to _dash-bootstrap-
-components_. If you find a bug or something is unclear please [submit a bug
-report][bug-report], if you have ideas for new features please feel free to
-make a [feature request][feature-request]. If you would like to submit a pull
-request, please read our [contributing guide][contribution-guide], which
-contains instructions on how to build and install _dash-bootstrap-components_
-locally, how to check your code will pass our linting checks, and how to submit
-the pull request itself. ## Copyright and license Code and documentation is
-copyright [Faculty Science Ltd.][faculty] 2018-2022, and released under the
-[Apache 2.0 license](./LICENSE) [dash-homepage]: https://dash.plotly.com/
-[dash-docs-external]: https://dash.plotly.com/external-resources [bootstrap-
-homepage]: https://getbootstrap.com/ [dbc-repo]: https://github.com/facultyai/
-dash-bootstrap-components [reactstrap-homepage]: https://reactstrap.github.io/
-[docs-homepage]: https://dash-bootstrap-components.opensource.faculty.ai [docs-
+Bootstrap components. These include layout components for organising the
+content of your app on the page, as well as UI components like navbars, cards,
+alerts and many more. ![layout](./readme-images/layout.png) See our
+[_documentation_][docs-components] for a full list of available components. ##
+Contributing We welcome contributions to _dash-bootstrap-components_. If you
+find a bug or something is unclear please [submit a bug report][bug-report], if
+you have ideas for new features please feel free to make a [feature request]
+[feature-request]. If you would like to submit a pull request, please read our
+[contributing guide][contribution-guide], which contains instructions on how to
+build and install _dash-bootstrap-components_ locally, how to check your code
+will pass our linting checks, and how to submit the pull request itself. ##
+Copyright and license Code and documentation is copyright [Faculty Science
+Ltd.][faculty] 2018-2024, and released under the [Apache 2.0 license](./
+LICENSE) [dash-homepage]: https://dash.plotly.com/ [dash-docs-external]: https:
+//dash.plotly.com/external-resources [bootstrap-homepage]: https://
+getbootstrap.com/ [dbc-repo]: https://github.com/facultyai/dash-bootstrap-
+components [reactstrap-homepage]: https://reactstrap.github.io/ [docs-
+homepage]: https://dash-bootstrap-components.opensource.faculty.ai [docs-
 components]: https://dash-bootstrap-components.opensource.faculty.ai/l/
 components [bootstrapcdn]: https://www.bootstrapcdn.com/ [faculty]: https://
 faculty.ai [bug-report]: https://github.com/facultyai/dash-bootstrap-
 components/issues/new?template=bug.md [feature-request]: https://github.com/
 facultyai/dash-bootstrap-components/issues/new?template=feature.md
 [contribution-guide]: https://github.com/facultyai/dash-bootstrap-components/
 blob/main/.github/CONTRIBUTING.md
```

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/__init__.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Accordion.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Accordion.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/AccordionItem.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/AccordionItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Alert.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Alert.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Badge.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Badge.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Breadcrumb.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Breadcrumb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTO GENERATED FILE - DO NOT EDIT
 
 from dash.development.base_component import Component, _explicitize_args
 
 
 class Breadcrumb(Component):
     """A Breadcrumb component.
-Use breadcrumbs to create a navigation breadcrumb in your app.
+
 
 Keyword arguments:
 
 - id (string; optional):
     The ID of this component, used to identify dash components in
     callbacks. The ID needs to be unique across all of the components
     in an app.
```

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Button.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Button.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ButtonGroup.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ButtonGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Card.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Card.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardBody.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardBody.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardFooter.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardFooter.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardGroup.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardHeader.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardHeader.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardImg.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImg.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardImgOverlay.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardImgOverlay.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/CardLink.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/CardLink.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Carousel.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Carousel.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Checkbox.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checkbox.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Checklist.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Checklist.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Col.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Col.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Collapse.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Collapse.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Container.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Container.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/DropdownMenu.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenu.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/DropdownMenuItem.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/DropdownMenuItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Fade.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Fade.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Form.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Form.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/FormFeedback.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFeedback.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/FormFloating.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormFloating.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/FormText.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/FormText.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Input.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Input.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/InputGroup.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/InputGroupText.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/InputGroupText.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Label.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Label.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ListGroup.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ListGroupItem.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ListGroupItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Modal.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Modal.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalBody.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalBody.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalFooter.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalFooter.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalHeader.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalHeader.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/ModalTitle.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/ModalTitle.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Nav.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Nav.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavItem.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavItem.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavLink.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavLink.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Navbar.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Navbar.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavbarBrand.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarBrand.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavbarSimple.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarSimple.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/NavbarToggler.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/NavbarToggler.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Offcanvas.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Offcanvas.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Pagination.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Pagination.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Placeholder.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Placeholder.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Popover.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Popover.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/PopoverBody.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverBody.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/PopoverHeader.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/PopoverHeader.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Progress.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Progress.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/RadioButton.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioButton.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/RadioItems.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/RadioItems.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Row.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Row.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Select.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Select.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Spinner.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Spinner.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Stack.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Stack.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Switch.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Switch.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Tab.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tab.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Table.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Tabs.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tabs.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Textarea.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Textarea.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Toast.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Toast.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/Tooltip.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/Tooltip.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/__init__.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/dash_bootstrap_components.min.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,377 +1,368 @@
 /*! For license information please see dash_bootstrap_components.min.js.LICENSE.txt */
 (() => {
     var e = [e => {
             "use strict";
             e.exports = window.React
-        }, (e, t, n) => {
-            "use strict";
-            e.exports = n(17)
         }, (e, t) => {
             var n;
             ! function() {
                 "use strict";
                 var r = {}.hasOwnProperty;
 
                 function a() {
-                    for (var e = [], t = 0; t < arguments.length; t++) {
+                    for (var e = "", t = 0; t < arguments.length; t++) {
                         var n = arguments[t];
-                        if (n) {
-                            var s = typeof n;
-                            if ("string" === s || "number" === s) e.push(n);
-                            else if (Array.isArray(n)) {
-                                if (n.length) {
-                                    var o = a.apply(null, n);
-                                    o && e.push(o)
-                                }
-                            } else if ("object" === s) {
-                                if (n.toString !== Object.prototype.toString && !n.toString.toString().includes("[native code]")) {
-                                    e.push(n.toString());
-                                    continue
-                                }
-                                for (var i in n) r.call(n, i) && n[i] && e.push(i)
-                            }
-                        }
+                        n && (e = o(e, s(n)))
                     }
-                    return e.join(" ")
+                    return e
+                }
+
+                function s(e) {
+                    if ("string" == typeof e || "number" == typeof e) return e;
+                    if ("object" != typeof e) return "";
+                    if (Array.isArray(e)) return a.apply(null, e);
+                    if (e.toString !== Object.prototype.toString && !e.toString.toString().includes("[native code]")) return e.toString();
+                    var t = "";
+                    for (var n in e) r.call(e, n) && e[n] && (t = o(t, n));
+                    return t
+                }
+
+                function o(e, t) {
+                    return t ? e ? e + " " + t : e + t : e
                 }
                 e.exports ? (a.default = a, e.exports = a) : void 0 === (n = function() {
                     return a
                 }.apply(t, [])) || (e.exports = n)
             }()
         }, e => {
             "use strict";
             e.exports = function() {}
         }, (e, t, n) => {
-            var r = n(5).default;
+            var r = n(4).default;
 
             function a() {
                 "use strict";
                 e.exports = a = function() {
-                    return t
+                    return n
                 }, e.exports.__esModule = !0, e.exports.default = e.exports;
-                var t = {},
-                    n = Object.prototype,
-                    s = n.hasOwnProperty,
-                    o = Object.defineProperty || function(e, t, n) {
+                var t, n = {},
+                    s = Object.prototype,
+                    o = s.hasOwnProperty,
+                    i = Object.defineProperty || function(e, t, n) {
                         e[t] = n.value
                     },
-                    i = "function" == typeof Symbol ? Symbol : {},
-                    l = i.iterator || "@@iterator",
-                    c = i.asyncIterator || "@@asyncIterator",
-                    u = i.toStringTag || "@@toStringTag";
+                    l = "function" == typeof Symbol ? Symbol : {},
+                    c = l.iterator || "@@iterator",
+                    u = l.asyncIterator || "@@asyncIterator",
+                    d = l.toStringTag || "@@toStringTag";
 
-                function d(e, t, n) {
+                function p(e, t, n) {
                     return Object.defineProperty(e, t, {
                         value: n,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
                     }), e[t]
                 }
                 try {
-                    d({}, "")
-                } catch (e) {
-                    d = function(e, t, n) {
+                    p({}, "")
+                } catch (t) {
+                    p = function(e, t, n) {
                         return e[t] = n
                     }
                 }
 
-                function p(e, t, n, r) {
-                    var a = t && t.prototype instanceof g ? t : g,
+                function f(e, t, n, r) {
+                    var a = t && t.prototype instanceof _ ? t : _,
                         s = Object.create(a.prototype),
-                        i = new P(r || []);
-                    return o(s, "_invoke", {
-                        value: N(e, n, i)
+                        o = new D(r || []);
+                    return i(s, "_invoke", {
+                        value: C(e, n, o)
                     }), s
                 }
 
-                function f(e, t, n) {
+                function m(e, t, n) {
                     try {
                         return {
                             type: "normal",
                             arg: e.call(t, n)
                         }
                     } catch (e) {
                         return {
                             type: "throw",
                             arg: e
                         }
                     }
                 }
-                t.wrap = p;
-                var m = {};
-
-                function g() {}
-
-                function b() {}
-
-                function y() {}
-                var h = {};
-                d(h, l, (function() {
+                n.wrap = f;
+                var g = "suspendedStart",
+                    b = "suspendedYield",
+                    y = "executing",
+                    h = "completed",
+                    v = {};
+
+                function _() {}
+
+                function x() {}
+
+                function O() {}
+                var w = {};
+                p(w, c, (function() {
                     return this
                 }));
-                var v = Object.getPrototypeOf,
-                    _ = v && v(v(C([])));
-                _ && _ !== n && s.call(_, l) && (h = _);
-                var x = y.prototype = g.prototype = Object.create(h);
+                var N = Object.getPrototypeOf,
+                    E = N && N(N(L([])));
+                E && E !== s && o.call(E, c) && (w = E);
+                var j = O.prototype = _.prototype = Object.create(w);
 
-                function O(e) {
+                function k(e) {
                     ["next", "throw", "return"].forEach((function(t) {
-                        d(e, t, (function(e) {
+                        p(e, t, (function(e) {
                             return this._invoke(t, e)
                         }))
                     }))
                 }
 
-                function w(e, t) {
-                    function n(a, o, i, l) {
-                        var c = f(e[a], e, o);
+                function P(e, t) {
+                    function n(a, s, i, l) {
+                        var c = m(e[a], e, s);
                         if ("throw" !== c.type) {
                             var u = c.arg,
                                 d = u.value;
-                            return d && "object" == r(d) && s.call(d, "__await") ? t.resolve(d.__await).then((function(e) {
+                            return d && "object" == r(d) && o.call(d, "__await") ? t.resolve(d.__await).then((function(e) {
                                 n("next", e, i, l)
                             }), (function(e) {
                                 n("throw", e, i, l)
                             })) : t.resolve(d).then((function(e) {
                                 u.value = e, i(u)
                             }), (function(e) {
                                 return n("throw", e, i, l)
                             }))
                         }
                         l(c.arg)
                     }
                     var a;
-                    o(this, "_invoke", {
+                    i(this, "_invoke", {
                         value: function(e, r) {
                             function s() {
                                 return new t((function(t, a) {
                                     n(e, r, t, a)
                                 }))
                             }
                             return a = a ? a.then(s, s) : s()
                         }
                     })
                 }
 
-                function N(e, t, n) {
-                    var r = "suspendedStart";
-                    return function(a, s) {
-                        if ("executing" === r) throw new Error("Generator is already running");
-                        if ("completed" === r) {
-                            if ("throw" === a) throw s;
+                function C(e, n, r) {
+                    var a = g;
+                    return function(s, o) {
+                        if (a === y) throw Error("Generator is already running");
+                        if (a === h) {
+                            if ("throw" === s) throw o;
                             return {
-                                value: void 0,
+                                value: t,
                                 done: !0
                             }
                         }
-                        for (n.method = a, n.arg = s;;) {
-                            var o = n.delegate;
-                            if (o) {
-                                var i = E(o, n);
-                                if (i) {
-                                    if (i === m) continue;
-                                    return i
+                        for (r.method = s, r.arg = o;;) {
+                            var i = r.delegate;
+                            if (i) {
+                                var l = T(i, r);
+                                if (l) {
+                                    if (l === v) continue;
+                                    return l
                                 }
                             }
-                            if ("next" === n.method) n.sent = n._sent = n.arg;
-                            else if ("throw" === n.method) {
-                                if ("suspendedStart" === r) throw r = "completed", n.arg;
-                                n.dispatchException(n.arg)
-                            } else "return" === n.method && n.abrupt("return", n.arg);
-                            r = "executing";
-                            var l = f(e, t, n);
-                            if ("normal" === l.type) {
-                                if (r = n.done ? "completed" : "suspendedYield", l.arg === m) continue;
+                            if ("next" === r.method) r.sent = r._sent = r.arg;
+                            else if ("throw" === r.method) {
+                                if (a === g) throw a = h, r.arg;
+                                r.dispatchException(r.arg)
+                            } else "return" === r.method && r.abrupt("return", r.arg);
+                            a = y;
+                            var c = m(e, n, r);
+                            if ("normal" === c.type) {
+                                if (a = r.done ? h : b, c.arg === v) continue;
                                 return {
-                                    value: l.arg,
-                                    done: n.done
+                                    value: c.arg,
+                                    done: r.done
                                 }
                             }
-                            "throw" === l.type && (r = "completed", n.method = "throw", n.arg = l.arg)
+                            "throw" === c.type && (a = h, r.method = "throw", r.arg = c.arg)
                         }
                     }
                 }
 
-                function E(e, t) {
-                    var n = t.method,
-                        r = e.iterator[n];
-                    if (void 0 === r) return t.delegate = null, "throw" === n && e.iterator.return && (t.method = "return", t.arg = void 0, E(e, t), "throw" === t.method) || "return" !== n && (t.method = "throw", t.arg = new TypeError("The iterator does not provide a '" + n + "' method")), m;
-                    var a = f(r, e.iterator, t.arg);
-                    if ("throw" === a.type) return t.method = "throw", t.arg = a.arg, t.delegate = null, m;
-                    var s = a.arg;
-                    return s ? s.done ? (t[e.resultName] = s.value, t.next = e.nextLoc, "return" !== t.method && (t.method = "next", t.arg = void 0), t.delegate = null, m) : s : (t.method = "throw", t.arg = new TypeError("iterator result is not an object"), t.delegate = null, m)
+                function T(e, n) {
+                    var r = n.method,
+                        a = e.iterator[r];
+                    if (a === t) return n.delegate = null, "throw" === r && e.iterator.return && (n.method = "return", n.arg = t, T(e, n), "throw" === n.method) || "return" !== r && (n.method = "throw", n.arg = new TypeError("The iterator does not provide a '" + r + "' method")), v;
+                    var s = m(a, e.iterator, n.arg);
+                    if ("throw" === s.type) return n.method = "throw", n.arg = s.arg, n.delegate = null, v;
+                    var o = s.arg;
+                    return o ? o.done ? (n[e.resultName] = o.value, n.next = e.nextLoc, "return" !== n.method && (n.method = "next", n.arg = t), n.delegate = null, v) : o : (n.method = "throw", n.arg = new TypeError("iterator result is not an object"), n.delegate = null, v)
                 }
 
-                function j(e) {
+                function S(e) {
                     var t = {
                         tryLoc: e[0]
                     };
                     1 in e && (t.catchLoc = e[1]), 2 in e && (t.finallyLoc = e[2], t.afterLoc = e[3]), this.tryEntries.push(t)
                 }
 
-                function k(e) {
+                function R(e) {
                     var t = e.completion || {};
                     t.type = "normal", delete t.arg, e.completion = t
                 }
 
-                function P(e) {
+                function D(e) {
                     this.tryEntries = [{
                         tryLoc: "root"
-                    }], e.forEach(j, this), this.reset(!0)
+                    }], e.forEach(S, this), this.reset(!0)
                 }
 
-                function C(e) {
-                    if (e) {
-                        var t = e[l];
-                        if (t) return t.call(e);
+                function L(e) {
+                    if (e || "" === e) {
+                        var n = e[c];
+                        if (n) return n.call(e);
                         if ("function" == typeof e.next) return e;
                         if (!isNaN(e.length)) {
-                            var n = -1,
-                                r = function t() {
-                                    for (; ++n < e.length;)
-                                        if (s.call(e, n)) return t.value = e[n], t.done = !1, t;
-                                    return t.value = void 0, t.done = !0, t
+                            var a = -1,
+                                s = function n() {
+                                    for (; ++a < e.length;)
+                                        if (o.call(e, a)) return n.value = e[a], n.done = !1, n;
+                                    return n.value = t, n.done = !0, n
                                 };
-                            return r.next = r
+                            return s.next = s
                         }
                     }
-                    return {
-                        next: T
-                    }
-                }
-
-                function T() {
-                    return {
-                        value: void 0,
-                        done: !0
-                    }
+                    throw new TypeError(r(e) + " is not iterable")
                 }
-                return b.prototype = y, o(x, "constructor", {
-                    value: y,
+                return x.prototype = O, i(j, "constructor", {
+                    value: O,
                     configurable: !0
-                }), o(y, "constructor", {
-                    value: b,
+                }), i(O, "constructor", {
+                    value: x,
                     configurable: !0
-                }), b.displayName = d(y, u, "GeneratorFunction"), t.isGeneratorFunction = function(e) {
+                }), x.displayName = p(O, d, "GeneratorFunction"), n.isGeneratorFunction = function(e) {
                     var t = "function" == typeof e && e.constructor;
-                    return !!t && (t === b || "GeneratorFunction" === (t.displayName || t.name))
-                }, t.mark = function(e) {
-                    return Object.setPrototypeOf ? Object.setPrototypeOf(e, y) : (e.__proto__ = y, d(e, u, "GeneratorFunction")), e.prototype = Object.create(x), e
-                }, t.awrap = function(e) {
+                    return !!t && (t === x || "GeneratorFunction" === (t.displayName || t.name))
+                }, n.mark = function(e) {
+                    return Object.setPrototypeOf ? Object.setPrototypeOf(e, O) : (e.__proto__ = O, p(e, d, "GeneratorFunction")), e.prototype = Object.create(j), e
+                }, n.awrap = function(e) {
                     return {
                         __await: e
                     }
-                }, O(w.prototype), d(w.prototype, c, (function() {
+                }, k(P.prototype), p(P.prototype, u, (function() {
                     return this
-                })), t.AsyncIterator = w, t.async = function(e, n, r, a, s) {
+                })), n.AsyncIterator = P, n.async = function(e, t, r, a, s) {
                     void 0 === s && (s = Promise);
-                    var o = new w(p(e, n, r, a), s);
-                    return t.isGeneratorFunction(n) ? o : o.next().then((function(e) {
+                    var o = new P(f(e, t, r, a), s);
+                    return n.isGeneratorFunction(t) ? o : o.next().then((function(e) {
                         return e.done ? e.value : o.next()
                     }))
-                }, O(x), d(x, u, "Generator"), d(x, l, (function() {
+                }, k(j), p(j, d, "Generator"), p(j, c, (function() {
                     return this
-                })), d(x, "toString", (function() {
+                })), p(j, "toString", (function() {
                     return "[object Generator]"
-                })), t.keys = function(e) {
+                })), n.keys = function(e) {
                     var t = Object(e),
                         n = [];
                     for (var r in t) n.push(r);
                     return n.reverse(),
                         function e() {
                             for (; n.length;) {
                                 var r = n.pop();
                                 if (r in t) return e.value = r, e.done = !1, e
                             }
                             return e.done = !0, e
                         }
-                }, t.values = C, P.prototype = {
-                    constructor: P,
+                }, n.values = L, D.prototype = {
+                    constructor: D,
                     reset: function(e) {
-                        if (this.prev = 0, this.next = 0, this.sent = this._sent = void 0, this.done = !1, this.delegate = null, this.method = "next", this.arg = void 0, this.tryEntries.forEach(k), !e)
-                            for (var t in this) "t" === t.charAt(0) && s.call(this, t) && !isNaN(+t.slice(1)) && (this[t] = void 0)
+                        if (this.prev = 0, this.next = 0, this.sent = this._sent = t, this.done = !1, this.delegate = null, this.method = "next", this.arg = t, this.tryEntries.forEach(R), !e)
+                            for (var n in this) "t" === n.charAt(0) && o.call(this, n) && !isNaN(+n.slice(1)) && (this[n] = t)
                     },
                     stop: function() {
                         this.done = !0;
                         var e = this.tryEntries[0].completion;
                         if ("throw" === e.type) throw e.arg;
                         return this.rval
                     },
                     dispatchException: function(e) {
                         if (this.done) throw e;
-                        var t = this;
+                        var n = this;
 
-                        function n(n, r) {
-                            return o.type = "throw", o.arg = e, t.next = n, r && (t.method = "next", t.arg = void 0), !!r
+                        function r(r, a) {
+                            return i.type = "throw", i.arg = e, n.next = r, a && (n.method = "next", n.arg = t), !!a
                         }
-                        for (var r = this.tryEntries.length - 1; r >= 0; --r) {
-                            var a = this.tryEntries[r],
-                                o = a.completion;
-                            if ("root" === a.tryLoc) return n("end");
-                            if (a.tryLoc <= this.prev) {
-                                var i = s.call(a, "catchLoc"),
-                                    l = s.call(a, "finallyLoc");
-                                if (i && l) {
-                                    if (this.prev < a.catchLoc) return n(a.catchLoc, !0);
-                                    if (this.prev < a.finallyLoc) return n(a.finallyLoc)
-                                } else if (i) {
-                                    if (this.prev < a.catchLoc) return n(a.catchLoc, !0)
+                        for (var a = this.tryEntries.length - 1; a >= 0; --a) {
+                            var s = this.tryEntries[a],
+                                i = s.completion;
+                            if ("root" === s.tryLoc) return r("end");
+                            if (s.tryLoc <= this.prev) {
+                                var l = o.call(s, "catchLoc"),
+                                    c = o.call(s, "finallyLoc");
+                                if (l && c) {
+                                    if (this.prev < s.catchLoc) return r(s.catchLoc, !0);
+                                    if (this.prev < s.finallyLoc) return r(s.finallyLoc)
+                                } else if (l) {
+                                    if (this.prev < s.catchLoc) return r(s.catchLoc, !0)
                                 } else {
-                                    if (!l) throw new Error("try statement without catch or finally");
-                                    if (this.prev < a.finallyLoc) return n(a.finallyLoc)
+                                    if (!c) throw Error("try statement without catch or finally");
+                                    if (this.prev < s.finallyLoc) return r(s.finallyLoc)
                                 }
                             }
                         }
                     },
                     abrupt: function(e, t) {
                         for (var n = this.tryEntries.length - 1; n >= 0; --n) {
                             var r = this.tryEntries[n];
-                            if (r.tryLoc <= this.prev && s.call(r, "finallyLoc") && this.prev < r.finallyLoc) {
+                            if (r.tryLoc <= this.prev && o.call(r, "finallyLoc") && this.prev < r.finallyLoc) {
                                 var a = r;
                                 break
                             }
                         }
                         a && ("break" === e || "continue" === e) && a.tryLoc <= t && t <= a.finallyLoc && (a = null);
-                        var o = a ? a.completion : {};
-                        return o.type = e, o.arg = t, a ? (this.method = "next", this.next = a.finallyLoc, m) : this.complete(o)
+                        var s = a ? a.completion : {};
+                        return s.type = e, s.arg = t, a ? (this.method = "next", this.next = a.finallyLoc, v) : this.complete(s)
                     },
                     complete: function(e, t) {
                         if ("throw" === e.type) throw e.arg;
-                        return "break" === e.type || "continue" === e.type ? this.next = e.arg : "return" === e.type ? (this.rval = this.arg = e.arg, this.method = "return", this.next = "end") : "normal" === e.type && t && (this.next = t), m
+                        return "break" === e.type || "continue" === e.type ? this.next = e.arg : "return" === e.type ? (this.rval = this.arg = e.arg, this.method = "return", this.next = "end") : "normal" === e.type && t && (this.next = t), v
                     },
                     finish: function(e) {
                         for (var t = this.tryEntries.length - 1; t >= 0; --t) {
                             var n = this.tryEntries[t];
-                            if (n.finallyLoc === e) return this.complete(n.completion, n.afterLoc), k(n), m
+                            if (n.finallyLoc === e) return this.complete(n.completion, n.afterLoc), R(n), v
                         }
                     },
                     catch: function(e) {
                         for (var t = this.tryEntries.length - 1; t >= 0; --t) {
                             var n = this.tryEntries[t];
                             if (n.tryLoc === e) {
                                 var r = n.completion;
                                 if ("throw" === r.type) {
                                     var a = r.arg;
-                                    k(n)
+                                    R(n)
                                 }
                                 return a
                             }
                         }
-                        throw new Error("illegal catch attempt")
+                        throw Error("illegal catch attempt")
                     },
-                    delegateYield: function(e, t, n) {
+                    delegateYield: function(e, n, r) {
                         return this.delegate = {
-                            iterator: C(e),
-                            resultName: t,
-                            nextLoc: n
-                        }, "next" === this.method && (this.arg = void 0), m
+                            iterator: L(e),
+                            resultName: n,
+                            nextLoc: r
+                        }, "next" === this.method && (this.arg = t), v
                     }
-                }, t
+                }, n
             }
             e.exports = a, e.exports.__esModule = !0, e.exports.default = e.exports
         }, e => {
             function t(n) {
                 return e.exports = t = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
@@ -408,15 +399,15 @@
                         if (null == a) {
                             var t = e.apply(void 0, n);
                             null != t && (a = t)
                         }
                     })), a
                 }))
             };
-            var r, a = (r = n(8)) && r.__esModule ? r : {
+            var r, a = (r = n(7)) && r.__esModule ? r : {
                 default: r
             };
             e.exports = t.default
         }, (e, t) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
@@ -429,15 +420,15 @@
                     return e.apply(void 0, [n, r, i, s, l].concat(u))
                 }
                 var n = t.bind(null, !1);
                 return n.isRequired = t.bind(null, !0), n
             }, e.exports = t.default
         }, (e, t, n) => {
             "use strict";
-            var r = n(10);
+            var r = n(9);
 
             function a() {}
 
             function s() {}
             s.resetWarningCache = a, e.exports = function() {
                 function e(e, t, n, a, s, o) {
                     if (o !== r) {
@@ -482,15 +473,15 @@
             "use strict";
             e.exports = function(e) {
                 if ("string" != typeof e) throw new TypeError("Expected a string");
                 return /^[a-z][a-z0-9+.-]*:/.test(e)
             }
         }, (e, t, n) => {
             "use strict";
-            var r = n(13);
+            var r = n(12);
             e.exports = function(e) {
                 var t = typeof e;
                 if ("string" === t) {
                     var n = e;
                     if (0 == (e = +e) && r(n)) return !1
                 } else if ("number" !== t) return !1;
                 return e - e < 1
@@ -661,21 +652,26 @@
                             }
                         }], null && c(t.prototype, null), n && c(t, n), Object.defineProperty(t, "prototype", {
                             writable: !1
                         }), e
                     }()
             }]))
         }, (e, t, n) => {
-            var r = n(4)();
+            var r = n(3)();
             e.exports = r;
             try {
                 regeneratorRuntime = r
             } catch (e) {
                 "object" == typeof globalThis ? globalThis.regeneratorRuntime = r : Function("r", "regeneratorRuntime = r")(r)
             }
+        }, (e, t, n) => {
+            e.exports = n(8)()
+        }, (e, t, n) => {
+            "use strict";
+            e.exports = n(18)
         }, , (e, t, n) => {
             "use strict";
             var r = n(0),
                 a = 60103;
             if (t.Fragment = 60107, "function" == typeof Symbol && Symbol.for) {
                 var s = Symbol.for;
                 a = s("react.element"), t.Fragment = s("react.fragment")
@@ -703,15 +699,40 @@
                     ref: u,
                     props: s,
                     _owner: o.current
                 }
             }
             t.jsx = c, t.jsxs = c
         }, (e, t, n) => {
-            e.exports = n(9)()
+            "use strict";
+            t.J = void 0;
+            var r = n(20);
+            t.J = function(e) {
+                if (!e) return r.BLANK_URL;
+                var t, n, a = e;
+                do {
+                    t = (a = (n = a, n.replace(r.ctrlCharactersRegex, "").replace(r.htmlEntitiesRegex, (function(e, t) {
+                        return String.fromCharCode(t)
+                    }))).replace(r.htmlCtrlEntityRegex, "").replace(r.ctrlCharactersRegex, "").trim()).match(r.ctrlCharactersRegex) || a.match(r.htmlEntitiesRegex) || a.match(r.htmlCtrlEntityRegex)
+                } while (t && t.length > 0);
+                var s = a;
+                if (!s) return r.BLANK_URL;
+                if (function(e) {
+                        return r.relativeFirstCharacters.indexOf(e[0]) > -1
+                    }(s)) return s;
+                var o = s.match(r.urlSchemeRegex);
+                if (!o) return s;
+                var i = o[0];
+                return r.invalidProtocolRegex.test(i) ? r.BLANK_URL : s
+            }
+        }, (e, t) => {
+            "use strict";
+            Object.defineProperty(t, "__esModule", {
+                value: !0
+            }), t.BLANK_URL = t.relativeFirstCharacters = t.urlSchemeRegex = t.ctrlCharactersRegex = t.htmlCtrlEntityRegex = t.htmlEntitiesRegex = t.invalidProtocolRegex = void 0, t.invalidProtocolRegex = /^([^\w]*)(javascript|data|vbscript)/im, t.htmlEntitiesRegex = /&#(\w+)(^\w|;)?/g, t.htmlCtrlEntityRegex = /&(newline|tab);/gi, t.ctrlCharactersRegex = /[\u0000-\u001F\u007F-\u009F\u2000-\u200D\uFEFF]/gim, t.urlSchemeRegex = /^.+(:|&colon;)/gim, t.relativeFirstCharacters = [".", "/"], t.BLANK_URL = "about:blank"
         }],
         t = {};
 
     function n(r) {
         var a = t[r];
         if (void 0 !== a) return a.exports;
         var s = t[r] = {
@@ -785,84 +806,84 @@
             if (Object.getOwnPropertySymbols) {
                 var o = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (a[n] = e[n])
             }
             return a
         }
         n.r(r), n.d(r, {
-            Accordion: () => He,
-            AccordionItem: () => qe,
-            Alert: () => St,
-            Badge: () => Vt,
+            Accordion: () => Ke,
+            AccordionItem: () => We,
+            Alert: () => Pt,
+            Badge: () => Wt,
             Breadcrumb: () => en,
             Button: () => sn,
             ButtonGroup: () => dn,
-            Card: () => Dn,
-            CardBody: () => In,
-            CardFooter: () => Fn,
-            CardGroup: () => Hn,
-            CardHeader: () => qn,
-            CardImg: () => Yn,
-            CardImgOverlay: () => Qn,
-            CardLink: () => tr,
-            Carousel: () => gr,
-            Checkbox: () => yr,
-            Checklist: () => na,
-            Col: () => da,
-            Collapse: () => ma,
-            Container: () => va,
-            DropdownMenu: () => xi,
-            DropdownMenuItem: () => Ni,
-            Fade: () => Ci,
-            Form: () => ll,
-            FormFeedback: () => dl,
-            FormFloating: () => ml,
-            FormText: () => vl,
-            Input: () => Cl,
-            InputGroup: () => $l,
-            InputGroupText: () => Ml,
-            Label: () => Vl,
-            ListGroup: () => ec,
-            ListGroupItem: () => sc,
-            Modal: () => Wc,
-            ModalBody: () => Gc,
-            ModalFooter: () => Qc,
-            ModalHeader: () => su,
-            ModalTitle: () => cu,
-            Nav: () => mu,
-            NavItem: () => sd,
-            NavLink: () => cd,
-            Navbar: () => Uu,
-            NavbarBrand: () => Gu,
-            NavbarSimple: () => nd,
-            NavbarToggler: () => Ju,
-            Offcanvas: () => pd,
-            Pagination: () => Ed,
-            Placeholder: () => Ld,
-            Popover: () => ip,
-            PopoverBody: () => up,
-            PopoverHeader: () => fp,
-            Progress: () => jp,
-            RadioButton: () => Rp,
-            RadioItems: () => Tp,
-            Row: () => Fp,
-            Select: () => Kp,
-            Spinner: () => Yp,
-            Stack: () => tf,
-            Switch: () => rf,
-            Tab: () => sf,
-            Table: () => Df,
-            Tabs: () => Pf,
-            Textarea: () => If,
-            Toast: () => Gf,
-            Tooltip: () => Jf
+            Card: () => Bn,
+            CardBody: () => Hn,
+            CardFooter: () => qn,
+            CardGroup: () => Jn,
+            CardHeader: () => er,
+            CardImg: () => rr,
+            CardImgOverlay: () => or,
+            CardLink: () => cr,
+            Carousel: () => wr,
+            Checkbox: () => Er,
+            Checklist: () => ua,
+            Col: () => va,
+            Collapse: () => Oa,
+            Container: () => ka,
+            DropdownMenu: () => $i,
+            DropdownMenuItem: () => Fi,
+            Fade: () => Hi,
+            Form: () => wl,
+            FormFeedback: () => jl,
+            FormFloating: () => Cl,
+            FormText: () => Ll,
+            Input: () => Ul,
+            InputGroup: () => Jl,
+            InputGroupText: () => ec,
+            Label: () => cc,
+            ListGroup: () => bc,
+            ListGroupItem: () => xc,
+            Modal: () => cu,
+            ModalBody: () => mu,
+            ModalFooter: () => vu,
+            ModalHeader: () => ju,
+            ModalTitle: () => Ru,
+            Nav: () => Au,
+            NavItem: () => Rd,
+            NavLink: () => Id,
+            Navbar: () => hd,
+            NavbarBrand: () => xd,
+            NavbarSimple: () => Cd,
+            NavbarToggler: () => Nd,
+            Offcanvas: () => Md,
+            Pagination: () => Qd,
+            Placeholder: () => ip,
+            Popover: () => Mp,
+            PopoverBody: () => Kp,
+            PopoverHeader: () => Wp,
+            Progress: () => af,
+            RadioButton: () => df,
+            RadioItems: () => cf,
+            Row: () => hf,
+            Select: () => xf,
+            Spinner: () => Pf,
+            Stack: () => Lf,
+            Switch: () => If,
+            Tab: () => Ff,
+            Table: () => pm,
+            Tabs: () => im,
+            Textarea: () => gm,
+            Toast: () => Pm,
+            Tooltip: () => Sm
         });
         var i = n(0),
             l = n.n(i),
-            c = n(18),
+            c = n(15),
             u = n.n(c);
 
         function d(e) {
             return null != e && "object" == typeof e && !0 === e["@@functional/placeholder"]
         }
 
         function p(e) {
@@ -890,15 +911,15 @@
             }
         }
         const m = f((function(e, t) {
             for (var n = {}, r = {}, a = 0, s = e.length; a < s;) r[e[a]] = 1, a += 1;
             for (var o in t) r.hasOwnProperty(o) || (n[o] = t[o]);
             return n
         }));
-        var g = n(2),
+        var g = n(1),
             b = n.n(g);
 
         function y(e) {
             return "default" + e.charAt(0).toUpperCase() + e.substr(1)
         }
 
         function h(e) {
@@ -935,188 +956,187 @@
                         }), [n])]
                     }(u, c, t[p]),
                     m = f[0],
                     g = f[1];
                 return e({}, d, ((o = {})[a] = m, o[p] = g, o))
             }), t)
         }
-        n(6);
-        var _ = n(1);
+        n(5);
+        var _ = n(16);
         const x = ["xxl", "xl", "lg", "md", "sm", "xs"],
-            O = "xs",
-            w = i.createContext({
+            O = i.createContext({
                 prefixes: {},
                 breakpoints: x,
-                minBreakpoint: O
+                minBreakpoint: "xs"
             }),
             {
-                Consumer: N,
-                Provider: E
-            } = w;
+                Consumer: w,
+                Provider: N
+            } = O;
 
-        function j(e, t) {
+        function E(e, t) {
             const {
                 prefixes: n
-            } = (0, i.useContext)(w);
+            } = (0, i.useContext)(O);
             return e || n[t] || t
         }
 
-        function k() {
+        function j() {
             const {
                 breakpoints: e
-            } = (0, i.useContext)(w);
+            } = (0, i.useContext)(O);
             return e
         }
 
-        function P() {
+        function k() {
             const {
                 minBreakpoint: e
-            } = (0, i.useContext)(w);
+            } = (0, i.useContext)(O);
             return e
         }
 
-        function C() {
+        function P() {
             const {
                 dir: e
-            } = (0, i.useContext)(w);
+            } = (0, i.useContext)(O);
             return "rtl" === e
         }
 
-        function T(e) {
+        function C(e) {
             return e && e.ownerDocument || document
         }
-        var S = /([A-Z])/g,
-            R = /^ms-/;
+        var T = /([A-Z])/g,
+            S = /^ms-/;
 
-        function D(e) {
+        function R(e) {
             return function(e) {
-                return e.replace(S, "-$1").toLowerCase()
-            }(e).replace(R, "-ms-")
+                return e.replace(T, "-$1").toLowerCase()
+            }(e).replace(S, "-ms-")
         }
-        var L = /^((translate|rotate|scale)(X|Y|Z|3d)?|matrix(3d)?|perspective|skew(X|Y)?)$/i;
-        const $ = function(e, t) {
+        var D = /^((translate|rotate|scale)(X|Y|Z|3d)?|matrix(3d)?|perspective|skew(X|Y)?)$/i;
+        const L = function(e, t) {
             var n = "",
                 r = "";
-            if ("string" == typeof t) return e.style.getPropertyValue(D(t)) || function(e, t) {
+            if ("string" == typeof t) return e.style.getPropertyValue(R(t)) || function(e, t) {
                 return function(e) {
-                    var t = T(e);
+                    var t = C(e);
                     return t && t.defaultView || window
                 }(e).getComputedStyle(e, t)
-            }(e).getPropertyValue(D(t));
+            }(e).getPropertyValue(R(t));
             Object.keys(t).forEach((function(a) {
                 var s = t[a];
                 s || 0 === s ? function(e) {
-                    return !(!e || !L.test(e))
-                }(a) ? r += a + "(" + s + ") " : n += D(a) + ": " + s + ";" : e.style.removeProperty(D(a))
+                    return !(!e || !D.test(e))
+                }(a) ? r += a + "(" + s + ") " : n += R(a) + ": " + s + ";" : e.style.removeProperty(R(a))
             })), r && (n += "transform: " + r + ";"), e.style.cssText += ";" + n
         };
 
-        function I(e, t) {
-            return I = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+        function $(e, t) {
+            return $ = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                 return e.__proto__ = t, e
-            }, I(e, t)
+            }, $(e, t)
         }
-        const A = window.ReactDOM;
-        var M = n.n(A);
+        const I = window.ReactDOM;
+        var A = n.n(I);
         const F = l().createContext(null);
-        var B = "unmounted",
-            z = "exited",
-            K = "entering",
-            H = "entered",
-            W = "exiting",
+        var M = "unmounted",
+            B = "exited",
+            z = "entering",
+            K = "entered",
+            H = "exiting",
             U = function(e) {
                 var t, n;
 
                 function r(t, n) {
                     var r;
                     r = e.call(this, t, n) || this;
                     var a, s = n && !n.isMounting ? t.enter : t.appear;
-                    return r.appearStatus = null, t.in ? s ? (a = z, r.appearStatus = K) : a = H : a = t.unmountOnExit || t.mountOnEnter ? B : z, r.state = {
+                    return r.appearStatus = null, t.in ? s ? (a = B, r.appearStatus = z) : a = K : a = t.unmountOnExit || t.mountOnEnter ? M : B, r.state = {
                         status: a
                     }, r.nextCallback = null, r
                 }
-                n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, I(t, n), r.getDerivedStateFromProps = function(e, t) {
-                    return e.in && t.status === B ? {
-                        status: z
+                n = e, (t = r).prototype = Object.create(n.prototype), t.prototype.constructor = t, $(t, n), r.getDerivedStateFromProps = function(e, t) {
+                    return e.in && t.status === M ? {
+                        status: B
                     } : null
                 };
                 var a = r.prototype;
                 return a.componentDidMount = function() {
                     this.updateStatus(!0, this.appearStatus)
                 }, a.componentDidUpdate = function(e) {
                     var t = null;
                     if (e !== this.props) {
                         var n = this.state.status;
-                        this.props.in ? n !== K && n !== H && (t = K) : n !== K && n !== H || (t = W)
+                        this.props.in ? n !== z && n !== K && (t = z) : n !== z && n !== K || (t = H)
                     }
                     this.updateStatus(!1, t)
                 }, a.componentWillUnmount = function() {
                     this.cancelNextCallback()
                 }, a.getTimeouts = function() {
                     var e, t, n, r = this.props.timeout;
                     return e = t = n = r, null != r && "number" != typeof r && (e = r.exit, t = r.enter, n = void 0 !== r.appear ? r.appear : t), {
                         exit: e,
                         enter: t,
                         appear: n
                     }
                 }, a.updateStatus = function(e, t) {
                     if (void 0 === e && (e = !1), null !== t)
-                        if (this.cancelNextCallback(), t === K) {
+                        if (this.cancelNextCallback(), t === z) {
                             if (this.props.unmountOnExit || this.props.mountOnEnter) {
-                                var n = this.props.nodeRef ? this.props.nodeRef.current : M().findDOMNode(this);
+                                var n = this.props.nodeRef ? this.props.nodeRef.current : A().findDOMNode(this);
                                 n && function(e) {
                                     e.scrollTop
                                 }(n)
                             }
                             this.performEnter(e)
                         } else this.performExit();
-                    else this.props.unmountOnExit && this.state.status === z && this.setState({
-                        status: B
+                    else this.props.unmountOnExit && this.state.status === B && this.setState({
+                        status: M
                     })
                 }, a.performEnter = function(e) {
                     var t = this,
                         n = this.props.enter,
                         r = this.context ? this.context.isMounting : e,
-                        a = this.props.nodeRef ? [r] : [M().findDOMNode(this), r],
+                        a = this.props.nodeRef ? [r] : [A().findDOMNode(this), r],
                         s = a[0],
                         o = a[1],
                         i = this.getTimeouts(),
                         l = r ? i.appear : i.enter;
                     e || n ? (this.props.onEnter(s, o), this.safeSetState({
-                        status: K
+                        status: z
                     }, (function() {
                         t.props.onEntering(s, o), t.onTransitionEnd(l, (function() {
                             t.safeSetState({
-                                status: H
+                                status: K
                             }, (function() {
                                 t.props.onEntered(s, o)
                             }))
                         }))
                     }))) : this.safeSetState({
-                        status: H
+                        status: K
                     }, (function() {
                         t.props.onEntered(s)
                     }))
                 }, a.performExit = function() {
                     var e = this,
                         t = this.props.exit,
                         n = this.getTimeouts(),
-                        r = this.props.nodeRef ? void 0 : M().findDOMNode(this);
+                        r = this.props.nodeRef ? void 0 : A().findDOMNode(this);
                     t ? (this.props.onExit(r), this.safeSetState({
-                        status: W
+                        status: H
                     }, (function() {
                         e.props.onExiting(r), e.onTransitionEnd(n.exit, (function() {
                             e.safeSetState({
-                                status: z
+                                status: B
                             }, (function() {
                                 e.props.onExited(r)
                             }))
                         }))
                     }))) : this.safeSetState({
-                        status: z
+                        status: B
                     }, (function() {
                         e.props.onExited(r)
                     }))
                 }, a.cancelNextCallback = function() {
                     null !== this.nextCallback && (this.nextCallback.cancel(), this.nextCallback = null)
                 }, a.safeSetState = function(e, t) {
                     t = this.setNextCallback(t), this.setState(e, t)
@@ -1126,191 +1146,187 @@
                     return this.nextCallback = function(r) {
                         n && (n = !1, t.nextCallback = null, e(r))
                     }, this.nextCallback.cancel = function() {
                         n = !1
                     }, this.nextCallback
                 }, a.onTransitionEnd = function(e, t) {
                     this.setNextCallback(t);
-                    var n = this.props.nodeRef ? this.props.nodeRef.current : M().findDOMNode(this),
+                    var n = this.props.nodeRef ? this.props.nodeRef.current : A().findDOMNode(this),
                         r = null == e && !this.props.addEndListener;
                     if (n && !r) {
                         if (this.props.addEndListener) {
                             var a = this.props.nodeRef ? [this.nextCallback] : [n, this.nextCallback],
                                 s = a[0],
                                 o = a[1];
                             this.props.addEndListener(s, o)
                         }
                         null != e && setTimeout(this.nextCallback, e)
                     } else setTimeout(this.nextCallback, 0)
                 }, a.render = function() {
                     var e = this.state.status;
-                    if (e === B) return null;
+                    if (e === M) return null;
                     var t = this.props,
                         n = t.children,
                         r = (t.in, t.mountOnEnter, t.unmountOnExit, t.appear, t.enter, t.exit, t.timeout, t.addEndListener, t.onEnter, t.onEntering, t.onEntered, t.onExit, t.onExiting, t.onExited, t.nodeRef, s(t, ["children", "in", "mountOnEnter", "unmountOnExit", "appear", "enter", "exit", "timeout", "addEndListener", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "nodeRef"]));
                     return l().createElement(F.Provider, {
                         value: null
                     }, "function" == typeof n ? n(e, r) : l().cloneElement(l().Children.only(n), r))
                 }, r
             }(l().Component);
 
-        function q() {}
+        function W() {}
         U.contextType = F, U.propTypes = {}, U.defaultProps = {
             in: !1,
             mountOnEnter: !1,
             unmountOnExit: !1,
             appear: !1,
             enter: !0,
             exit: !0,
-            onEnter: q,
-            onEntering: q,
-            onEntered: q,
-            onExit: q,
-            onExiting: q,
-            onExited: q
-        }, U.UNMOUNTED = B, U.EXITED = z, U.ENTERING = K, U.ENTERED = H, U.EXITING = W;
-        const V = U,
-            G = !("undefined" == typeof window || !window.document || !window.document.createElement);
-        var Y = !1,
-            X = !1;
+            onEnter: W,
+            onEntering: W,
+            onEntered: W,
+            onExit: W,
+            onExiting: W,
+            onExited: W
+        }, U.UNMOUNTED = M, U.EXITED = B, U.ENTERING = z, U.ENTERED = K, U.EXITING = H;
+        const q = U,
+            V = !("undefined" == typeof window || !window.document || !window.document.createElement);
+        var G = !1,
+            Y = !1;
         try {
-            var J = {
+            var X = {
                 get passive() {
-                    return Y = !0
+                    return G = !0
                 },
                 get once() {
-                    return X = Y = !0
+                    return Y = G = !0
                 }
             };
-            G && (window.addEventListener("test", J, J), window.removeEventListener("test", J, !0))
+            V && (window.addEventListener("test", X, X), window.removeEventListener("test", X, !0))
         } catch (e) {}
-        const Q = function(e, t, n, r) {
-                if (r && "boolean" != typeof r && !X) {
+        const J = function(e, t, n, r) {
+                if (r && "boolean" != typeof r && !Y) {
                     var a = r.once,
                         s = r.capture,
                         o = n;
-                    !X && a && (o = n.__once || function e(r) {
+                    !Y && a && (o = n.__once || function e(r) {
                         this.removeEventListener(t, e, s), n.call(this, r)
-                    }, n.__once = o), e.addEventListener(t, o, Y ? r : s)
+                    }, n.__once = o), e.addEventListener(t, o, G ? r : s)
                 }
                 e.addEventListener(t, n, r)
             },
-            Z = function(e, t, n, r) {
+            Q = function(e, t, n, r) {
                 var a = r && "boolean" != typeof r ? r.capture : r;
                 e.removeEventListener(t, n, a), n.__once && e.removeEventListener(t, n.__once, a)
             },
-            ee = function(e, t, n, r) {
-                return Q(e, t, n, r),
+            Z = function(e, t, n, r) {
+                return J(e, t, n, r),
                     function() {
-                        Z(e, t, n, r)
+                        Q(e, t, n, r)
                     }
             };
 
-        function te(e, t, n, r) {
+        function ee(e, t, n, r) {
             var a, s;
-            null == n && (s = -1 === (a = $(e, "transitionDuration") || "").indexOf("ms") ? 1e3 : 1, n = parseFloat(a) * s || 0);
+            null == n && (s = -1 === (a = L(e, "transitionDuration") || "").indexOf("ms") ? 1e3 : 1, n = parseFloat(a) * s || 0);
             var o = function(e, t, n) {
                     void 0 === n && (n = 5);
                     var r = !1,
                         a = setTimeout((function() {
                             r || function(e, t, n, r) {
                                 if (void 0 === n && (n = !1), void 0 === r && (r = !0), e) {
                                     var a = document.createEvent("HTMLEvents");
                                     a.initEvent("transitionend", n, r), e.dispatchEvent(a)
                                 }
                             }(e, 0, !0)
                         }), t + n),
-                        s = ee(e, "transitionend", (function() {
+                        s = Z(e, "transitionend", (function() {
                             r = !0
                         }), {
                             once: !0
                         });
                     return function() {
                         clearTimeout(a), s()
                     }
                 }(e, n, r),
-                i = ee(e, "transitionend", t);
+                i = Z(e, "transitionend", t);
             return function() {
                 o(), i()
             }
         }
 
-        function ne(e, t) {
-            const n = $(e, t) || "",
+        function te(e, t) {
+            const n = L(e, t) || "",
                 r = -1 === n.indexOf("ms") ? 1e3 : 1;
             return parseFloat(n) * r
         }
 
-        function re(e, t) {
-            const n = ne(e, "transitionDuration"),
-                r = ne(e, "transitionDelay"),
-                a = te(e, (n => {
+        function ne(e, t) {
+            const n = te(e, "transitionDuration"),
+                r = te(e, "transitionDelay"),
+                a = ee(e, (n => {
                     n.target === e && (a(), t(n))
                 }), n + r)
         }
-        const ae = function(...e) {
+        const re = function(...e) {
             return e.filter((e => null != e)).reduce(((e, t) => {
                 if ("function" != typeof t) throw new Error("Invalid Argument Type, must only provide functions, undefined, or null.");
                 return null === e ? t : function(...n) {
                     e.apply(this, n), t.apply(this, n)
                 }
             }), null)
         };
 
-        function se(e) {
+        function ae(e) {
             e.offsetHeight
         }
-        var oe = function(e) {
-            return e && "function" != typeof e ? function(t) {
+        const se = e => e && "function" != typeof e ? t => {
                 e.current = t
-            } : e
-        };
-        const ie = function(e, t) {
-            return (0, i.useMemo)((function() {
-                return function(e, t) {
-                    var n = oe(e),
-                        r = oe(t);
-                    return function(e) {
+            } : e,
+            oe = function(e, t) {
+                return (0, i.useMemo)((() => function(e, t) {
+                    const n = se(e),
+                        r = se(t);
+                    return e => {
                         n && n(e), r && r(e)
                     }
-                }(e, t)
-            }), [e, t])
-        };
+                }(e, t)), [e, t])
+            };
 
-        function le(e) {
-            return e && "setState" in e ? M().findDOMNode(e) : null != e ? e : null
+        function ie(e) {
+            return e && "setState" in e ? A().findDOMNode(e) : null != e ? e : null
         }
-        const ce = l().forwardRef((({
+        const le = l().forwardRef((({
                 onEnter: e,
                 onEntering: t,
                 onEntered: n,
                 onExit: r,
                 onExiting: a,
                 onExited: s,
                 addEndListener: o,
                 children: c,
                 childRef: u,
                 ...d
             }, p) => {
                 const f = (0, i.useRef)(null),
-                    m = ie(f, u),
+                    m = oe(f, u),
                     g = e => {
-                        m(le(e))
+                        m(ie(e))
                     },
                     b = e => t => {
                         e && f.current && e(f.current, t)
                     },
                     y = (0, i.useCallback)(b(e), [e]),
                     h = (0, i.useCallback)(b(t), [t]),
                     v = (0, i.useCallback)(b(n), [n]),
                     x = (0, i.useCallback)(b(r), [r]),
                     O = (0, i.useCallback)(b(a), [a]),
                     w = (0, i.useCallback)(b(s), [s]),
                     N = (0, i.useCallback)(b(o), [o]);
-                return (0, _.jsx)(V, {
+                return (0, _.jsx)(q, {
                     ref: p,
                     ...d,
                     onEnter: y,
                     onEntered: v,
                     onEntering: h,
                     onExit: x,
                     onExited: w,
@@ -1321,271 +1337,271 @@
                         ...t,
                         ref: g
                     }) : l().cloneElement(c, {
                         ref: g
                     })
                 })
             })),
-            ue = {
+            ce = {
                 height: ["marginTop", "marginBottom"],
                 width: ["marginLeft", "marginRight"]
             };
 
-        function de(e, t) {
+        function ue(e, t) {
             const n = t[`offset${e[0].toUpperCase()}${e.slice(1)}`],
-                r = ue[e];
-            return n + parseInt($(t, r[0]), 10) + parseInt($(t, r[1]), 10)
+                r = ce[e];
+            return n + parseInt(L(t, r[0]), 10) + parseInt(L(t, r[1]), 10)
         }
-        const pe = {
-                [z]: "collapse",
-                [W]: "collapsing",
-                [K]: "collapsing",
-                [H]: "collapse show"
-            },
-            fe = {
-                in: !1,
-                timeout: 300,
-                mountOnEnter: !1,
-                unmountOnExit: !1,
-                appear: !1,
-                getDimensionValue: de
+        const de = {
+                [B]: "collapse",
+                [H]: "collapsing",
+                [z]: "collapsing",
+                [K]: "collapse show"
             },
-            me = l().forwardRef((({
+            pe = l().forwardRef((({
                 onEnter: e,
                 onEntering: t,
                 onEntered: n,
                 onExit: r,
                 onExiting: a,
                 className: s,
                 children: o,
                 dimension: c = "height",
-                getDimensionValue: u = de,
-                ...d
-            }, p) => {
-                const f = "function" == typeof c ? c() : c,
-                    m = (0, i.useMemo)((() => ae((e => {
-                        e.style[f] = "0"
-                    }), e)), [f, e]),
-                    g = (0, i.useMemo)((() => ae((e => {
-                        const t = `scroll${f[0].toUpperCase()}${f.slice(1)}`;
-                        e.style[f] = `${e[t]}px`
-                    }), t)), [f, t]),
-                    y = (0, i.useMemo)((() => ae((e => {
-                        e.style[f] = null
-                    }), n)), [f, n]),
-                    h = (0, i.useMemo)((() => ae((e => {
-                        e.style[f] = `${u(f,e)}px`, se(e)
-                    }), r)), [r, u, f]),
-                    v = (0, i.useMemo)((() => ae((e => {
-                        e.style[f] = null
-                    }), a)), [f, a]);
-                return (0, _.jsx)(ce, {
-                    ref: p,
-                    addEndListener: re,
-                    ...d,
-                    "aria-expanded": d.role ? d.in : null,
-                    onEnter: m,
-                    onEntering: g,
-                    onEntered: y,
-                    onExit: h,
-                    onExiting: v,
+                in: u = !1,
+                timeout: d = 300,
+                mountOnEnter: p = !1,
+                unmountOnExit: f = !1,
+                appear: m = !1,
+                getDimensionValue: g = ue,
+                ...y
+            }, h) => {
+                const v = "function" == typeof c ? c() : c,
+                    x = (0, i.useMemo)((() => re((e => {
+                        e.style[v] = "0"
+                    }), e)), [v, e]),
+                    O = (0, i.useMemo)((() => re((e => {
+                        const t = `scroll${v[0].toUpperCase()}${v.slice(1)}`;
+                        e.style[v] = `${e[t]}px`
+                    }), t)), [v, t]),
+                    w = (0, i.useMemo)((() => re((e => {
+                        e.style[v] = null
+                    }), n)), [v, n]),
+                    N = (0, i.useMemo)((() => re((e => {
+                        e.style[v] = `${g(v,e)}px`, ae(e)
+                    }), r)), [r, g, v]),
+                    E = (0, i.useMemo)((() => re((e => {
+                        e.style[v] = null
+                    }), a)), [v, a]);
+                return (0, _.jsx)(le, {
+                    ref: h,
+                    addEndListener: ne,
+                    ...y,
+                    "aria-expanded": y.role ? u : null,
+                    onEnter: x,
+                    onEntering: O,
+                    onEntered: w,
+                    onExit: N,
+                    onExiting: E,
                     childRef: o.ref,
+                    in: u,
+                    timeout: d,
+                    mountOnEnter: p,
+                    unmountOnExit: f,
+                    appear: m,
                     children: (e, t) => l().cloneElement(o, {
                         ...t,
-                        className: b()(s, o.props.className, pe[e], "width" === f && "collapse-horizontal")
+                        className: b()(s, o.props.className, de[e], "width" === v && "collapse-horizontal")
                     })
                 })
             }));
-        me.defaultProps = fe;
-        const ge = me;
 
-        function be(e, t) {
+        function fe(e, t) {
             return Array.isArray(e) ? e.includes(t) : e === t
         }
-        const ye = i.createContext({});
-        ye.displayName = "AccordionContext";
-        const he = ye,
-            ve = i.forwardRef((({
+        const me = i.createContext({});
+        me.displayName = "AccordionContext";
+        const ge = me,
+            be = i.forwardRef((({
                 as: e = "div",
                 bsPrefix: t,
                 className: n,
                 children: r,
                 eventKey: a,
                 ...s
             }, o) => {
                 const {
                     activeEventKey: l
-                } = (0, i.useContext)(he);
-                return t = j(t, "accordion-collapse"), (0, _.jsx)(ge, {
+                } = (0, i.useContext)(ge);
+                return t = E(t, "accordion-collapse"), (0, _.jsx)(pe, {
                     ref: o,
-                    in: be(l, a),
+                    in: fe(l, a),
                     ...s,
                     className: b()(n, t),
                     children: (0, _.jsx)(e, {
                         children: i.Children.only(r)
                     })
                 })
             }));
-        ve.displayName = "AccordionCollapse";
-        const _e = ve,
-            xe = i.createContext({
+        be.displayName = "AccordionCollapse";
+        const ye = be,
+            he = i.createContext({
                 eventKey: ""
             });
-        xe.displayName = "AccordionItemContext";
-        const Oe = xe,
-            we = i.forwardRef((({
+        he.displayName = "AccordionItemContext";
+        const ve = he,
+            _e = i.forwardRef((({
                 as: e = "div",
                 bsPrefix: t,
                 className: n,
                 onEnter: r,
                 onEntering: a,
                 onEntered: s,
                 onExit: o,
                 onExiting: l,
                 onExited: c,
                 ...u
             }, d) => {
-                t = j(t, "accordion-body");
+                t = E(t, "accordion-body");
                 const {
                     eventKey: p
-                } = (0, i.useContext)(Oe);
-                return (0, _.jsx)(_e, {
+                } = (0, i.useContext)(ve);
+                return (0, _.jsx)(ye, {
                     eventKey: p,
                     onEnter: r,
                     onEntering: a,
                     onEntered: s,
                     onExit: o,
                     onExiting: l,
                     onExited: c,
                     children: (0, _.jsx)(e, {
                         ref: d,
                         ...u,
                         className: b()(n, t)
                     })
                 })
             }));
-        we.displayName = "AccordionBody";
-        const Ne = we,
-            Ee = i.forwardRef((({
+        _e.displayName = "AccordionBody";
+        const xe = _e,
+            Oe = i.forwardRef((({
                 as: e = "button",
                 bsPrefix: t,
                 className: n,
                 onClick: r,
                 ...a
             }, s) => {
-                t = j(t, "accordion-button");
+                t = E(t, "accordion-button");
                 const {
                     eventKey: o
-                } = (0, i.useContext)(Oe), l = function(e, t) {
+                } = (0, i.useContext)(ve), l = function(e, t) {
                     const {
                         activeEventKey: n,
                         onSelect: r,
                         alwaysOpen: a
-                    } = (0, i.useContext)(he);
+                    } = (0, i.useContext)(ge);
                     return s => {
                         let o = e === n ? null : e;
                         a && (o = Array.isArray(n) ? n.includes(e) ? n.filter((t => t !== e)) : [...n, e] : [e]), null == r || r(o, s), null == t || t(s)
                     }
                 }(o, r), {
                     activeEventKey: c
-                } = (0, i.useContext)(he);
+                } = (0, i.useContext)(ge);
                 return "button" === e && (a.type = "button"), (0, _.jsx)(e, {
                     ref: s,
                     onClick: l,
                     ...a,
                     "aria-expanded": Array.isArray(c) ? c.includes(o) : o === c,
-                    className: b()(n, t, !be(c, o) && "collapsed")
+                    className: b()(n, t, !fe(c, o) && "collapsed")
                 })
             }));
-        Ee.displayName = "AccordionButton";
-        const je = Ee,
-            ke = i.forwardRef((({
+        Oe.displayName = "AccordionButton";
+        const we = Oe,
+            Ne = i.forwardRef((({
                 as: e = "h2",
                 bsPrefix: t,
                 className: n,
                 children: r,
                 onClick: a,
                 ...s
-            }, o) => (t = j(t, "accordion-header"), (0, _.jsx)(e, {
+            }, o) => (t = E(t, "accordion-header"), (0, _.jsx)(e, {
                 ref: o,
                 ...s,
                 className: b()(n, t),
-                children: (0, _.jsx)(je, {
+                children: (0, _.jsx)(we, {
                     onClick: a,
                     children: r
                 })
             }))));
-        ke.displayName = "AccordionHeader";
-        const Pe = ke,
-            Ce = i.forwardRef((({
+        Ne.displayName = "AccordionHeader";
+        const Ee = Ne,
+            je = i.forwardRef((({
                 as: e = "div",
                 bsPrefix: t,
                 className: n,
                 eventKey: r,
                 ...a
             }, s) => {
-                t = j(t, "accordion-item");
+                t = E(t, "accordion-item");
                 const o = (0, i.useMemo)((() => ({
                     eventKey: r
                 })), [r]);
-                return (0, _.jsx)(Oe.Provider, {
+                return (0, _.jsx)(ve.Provider, {
                     value: o,
                     children: (0, _.jsx)(e, {
                         ref: s,
                         ...a,
                         className: b()(n, t)
                     })
                 })
             }));
-        Ce.displayName = "AccordionItem";
-        const Te = Ce,
-            Se = i.forwardRef(((e, t) => {
+        je.displayName = "AccordionItem";
+        const ke = je,
+            Pe = i.forwardRef(((e, t) => {
                 const {
                     as: n = "div",
                     activeKey: r,
                     bsPrefix: a,
                     className: s,
                     onSelect: o,
                     flush: l,
                     alwaysOpen: c,
                     ...u
                 } = v(e, {
                     activeKey: "onSelect"
-                }), d = j(a, "accordion"), p = (0, i.useMemo)((() => ({
+                }), d = E(a, "accordion"), p = (0, i.useMemo)((() => ({
                     activeEventKey: r,
                     onSelect: o,
                     alwaysOpen: c
                 })), [r, o, c]);
-                return (0, _.jsx)(he.Provider, {
+                return (0, _.jsx)(ge.Provider, {
                     value: p,
                     children: (0, _.jsx)(n, {
                         ref: t,
                         ...u,
                         className: b()(s, d, l && `${d}-flush`)
                     })
                 })
             }));
-        Se.displayName = "Accordion";
-        const Re = Object.assign(Se, {
-            Button: je,
-            Collapse: _e,
-            Item: Te,
-            Header: Pe,
-            Body: Ne
+        Pe.displayName = "Accordion";
+        const Ce = Object.assign(Pe, {
+            Button: we,
+            Collapse: ye,
+            Item: ke,
+            Header: Ee,
+            Body: xe
         });
 
-        function De(e) {
-            return De = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+        function Te(e) {
+            return Te = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                 return typeof e
             } : function(e) {
                 return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-            }, De(e)
+            }, Te(e)
         }
 
-        function Le(e, t) {
+        function Se(e, t) {
             return function(e) {
                 if (Array.isArray(e)) return e
             }(e) || function(e, t) {
                 var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                 if (null != n) {
                     var r, a, s, o, i = [],
                         l = !0,
@@ -1607,61 +1623,72 @@
                     }
                     return i
                 }
             }(e, t) || a(e, t) || function() {
                 throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
             }()
         }
-        const $e = p((function(e) {
+        const Re = p((function(e) {
             return null === e ? "Null" : void 0 === e ? "Undefined" : Object.prototype.toString.call(e).slice(8, -1)
         }));
-        var Ie = function(e) {
+        var De = n(19),
+            Le = function(e) {
                 return e && !Array.isArray(e) ? [e] : e
             },
-            Ae = function(e) {
+            $e = function(e) {
                 return e.props._dashprivate_layout && e.props._dashprivate_layout.props ? e.props._dashprivate_layout.props : e.props
             },
-            Me = function(e) {
-                return "Object" === $e(e) ? Object.entries(e).map((function(e) {
-                    var t = Le(e, 2),
+            Ie = function(e) {
+                return "Object" === Re(e) ? Object.entries(e).map((function(e) {
+                    var t = Se(e, 2),
                         n = t[0],
                         r = t[1];
                     return {
                         label: String(r),
                         value: n
                     }
-                })) : "Array" === $e(e) && e.length > 0 && ["String", "Number"].includes($e(e[0])) ? e.map((function(e) {
+                })) : "Array" === Re(e) && e.length > 0 && ["String", "Number"].includes(Re(e[0])) ? e.map((function(e) {
                     return {
                         label: String(e),
                         value: e
                     }
                 })) : e
             },
-            Fe = function(e) {
-                return "object" !== De(e) ? e : "{" + Object.keys(e).sort().map((function(t) {
+            Ae = function(e) {
+                return "object" !== Te(e) ? e : "{" + Object.keys(e).sort().map((function(t) {
                     return JSON.stringify(t) + ":" + ((n = e[t]) && n.wild || JSON.stringify(n));
                     var n
                 })).join(",") + "}"
             },
-            Be = l().createContext({}),
-            ze = ["children", "active_item", "always_open", "start_collapsed", "loading_state", "key", "setProps", "class_name", "className"],
-            Ke = function(n) {
+            Fe = function(e, t) {
+                var n = (0, i.useMemo)((function() {
+                    return e ? (0, De.J)(e) : void 0
+                }), [e]);
+                return (0, i.useEffect)((function() {
+                    n && n !== e && t({
+                        _dash_error: new Error("Dangerous link detected:: ".concat(e))
+                    })
+                }), [e, n]), n
+            },
+            Me = l().createContext({}),
+            Be = ["children", "active_item", "always_open", "start_collapsed", "loading_state", "key", "setProps", "class_name", "className"],
+            ze = function(n) {
                 var r = n.children,
                     s = n.active_item,
                     c = n.always_open,
                     u = n.start_collapsed,
                     d = n.loading_state,
                     p = n.key,
                     f = n.setProps,
                     g = n.class_name,
                     b = n.className,
-                    y = o(n, ze);
-                r = Ie(r), (0, i.useEffect)((function() {
+                    y = o(n, Be);
+                r = Le(r), (0, i.useEffect)((function() {
                     if (f && void 0 === s && !u) {
-                        var e = r && (Ae(r[0]).item_id || "item-0");
+                        var e = r && ($e(r[0]).item_id || "item-0");
                         f({
                             active_item: c ? [e] : e
                         })
                     }
                 }), []);
                 var h = function(e) {
                         var n, r;
@@ -1674,38 +1701,38 @@
                         }(r) || a(r) || function() {
                             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                         }()) : [e] : s !== e ? e : null, f({
                             active_item: n
                         }))
                     },
                     v = r && r.map((function(e, t) {
-                        var n = Ae(e).item_id || "item-".concat(t);
-                        return l().createElement(Be.Provider, {
+                        var n = $e(e).item_id || "item-".concat(t);
+                        return l().createElement(Me.Provider, {
                             key: n,
                             value: {
                                 toggle: h,
                                 idx: t
                             }
                         }, e)
                     }));
-                return l().createElement(Re, e({
+                return l().createElement(Ce, e({
                     key: p,
                     "data-dash-is-loading": d && d.is_loading || void 0,
                     activeKey: s,
                     defaultActiveKey: u ? null : s,
                     alwaysOpen: c,
                     className: g || b
                 }, m(["setProps", "persistence", "persistence_type", "persisted_props"], y)), v)
             };
-        Ke.defaultProps = {
+        ze.defaultProps = {
             persisted_props: ["active_item"],
             persistence_type: "local",
             start_collapsed: !1,
             always_open: !1
-        }, Ke.propTypes = {
+        }, ze.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             flush: u().bool,
@@ -1717,41 +1744,41 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["active_item"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const He = Ke;
-        var We = ["title", "item_id", "loading_state", "class_name", "className", "id", "children"],
+        const Ke = ze;
+        var He = ["title", "item_id", "loading_state", "class_name", "className", "id", "children"],
             Ue = function(t) {
                 var n = t.title,
                     r = t.item_id,
                     a = t.loading_state,
                     s = t.class_name,
                     c = t.className,
                     u = t.id,
                     d = t.children,
-                    p = o(t, We),
-                    f = (0, i.useContext)(Be),
+                    p = o(t, He),
+                    f = (0, i.useContext)(Me),
                     g = f.toggle,
                     b = f.idx,
                     y = r || "item-".concat(b);
-                return l().createElement(Re.Item, e({
-                    id: Fe(u),
+                return l().createElement(Ce.Item, e({
+                    id: Ae(u),
                     key: y,
                     eventKey: y,
                     className: s || c
                 }, m(["setProps", "persistence", "persistence_type", "persisted_props"], p), {
                     "data-dash-is-loading": a && a.is_loading || void 0
-                }), l().createElement(Re.Header, {
+                }), l().createElement(Ce.Header, {
                     onClick: function() {
                         g(y)
                     }
-                }, n), l().createElement(Re.Body, null, d))
+                }, n), l().createElement(Ce.Body, null, d))
             };
         Ue.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
@@ -1759,81 +1786,95 @@
             item_id: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const qe = Ue;
+        const We = Ue;
 
-        function Ve(e) {
+        function qe(e) {
             var t = function(e, t) {
-                if ("object" !== De(e) || null === e) return e;
+                if ("object" != Te(e) || !e) return e;
                 var n = e[Symbol.toPrimitive];
                 if (void 0 !== n) {
                     var r = n.call(e, "string");
-                    if ("object" !== De(r)) return r;
+                    if ("object" != Te(r)) return r;
                     throw new TypeError("@@toPrimitive must return a primitive value.")
                 }
                 return String(e)
             }(e);
-            return "symbol" === De(t) ? t : String(t)
+            return "symbol" == Te(t) ? t : t + ""
         }
 
-        function Ge(e, t, n) {
-            return (t = Ve(t)) in e ? Object.defineProperty(e, t, {
+        function Ve(e, t, n) {
+            return (t = qe(t)) in e ? Object.defineProperty(e, t, {
                 value: n,
                 enumerable: !0,
                 configurable: !0,
                 writable: !0
             }) : e[t] = n, e
         }
-        const Ye = function(e) {
-            var t = (0, i.useRef)(e);
-            return (0, i.useEffect)((function() {
+        const Ge = function(e) {
+            const t = (0, i.useRef)(e);
+            return (0, i.useEffect)((() => {
                 t.current = e
             }), [e]), t
         };
 
-        function Xe(e) {
-            var t = Ye(e);
-            return (0, i.useCallback)((function() {
-                return t.current && t.current.apply(t, arguments)
+        function Ye(e) {
+            const t = Ge(e);
+            return (0, i.useCallback)((function(...e) {
+                return t.current && t.current(...e)
             }), [t])
         }
+        const Xe = e => i.forwardRef(((t, n) => (0, _.jsx)("div", {
+                ...t,
+                ref: n,
+                className: b()(t.className, e)
+            }))),
+            Je = Xe("h4");
+        Je.displayName = "DivStyledAsH4";
+        const Qe = i.forwardRef((({
+            className: e,
+            bsPrefix: t,
+            as: n = Je,
+            ...r
+        }, a) => (t = E(t, "alert-heading"), (0, _.jsx)(n, {
+            ref: a,
+            className: b()(e, t),
+            ...r
+        }))));
+        Qe.displayName = "AlertHeading";
+        const Ze = Qe;
 
-        function Je() {
+        function et() {
             return (0, i.useState)(null)
         }
 
-        function Qe() {
-            var e = (0, i.useRef)(!0),
-                t = (0, i.useRef)((function() {
-                    return e.current
-                }));
-            return (0, i.useEffect)((function() {
-                return e.current = !0,
-                    function() {
-                        e.current = !1
-                    }
-            }), []), t.current
+        function tt() {
+            const e = (0, i.useRef)(!0),
+                t = (0, i.useRef)((() => e.current));
+            return (0, i.useEffect)((() => (e.current = !0, () => {
+                e.current = !1
+            })), []), t.current
         }
 
-        function Ze(e) {
-            var t = (0, i.useRef)(null);
-            return (0, i.useEffect)((function() {
+        function nt(e) {
+            const t = (0, i.useRef)(null);
+            return (0, i.useEffect)((() => {
                 t.current = e
             })), t.current
         }
-        var et = void 0 !== n.g && n.g.navigator && "ReactNative" === n.g.navigator.product;
-        const tt = "undefined" != typeof document || et ? i.useLayoutEffect : i.useEffect;
+        const rt = void 0 !== n.g && n.g.navigator && "ReactNative" === n.g.navigator.product,
+            at = "undefined" != typeof document || rt ? i.useLayoutEffect : i.useEffect;
         new WeakMap;
-        const nt = ["as", "disabled"];
+        const st = ["as", "disabled"];
 
-        function rt({
+        function ot({
             tagName: e,
             disabled: t,
             href: n,
             target: r,
             rel: a,
             role: s,
             onClick: o,
@@ -1863,279 +1904,247 @@
                 rel: "a" === e ? a : void 0,
                 onClick: u,
                 onKeyDown: e => {
                     " " === e.key && (e.preventDefault(), u(e))
                 }
             }, c]
         }
-        const at = i.forwardRef(((e, t) => {
+        const it = i.forwardRef(((e, t) => {
             let {
                 as: n,
                 disabled: r
             } = e, a = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, nt);
+            }(e, st);
             const [s, {
                 tagName: o
-            }] = rt(Object.assign({
+            }] = ot(Object.assign({
                 tagName: n,
                 disabled: r
             }, a));
             return (0, _.jsx)(o, Object.assign({}, a, s, {
                 ref: t
             }))
         }));
-        at.displayName = "Button";
-        const st = at,
-            ot = ["onKeyDown"],
-            it = i.forwardRef(((e, t) => {
+        it.displayName = "Button";
+        const lt = it,
+            ct = ["onKeyDown"],
+            ut = i.forwardRef(((e, t) => {
                 let {
                     onKeyDown: n
                 } = e, r = function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(e, ot);
-                const [a] = rt(Object.assign({
+                }(e, ct);
+                const [a] = ot(Object.assign({
                     tagName: "a"
-                }, r)), s = Xe((e => {
+                }, r)), s = Ye((e => {
                     a.onKeyDown(e), null == n || n(e)
                 }));
                 return (o = r.href) && "#" !== o.trim() && "button" !== r.role ? (0, _.jsx)("a", Object.assign({
                     ref: t
                 }, r, {
                     onKeyDown: n
                 })) : (0, _.jsx)("a", Object.assign({
                     ref: t
                 }, r, a, {
                     onKeyDown: s
                 }));
                 var o
             }));
-        it.displayName = "Anchor";
-        const lt = it,
-            ct = {
-                [K]: "show",
-                [H]: "show"
+        ut.displayName = "Anchor";
+        const dt = ut,
+            pt = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = dt,
+                ...r
+            }, a) => (t = E(t, "alert-link"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        pt.displayName = "AlertLink";
+        const ft = pt,
+            mt = {
+                [z]: "show",
+                [K]: "show"
             },
-            ut = i.forwardRef((({
+            gt = i.forwardRef((({
                 className: e,
                 children: t,
                 transitionClasses: n = {},
-                ...r
-            }, a) => {
-                const s = (0, i.useCallback)(((e, t) => {
-                    se(e), null == r.onEnter || r.onEnter(e, t)
-                }), [r]);
-                return (0, _.jsx)(ce, {
-                    ref: a,
-                    addEndListener: re,
-                    ...r,
-                    onEnter: s,
+                onEnter: r,
+                ...a
+            }, s) => {
+                const o = {
+                        in: !1,
+                        timeout: 300,
+                        mountOnEnter: !1,
+                        unmountOnExit: !1,
+                        appear: !1,
+                        ...a
+                    },
+                    l = (0, i.useCallback)(((e, t) => {
+                        ae(e), null == r || r(e, t)
+                    }), [r]);
+                return (0, _.jsx)(le, {
+                    ref: s,
+                    addEndListener: ne,
+                    ...o,
+                    onEnter: l,
                     childRef: t.ref,
                     children: (r, a) => i.cloneElement(t, {
                         ...a,
-                        className: b()("fade", e, t.props.className, ct[r], n[r])
+                        className: b()("fade", e, t.props.className, mt[r], n[r])
                     })
                 })
             }));
-        ut.defaultProps = {
-            in: !1,
-            timeout: 300,
-            mountOnEnter: !1,
-            unmountOnExit: !1,
-            appear: !1
-        }, ut.displayName = "Fade";
-        const dt = ut,
-            pt = {
+        gt.displayName = "Fade";
+        const bt = gt,
+            yt = {
                 "aria-label": u().string,
                 onClick: u().func,
                 variant: u().oneOf(["white"])
             },
-            ft = i.forwardRef((({
+            ht = i.forwardRef((({
                 className: e,
                 variant: t,
-                ...n
-            }, r) => (0, _.jsx)("button", {
-                ref: r,
+                "aria-label": n = "Close",
+                ...r
+            }, a) => (0, _.jsx)("button", {
+                ref: a,
                 type: "button",
                 className: b()("btn-close", t && `btn-close-${t}`, e),
-                ...n
-            })));
-        ft.displayName = "CloseButton", ft.propTypes = pt, ft.defaultProps = {
-            "aria-label": "Close"
-        };
-        const mt = ft,
-            gt = e => i.forwardRef(((t, n) => (0, _.jsx)("div", {
-                ...t,
-                ref: n,
-                className: b()(t.className, e)
+                "aria-label": n,
+                ...r
             })));
-        var bt = /-(.)/g;
-        const yt = e => {
-            return e[0].toUpperCase() + (t = e, t.replace(bt, (function(e, t) {
-                return t.toUpperCase()
-            }))).slice(1);
-            var t
-        };
-
-        function ht(e, {
-            displayName: t = yt(e),
-            Component: n,
-            defaultProps: r
-        } = {}) {
-            const a = i.forwardRef((({
-                className: t,
-                bsPrefix: r,
-                as: a = n || "div",
-                ...s
-            }, o) => {
-                const i = j(r, e);
-                return (0, _.jsx)(a, {
-                    ref: o,
-                    className: b()(t, i),
-                    ...s
-                })
-            }));
-            return a.defaultProps = r, a.displayName = t, a
-        }
-        const vt = gt("h4");
-        vt.displayName = "DivStyledAsH4";
-        const _t = ht("alert-heading", {
-                Component: vt
-            }),
-            xt = ht("alert-link", {
-                Component: lt
-            }),
-            Ot = {
-                variant: "primary",
-                show: !0,
-                transition: dt,
-                closeLabel: "Close alert"
-            },
-            wt = i.forwardRef(((e, t) => {
+        ht.displayName = "CloseButton", ht.propTypes = yt;
+        const vt = ht,
+            _t = i.forwardRef(((e, t) => {
                 const {
                     bsPrefix: n,
-                    show: r,
-                    closeLabel: a,
+                    show: r = !0,
+                    closeLabel: a = "Close alert",
                     closeVariant: s,
                     className: o,
                     children: i,
-                    variant: l,
+                    variant: l = "primary",
                     onClose: c,
                     dismissible: u,
-                    transition: d,
+                    transition: d = bt,
                     ...p
                 } = v(e, {
                     show: "onClose"
-                }), f = j(n, "alert"), m = Xe((e => {
+                }), f = E(n, "alert"), m = Ye((e => {
                     c && c(!1, e)
-                })), g = !0 === d ? dt : d, y = (0, _.jsxs)("div", {
+                })), g = !0 === d ? bt : d, y = (0, _.jsxs)("div", {
                     role: "alert",
                     ...g ? void 0 : p,
                     ref: t,
                     className: b()(o, f, l && `${f}-${l}`, u && `${f}-dismissible`),
-                    children: [u && (0, _.jsx)(mt, {
+                    children: [u && (0, _.jsx)(vt, {
                         onClick: m,
                         "aria-label": a,
                         variant: s
                     }), i]
                 });
                 return g ? (0, _.jsx)(g, {
                     unmountOnExit: !0,
                     ...p,
                     ref: void 0,
                     in: r,
                     children: y
                 }) : r ? y : null
             }));
-        wt.displayName = "Alert", wt.defaultProps = Ot;
-        const Nt = Object.assign(wt, {
-            Link: xt,
-            Heading: _t
+        _t.displayName = "Alert";
+        const xt = Object.assign(_t, {
+            Link: ft,
+            Heading: Ze
         });
-        var Et = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "white", "transparent"]),
-            jt = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "muted", "white", "black-50", "white-50"]),
-            kt = ["children", "dismissable", "duration", "is_open", "loading_state", "setProps", "color", "style", "class_name", "className", "fade"];
+        var Ot = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "white", "transparent"]),
+            wt = new Set(["primary", "secondary", "success", "danger", "warning", "info", "light", "dark", "muted", "white", "black-50", "white-50"]),
+            Nt = ["children", "dismissable", "duration", "is_open", "loading_state", "setProps", "color", "style", "class_name", "className", "fade"];
 
-        function Pt(e, t) {
+        function Et(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Ct(e) {
+        function jt(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Pt(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Pt(Object(n)).forEach((function(t) {
+                t % 2 ? Et(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Et(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Tt = function(t) {
+        var kt = function(t) {
             var n = t.children,
                 r = t.dismissable,
                 a = t.duration,
                 s = t.is_open,
                 c = t.loading_state,
                 u = t.setProps,
                 d = t.color,
                 p = t.style,
                 f = t.class_name,
                 g = t.className,
                 b = t.fade,
-                y = o(t, kt),
+                y = o(t, Nt),
                 h = (0, i.useRef)(null);
             (0, i.useEffect)((function() {
                 return a && (s ? h.current = setTimeout(v, a) : h.current && (clearTimeout(h.current), h.current = null)),
                     function() {
                         return clearTimeout(h.current)
                     }
             }), [s]);
             var v = function() {
                     u && u({
                         is_open: !1
                     })
                 },
-                _ = Et.has(d);
-            return l().createElement(Nt, e({
+                _ = Ot.has(d);
+            return l().createElement(xt, e({
                 show: s,
                 dismissible: r,
                 onClose: r ? v : null,
                 variant: _ ? d : null,
                 className: f || g,
                 transition: b,
-                style: _ ? p : Ct({
+                style: _ ? p : jt({
                     backgroundColor: d
                 }, p)
             }, m(["persistence", "persisted_props", "persistence_type", "setProps"], y), {
                 "data-dash-is-loading": c && c.is_loading || void 0
             }), n)
         };
-        Tt.defaultProps = {
+        kt.defaultProps = {
             color: "success",
             is_open: !0,
             duration: null,
             persisted_props: ["is_open"],
             persistence_type: "local"
-        }, Tt.propTypes = {
+        }, kt.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
@@ -2148,232 +2157,224 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["is_open"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const St = Tt,
-            Rt = i.forwardRef((({
+        const Pt = kt,
+            Ct = i.forwardRef((({
                 bsPrefix: e,
-                bg: t,
-                pill: n,
+                bg: t = "primary",
+                pill: n = !1,
                 text: r,
                 className: a,
                 as: s = "span",
                 ...o
             }, i) => {
-                const l = j(e, "badge");
+                const l = E(e, "badge");
                 return (0, _.jsx)(s, {
                     ref: i,
                     ...o,
                     className: b()(a, l, n && "rounded-pill", r && `text-${r}`, t && `bg-${t}`)
                 })
             }));
-        Rt.displayName = "Badge", Rt.defaultProps = {
-            bg: "primary",
-            pill: !1
-        };
-        const Dt = Rt;
+        Ct.displayName = "Badge";
+        const Tt = Ct;
 
-        function Lt(e, t) {
+        function St(e, t) {
             for (var n = 0; n < t.length; n++) {
                 var r = t[n];
-                r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, Ve(r.key), r)
+                r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, qe(r.key), r)
             }
         }
 
-        function $t(e) {
-            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-            return e
+        function Rt(e) {
+            return Rt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
+                return e.__proto__ || Object.getPrototypeOf(e)
+            }, Rt(e)
+        }
+        var Dt = n(10),
+            Lt = n.n(Dt),
+            $t = ["children", "external_link", "preOnClick", "target", "linkTarget", "href", "download"];
+
+        function It(e, t, n) {
+            return t = Rt(t),
+                function(e, t) {
+                    if (t && ("object" === Te(t) || "function" == typeof t)) return t;
+                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
+                    return function(e) {
+                        if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                        return e
+                    }(e)
+                }(e, At() ? Reflect.construct(t, n || [], Rt(e).constructor) : t.apply(e, n))
         }
 
-        function It(e) {
-            return It = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
-                return e.__proto__ || Object.getPrototypeOf(e)
-            }, It(e)
+        function At() {
+            try {
+                var e = !Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {})))
+            } catch (e) {}
+            return (At = function() {
+                return !!e
+            })()
         }
-        var At = n(11),
-            Mt = n.n(At),
-            Ft = ["children", "external_link", "preOnClick", "target", "linkTarget", "href", "download"];
 
-        function Bt(e, t) {
+        function Ft(e, t) {
             t = t || {
                 bubbles: !1,
                 cancelable: !1,
                 detail: void 0
             };
             var n = document.createEvent("CustomEvent");
             return n.initCustomEvent(e, t.bubbles, t.cancelable, t.detail), n
         }
 
-        function zt(e, t) {
-            return null == e ? Mt()(t) : e
+        function Mt(e, t) {
+            return null == e ? Lt()(t) : e
         }
-        Bt.prototype = window.Event.prototype;
-        var Kt = function(t) {
-            ! function(e, t) {
+        Ft.prototype = window.Event.prototype;
+        var Bt = function(t) {
+            function n(e) {
+                var t;
+                return function(e, t) {
+                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+                }(this, n), (t = It(this, n, [e])).updateLocation = t.updateLocation.bind(t), t
+            }
+            return function(e, t) {
                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                 e.prototype = Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
                         configurable: !0
                     }
                 }), Object.defineProperty(e, "prototype", {
                     writable: !1
-                }), t && I(e, t)
-            }(c, t);
-            var n, r, a, s, i = (a = c, s = function() {
-                if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                if (Reflect.construct.sham) return !1;
-                if ("function" == typeof Proxy) return !0;
-                try {
-                    return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                } catch (e) {
-                    return !1
-                }
-            }(), function() {
-                var e, t = It(a);
-                if (s) {
-                    var n = It(this).constructor;
-                    e = Reflect.construct(t, arguments, n)
-                } else e = t.apply(this, arguments);
-                return function(e, t) {
-                    if (t && ("object" === De(t) || "function" == typeof t)) return t;
-                    if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return $t(e)
-                }(this, e)
-            });
-
-            function c(e) {
-                var t;
-                return function(e, t) {
-                    if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                }(this, c), (t = i.call(this, e)).updateLocation = t.updateLocation.bind($t(t)), t
-            }
-            return n = c, (r = [{
+                }), t && $(e, t)
+            }(n, t), r = n, (a = [{
                 key: "updateLocation",
                 value: function(e) {
                     if (!(e.metaKey || e.shiftKey || e.altKey || e.ctrlKey))
                         if (this.props.disabled) e.preventDefault();
                         else {
                             this.props.preOnClick && this.props.preOnClick();
                             var t = this.props,
                                 n = t.external_link,
                                 r = t.href;
-                            if (r && !zt(n, r)) {
+                            if (r && !Mt(n, r)) {
                                 e.preventDefault();
                                 var a = this.props.href;
-                                window.history.pushState({}, "", a), window.dispatchEvent(new Bt("_dashprivate_pushstate")), window.scrollTo(0, 0)
+                                window.history.pushState({}, "", a), window.dispatchEvent(new Ft("_dashprivate_pushstate")), window.scrollTo(0, 0)
                             }
                         }
                 }
             }, {
                 key: "render",
                 value: function() {
                     var t = this,
                         n = this.props,
                         r = n.children,
                         a = n.external_link,
                         s = (n.preOnClick, n.target),
                         i = n.linkTarget,
                         c = n.href,
                         u = n.download,
-                        d = o(n, Ft),
-                        p = c && zt(a, c);
+                        d = o(n, $t),
+                        p = c && Mt(a, c);
                     return l().createElement("a", e({
                         href: c,
                         target: p ? s || i : void 0,
                         download: u && p ? u : void 0
                     }, d, {
                         onClick: function(e) {
                             return t.updateLocation(e)
                         }
                     }), r)
                 }
-            }]) && Lt(n.prototype, r), Object.defineProperty(n, "prototype", {
+            }]) && St(r.prototype, a), Object.defineProperty(r, "prototype", {
                 writable: !1
-            }), c
+            }), r;
+            var r, a
         }(i.Component);
-        Kt.propTypes = {
+        Bt.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             href: u().string,
             disabled: u().bool,
             external_link: u().bool,
             preOnClick: u().func,
             target: u().string,
             download: u().string
-        }, Kt.defaultProps = {
+        }, Bt.defaultProps = {
             disabled: !1,
             external_link: null
         };
-        var Ht = ["children", "href", "loading_state", "setProps", "color", "style", "className", "class_name", "text_color"];
+        var zt = ["children", "href", "loading_state", "setProps", "color", "style", "className", "class_name", "text_color"];
 
-        function Wt(e, t) {
+        function Kt(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Ut(e) {
+        function Ht(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Wt(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Wt(Object(n)).forEach((function(t) {
+                t % 2 ? Kt(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Kt(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var qt = function(t) {
+        var Ut = function(t) {
             var n = t.children,
                 r = t.href,
                 a = t.loading_state,
                 s = t.setProps,
                 i = t.color,
                 c = t.style,
                 u = t.className,
                 d = t.class_name,
                 p = t.text_color,
-                f = o(t, Ht),
-                g = Et.has(i);
+                f = o(t, zt),
+                g = Fe(r, s),
+                b = Ot.has(i);
             return f[r ? "preOnClick" : "onClick"] = function() {
                 s && s({
                     n_clicks: t.n_clicks + 1,
                     n_clicks_timestamp: Date.now()
                 })
-            }, l().createElement(Dt, e({
-                as: r && Kt,
-                href: r,
-                bg: g ? i : null,
+            }, l().createElement(Tt, e({
+                as: g && Bt,
+                href: g,
+                bg: b ? i : null,
                 text: p,
                 className: d || u,
-                style: g ? c : Ut({
+                style: b ? c : Ht({
                     backgroundColor: i
                 }, c)
             }, m(["setProps", "n_clicks", "n_clicks_timestamp"], f), {
                 "data-dash-is-loading": a && a.is_loading || void 0
             }), n)
         };
-        qt.defaultProps = {
+        Ut.defaultProps = {
             color: "secondary",
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, qt.propTypes = {
+        }, Ut.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
@@ -2388,29 +2389,29 @@
             }),
             external_link: u().bool,
             n_clicks: u().number,
             n_clicks_timestamp: u().number,
             target: u().string,
             title: u().string
         };
-        const Vt = qt,
-            Gt = i.forwardRef((({
+        const Wt = Ut,
+            qt = i.forwardRef((({
                 bsPrefix: e,
-                active: t,
+                active: t = !1,
                 children: n,
                 className: r,
                 as: a = "li",
-                linkAs: s = lt,
-                linkProps: o,
+                linkAs: s = dt,
+                linkProps: o = {},
                 href: i,
                 title: l,
                 target: c,
                 ...u
             }, d) => {
-                const p = j(e, "breadcrumb-item");
+                const p = E(e, "breadcrumb-item");
                 return (0, _.jsx)(a, {
                     ref: d,
                     ...u,
                     className: b()(p, r, {
                         active: t
                     }),
                     "aria-current": t ? "page" : void 0,
@@ -2419,73 +2420,79 @@
                         href: i,
                         title: l,
                         target: c,
                         children: n
                     })
                 })
             }));
-        Gt.displayName = "BreadcrumbItem", Gt.defaultProps = {
-            active: !1,
-            linkProps: {}
-        };
-        const Yt = Gt,
-            Xt = i.forwardRef((({
+        qt.displayName = "BreadcrumbItem";
+        const Vt = qt,
+            Gt = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                listProps: n,
+                listProps: n = {},
                 children: r,
-                label: a,
+                label: a = "breadcrumb",
                 as: s = "nav",
                 ...o
             }, i) => {
-                const l = j(e, "breadcrumb");
+                const l = E(e, "breadcrumb");
                 return (0, _.jsx)(s, {
                     "aria-label": a,
                     className: t,
                     ref: i,
                     ...o,
                     children: (0, _.jsx)("ol", {
                         ...n,
                         className: b()(l, null == n ? void 0 : n.className),
                         children: r
                     })
                 })
             }));
-        Xt.displayName = "Breadcrumb", Xt.defaultProps = {
-            label: "breadcrumb",
-            listProps: {}
-        };
-        const Jt = Object.assign(Xt, {
-            Item: Yt
+        Gt.displayName = "Breadcrumb";
+        const Yt = Object.assign(Gt, {
+            Item: Vt
         });
-        var Qt = ["items", "tag", "loading_state", "class_name", "className", "item_class_name", "itemClassName", "item_style"],
+        var Xt = ["href", "setProps", "external_link", "label"],
+            Jt = ["items", "tag", "loading_state", "class_name", "className", "item_class_name", "itemClassName", "item_style", "setProps"],
+            Qt = function(t) {
+                var n = t.href,
+                    r = t.setProps,
+                    a = t.external_link,
+                    s = t.label,
+                    i = o(t, Xt),
+                    c = Fe(n, r);
+                return l().createElement(Yt.Item, e({
+                    linkAs: c && Bt,
+                    href: c,
+                    linkProps: c && {
+                        external_link: a
+                    }
+                }, i), s)
+            },
             Zt = function(t) {
                 var n = t.items,
                     r = t.tag,
                     a = t.loading_state,
                     s = t.class_name,
                     i = t.className,
                     c = t.item_class_name,
                     u = t.itemClassName,
-                    d = (t.item_style, o(t, Qt));
-                return l().createElement(Jt, e({
+                    d = (t.item_style, t.setProps),
+                    p = o(t, Jt);
+                return l().createElement(Yt, e({
                     as: r,
                     "data-dash-is-loading": a && a.is_loading || void 0,
                     className: s || i
-                }, d), (n || []).map((function(e, t) {
-                    return l().createElement(Jt.Item, {
-                        key: "".concat(e.value).concat(t),
-                        active: e.active,
-                        linkAs: e.href && Kt,
+                }, p), (n || []).map((function(t, n) {
+                    return l().createElement(Qt, e({
+                        key: "".concat(t.value).concat(n),
                         className: c || u,
-                        href: e.href,
-                        linkProps: e.href && {
-                            external_link: e.external_link
-                        }
-                    }, e.label)
+                        setProps: d
+                    }, t))
                 })))
             };
         Zt.propTypes = {
             id: u().string,
             items: u().arrayOf(u().shape({
                 label: u().string,
                 href: u().string,
@@ -2508,40 +2515,39 @@
                 component_name: u().string
             })
         };
         const en = Zt,
             tn = i.forwardRef((({
                 as: e,
                 bsPrefix: t,
-                variant: n,
+                variant: n = "primary",
                 size: r,
-                active: a,
-                className: s,
-                ...o
-            }, i) => {
-                const l = j(t, "btn"),
-                    [c, {
-                        tagName: u
-                    }] = rt({
+                active: a = !1,
+                disabled: s = !1,
+                className: o,
+                ...i
+            }, l) => {
+                const c = E(t, "btn"),
+                    [u, {
+                        tagName: d
+                    }] = ot({
                         tagName: e,
-                        ...o
+                        disabled: s,
+                        ...i
                     }),
-                    d = u;
-                return (0, _.jsx)(d, {
-                    ...c,
-                    ...o,
-                    ref: i,
-                    className: b()(s, l, a && "active", n && `${l}-${n}`, r && `${l}-${r}`, o.href && o.disabled && "disabled")
+                    p = d;
+                return (0, _.jsx)(p, {
+                    ...u,
+                    ...i,
+                    ref: l,
+                    disabled: s,
+                    className: b()(o, c, a && "active", n && `${c}-${n}`, r && `${c}-${r}`, i.href && s && "disabled")
                 })
             }));
-        tn.displayName = "Button", tn.defaultProps = {
-            variant: "primary",
-            active: !1,
-            disabled: !1
-        };
+        tn.displayName = "Button";
         const nn = tn;
         var rn = ["children", "disabled", "href", "loading_state", "setProps", "n_clicks", "target", "type", "download", "name", "value", "className", "class_name", "color", "outline", "onClick", "rel"],
             an = function(t) {
                 var n = t.children,
                     r = t.disabled,
                     a = t.href,
                     s = t.loading_state,
@@ -2555,31 +2561,32 @@
                     b = t.className,
                     y = t.class_name,
                     h = t.color,
                     v = t.outline,
                     _ = t.onClick,
                     x = t.rel,
                     O = o(t, rn),
-                    w = a && !r;
-                return O[w ? "preOnClick" : "onClick"] = _ || function() {
+                    w = Fe(a, i),
+                    N = w && !r;
+                return O[N ? "preOnClick" : "onClick"] = _ || function() {
                     !r && i && i({
                         n_clicks: c + 1,
                         n_clicks_timestamp: Date.now()
                     })
-                }, w && (O.linkTarget = u), l().createElement(nn, e({
-                    as: w ? Kt : "button",
+                }, N && (O.linkTarget = u), l().createElement(nn, e({
+                    as: N ? Bt : "button",
                     variant: v ? "outline-".concat(h) : h,
-                    type: w ? void 0 : d,
-                    href: r ? void 0 : a,
+                    type: N ? void 0 : d,
+                    href: r ? void 0 : w,
                     disabled: r,
-                    download: w ? p : void 0,
-                    name: w ? void 0 : f,
-                    value: w ? void 0 : g,
+                    download: N ? p : void 0,
+                    name: N ? void 0 : f,
+                    value: N ? void 0 : g,
                     className: y || b,
-                    rel: w ? x : void 0
+                    rel: N ? x : void 0
                 }, m(["n_clicks_timestamp"], O), {
                     "data-dash-is-loading": s && s.is_loading || void 0
                 }), n)
             };
         an.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
@@ -2612,31 +2619,30 @@
             value: u().string,
             rel: u().string
         };
         const sn = an,
             on = i.forwardRef((({
                 bsPrefix: e,
                 size: t,
-                vertical: n,
+                vertical: n = !1,
                 className: r,
-                as: a = "div",
-                ...s
-            }, o) => {
-                const i = j(e, "btn-group");
-                let l = i;
-                return n && (l = `${i}-vertical`), (0, _.jsx)(a, {
-                    ...s,
-                    ref: o,
-                    className: b()(r, l, t && `${i}-${t}`)
+                role: a = "group",
+                as: s = "div",
+                ...o
+            }, i) => {
+                const l = E(e, "btn-group");
+                let c = l;
+                return n && (c = `${l}-vertical`), (0, _.jsx)(s, {
+                    ...o,
+                    ref: i,
+                    role: a,
+                    className: b()(r, c, t && `${l}-${t}`)
                 })
             }));
-        on.displayName = "ButtonGroup", on.defaultProps = {
-            vertical: !1,
-            role: "group"
-        };
+        on.displayName = "ButtonGroup";
         const ln = on;
         var cn = ["children", "loading_state", "class_name", "className"],
             un = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.class_name,
                     s = t.className,
@@ -2660,152 +2666,219 @@
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
         const dn = un,
             pn = i.forwardRef((({
-                bsPrefix: e,
-                className: t,
-                variant: n,
-                as: r = "img",
-                ...a
-            }, s) => {
-                const o = j(e, "card-img");
-                return (0, _.jsx)(r, {
-                    ref: s,
-                    className: b()(n ? `${o}-${n}` : o, t),
-                    ...a
-                })
-            }));
-        pn.displayName = "CardImg";
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "card-body"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        pn.displayName = "CardBody";
         const fn = pn,
-            mn = i.createContext(null);
-        mn.displayName = "CardHeaderContext";
+            mn = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "card-footer"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        mn.displayName = "CardFooter";
         const gn = mn,
-            bn = i.forwardRef((({
+            bn = i.createContext(null);
+        bn.displayName = "CardHeaderContext";
+        const yn = bn,
+            hn = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n = "div",
                 ...r
             }, a) => {
-                const s = j(e, "card-header"),
+                const s = E(e, "card-header"),
                     o = (0, i.useMemo)((() => ({
                         cardHeaderBsPrefix: s
                     })), [s]);
-                return (0, _.jsx)(gn.Provider, {
+                return (0, _.jsx)(yn.Provider, {
                     value: o,
                     children: (0, _.jsx)(n, {
                         ref: a,
                         ...r,
                         className: b()(t, s)
                     })
                 })
             }));
-        bn.displayName = "CardHeader";
-        const yn = bn,
-            hn = gt("h5"),
-            vn = gt("h6"),
-            _n = ht("card-body"),
-            xn = ht("card-title", {
-                Component: hn
-            }),
-            On = ht("card-subtitle", {
-                Component: vn
-            }),
-            wn = ht("card-link", {
-                Component: "a"
-            }),
-            Nn = ht("card-text", {
-                Component: "p"
-            }),
-            En = ht("card-footer"),
-            jn = ht("card-img-overlay"),
+        hn.displayName = "CardHeader";
+        const vn = hn,
+            _n = i.forwardRef((({
+                bsPrefix: e,
+                className: t,
+                variant: n,
+                as: r = "img",
+                ...a
+            }, s) => {
+                const o = E(e, "card-img");
+                return (0, _.jsx)(r, {
+                    ref: s,
+                    className: b()(n ? `${o}-${n}` : o, t),
+                    ...a
+                })
+            }));
+        _n.displayName = "CardImg";
+        const xn = _n,
+            On = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "card-img-overlay"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        On.displayName = "CardImgOverlay";
+        const wn = On,
+            Nn = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "a",
+                ...r
+            }, a) => (t = E(t, "card-link"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Nn.displayName = "CardLink";
+        const En = Nn,
+            jn = Xe("h6"),
             kn = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = jn,
+                ...r
+            }, a) => (t = E(t, "card-subtitle"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        kn.displayName = "CardSubtitle";
+        const Pn = kn,
+            Cn = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "p",
+                ...r
+            }, a) => (t = E(t, "card-text"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Cn.displayName = "CardText";
+        const Tn = Cn,
+            Sn = Xe("h5"),
+            Rn = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = Sn,
+                ...r
+            }, a) => (t = E(t, "card-title"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Rn.displayName = "CardTitle";
+        const Dn = Rn,
+            Ln = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 bg: n,
                 text: r,
                 border: a,
-                body: s,
+                body: s = !1,
                 children: o,
                 as: i = "div",
                 ...l
             }, c) => {
-                const u = j(e, "card");
+                const u = E(e, "card");
                 return (0, _.jsx)(i, {
                     ref: c,
                     ...l,
                     className: b()(t, u, n && `bg-${n}`, r && `text-${r}`, a && `border-${a}`),
-                    children: s ? (0, _.jsx)(_n, {
+                    children: s ? (0, _.jsx)(fn, {
                         children: o
                     }) : o
                 })
             }));
-        kn.displayName = "Card", kn.defaultProps = {
-            body: !1
-        };
-        const Pn = Object.assign(kn, {
-            Img: fn,
-            Title: xn,
-            Subtitle: On,
-            Body: _n,
-            Link: wn,
-            Text: Nn,
-            Header: yn,
-            Footer: En,
-            ImgOverlay: jn
+        Ln.displayName = "Card";
+        const $n = Object.assign(Ln, {
+            Img: xn,
+            Title: Dn,
+            Subtitle: Pn,
+            Body: fn,
+            Link: En,
+            Text: Tn,
+            Header: vn,
+            Footer: gn,
+            ImgOverlay: wn
         });
-        var Cn = ["children", "color", "inverse", "outline", "style", "loading_state", "className", "class_name"];
+        var In = ["children", "color", "inverse", "outline", "style", "loading_state", "className", "class_name"];
 
-        function Tn(e, t) {
+        function An(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Sn(e) {
+        function Fn(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Tn(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Tn(Object(n)).forEach((function(t) {
+                t % 2 ? An(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : An(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Rn = function(t) {
+        var Mn = function(t) {
             var n = t.children,
                 r = t.color,
                 a = t.inverse,
                 s = t.outline,
                 i = t.style,
                 c = t.loading_state,
                 u = t.className,
                 d = t.class_name,
-                p = o(t, Cn),
-                f = Et.has(r);
-            return l().createElement(Pn, e({
+                p = o(t, In),
+                f = Ot.has(r);
+            return l().createElement($n, e({
                 "data-dash-is-loading": c && c.is_loading || void 0,
                 text: a ? "white" : null,
                 bg: f && !s ? r : null,
                 border: f && s ? r : null,
-                style: f ? i : Sn({
+                style: f ? i : Fn({
                     backgroundColor: r
                 }, i),
                 className: d || u
             }, m(["setProps"], p)), n)
         };
-        Rn.propTypes = {
+        Mn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
@@ -2814,140 +2887,151 @@
             inverse: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Dn = Rn;
-        var Ln = ["children", "loading_state", "className", "class_name"],
-            $n = function(t) {
+        const Bn = Mn;
+        var zn = ["children", "loading_state", "className", "class_name"],
+            Kn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Ln);
-                return l().createElement(Pn.Body, e({
+                    i = o(t, zn);
+                return l().createElement($n.Body, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        $n.propTypes = {
+        Kn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const In = $n;
-        var An = ["children", "loading_state", "className", "class_name"],
-            Mn = function(t) {
+        const Hn = Kn;
+        var Un = ["children", "loading_state", "className", "class_name"],
+            Wn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, An);
-                return l().createElement(Pn.Footer, e({
+                    i = o(t, Un);
+                return l().createElement($n.Footer, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Mn.propTypes = {
+        Wn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Fn = Mn,
-            Bn = ht("card-group");
-        var zn = ["children", "loading_state", "className", "class_name"],
-            Kn = function(t) {
+        const qn = Wn,
+            Vn = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "card-group"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Vn.displayName = "CardGroup";
+        const Gn = Vn;
+        var Yn = ["children", "loading_state", "className", "class_name"],
+            Xn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, zn);
-                return l().createElement(Bn, e({
+                    i = o(t, Yn);
+                return l().createElement(Gn, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Kn.propTypes = {
+        Xn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Hn = Kn;
-        var Wn = ["children", "loading_state", "className", "class_name"],
-            Un = function(t) {
+        const Jn = Xn;
+        var Qn = ["children", "loading_state", "className", "class_name"],
+            Zn = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Wn);
-                return l().createElement(yn, e({
+                    i = o(t, Qn);
+                return l().createElement(vn, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Un.propTypes = {
+        Zn.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const qn = Un;
-        var Vn = ["children", "loading_state", "className", "class_name", "top", "bottom"],
-            Gn = function(t) {
+        const er = Zn;
+        var tr = ["children", "loading_state", "className", "class_name", "top", "bottom"],
+            nr = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.top,
                     c = t.bottom,
-                    u = o(t, Vn);
-                return l().createElement(fn, e({
+                    u = o(t, tr);
+                return l().createElement(xn, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a,
                     variant: i ? "top" : c ? "bottom" : null
                 }, m(["setProps"], u)), n)
             };
-        Gn.propTypes = {
+        nr.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
@@ -2958,67 +3042,71 @@
             title: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Yn = Gn;
-        var Xn = ["children", "loading_state", "className", "class_name"],
-            Jn = function(t) {
+        const rr = nr;
+        var ar = ["children", "loading_state", "className", "class_name"],
+            sr = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Xn);
-                return l().createElement(Pn.ImgOverlay, e({
+                    i = o(t, ar);
+                return l().createElement($n.ImgOverlay, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
                     className: s || a
                 }, m(["setProps"], i)), n)
             };
-        Jn.propTypes = {
+        sr.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Qn = Jn;
-        var Zn = ["children", "loading_state", "disabled", "className", "class_name"],
-            er = function(t) {
+        const or = sr;
+        var ir = ["children", "loading_state", "disabled", "className", "class_name", "href", "setProps"],
+            lr = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.disabled,
                     s = t.className,
                     i = t.class_name,
-                    c = o(t, Zn);
-                return l().createElement(Pn.Link, e({
+                    c = t.href,
+                    u = t.setProps,
+                    d = o(t, ir),
+                    p = Fe(c, u);
+                return l().createElement($n.Link, e({
                     "data-dash-is-loading": r && r.is_loading || void 0,
-                    as: Kt,
+                    as: Bt,
                     preOnClick: function() {
-                        !a && t.setProps && t.setProps({
+                        !a && u && u({
                             n_clicks: t.n_clicks + 1,
                             n_clicks_timestamp: Date.now()
                         })
                     },
                     disabled: a,
+                    href: p,
                     className: i || s
-                }, m(["setProps", "n_clicks", "n_clicks_timestamp"], c)), n)
+                }, m(["n_clicks", "n_clicks_timestamp"], d)), n)
             };
-        er.defaultProps = {
+        lr.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, er.propTypes = {
+        }, lr.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             href: u().string,
@@ -3028,351 +3116,347 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
         };
-        const tr = er;
+        const cr = lr;
 
-        function nr(e) {
-            var t, n, r = (t = e, (n = (0, i.useRef)(t)).current = t, n);
-            (0, i.useEffect)((function() {
-                return function() {
-                    return r.current()
-                }
-            }), [])
+        function ur(e) {
+            const t = function(e) {
+                const t = (0, i.useRef)(e);
+                return t.current = e, t
+            }(e);
+            (0, i.useEffect)((() => () => t.current()), [])
         }
-        var rr = Math.pow(2, 31) - 1;
+        const dr = 2 ** 31 - 1;
 
-        function ar(e, t, n) {
-            var r = n - Date.now();
-            e.current = r <= rr ? setTimeout(t, r) : setTimeout((function() {
-                return ar(e, t, n)
-            }), rr)
+        function pr(e, t, n) {
+            const r = n - Date.now();
+            e.current = r <= dr ? setTimeout(t, r) : setTimeout((() => pr(e, t, n)), dr)
         }
 
-        function sr() {
-            var e = Qe(),
+        function fr() {
+            const e = tt(),
                 t = (0, i.useRef)();
-            return nr((function() {
-                return clearTimeout(t.current)
-            })), (0, i.useMemo)((function() {
-                var n = function() {
-                    return clearTimeout(t.current)
-                };
+            return ur((() => clearTimeout(t.current))), (0, i.useMemo)((() => {
+                const n = () => clearTimeout(t.current);
                 return {
-                    set: function(r, a) {
-                        void 0 === a && (a = 0), e() && (n(), a <= rr ? t.current = setTimeout(r, a) : ar(t, r, Date.now() + a))
+                    set: function(r, a = 0) {
+                        e() && (n(), a <= dr ? t.current = setTimeout(r, a) : pr(t, r, Date.now() + a))
                     },
-                    clear: n
+                    clear: n,
+                    handleRef: t
                 }
             }), [])
         }
-        const or = ht("carousel-caption"),
-            ir = i.forwardRef((({
+        const mr = i.forwardRef((({
+            className: e,
+            bsPrefix: t,
+            as: n = "div",
+            ...r
+        }, a) => (t = E(t, "carousel-caption"), (0, _.jsx)(n, {
+            ref: a,
+            className: b()(e, t),
+            ...r
+        }))));
+        mr.displayName = "CarouselCaption";
+        const gr = mr,
+            br = i.forwardRef((({
                 as: e = "div",
                 bsPrefix: t,
                 className: n,
                 ...r
             }, a) => {
-                const s = b()(n, j(t, "carousel-item"));
+                const s = b()(n, E(t, "carousel-item"));
                 return (0, _.jsx)(e, {
                     ref: a,
                     ...r,
                     className: s
                 })
             }));
-        ir.displayName = "CarouselItem";
-        const lr = ir;
+        br.displayName = "CarouselItem";
+        const yr = br;
 
-        function cr(e, t) {
+        function hr(e, t) {
             let n = 0;
             return i.Children.map(e, (e => i.isValidElement(e) ? t(e, n++) : e))
         }
-        const ur = {
-                slide: !0,
-                fade: !1,
-                controls: !0,
-                indicators: !0,
-                indicatorLabels: [],
-                defaultActiveIndex: 0,
-                interval: 5e3,
-                keyboard: !0,
-                pause: "hover",
-                wrap: !0,
-                touch: !0,
-                prevIcon: (0, _.jsx)("span", {
+        const vr = i.forwardRef((({
+            defaultActiveIndex: e = 0,
+            ...t
+        }, n) => {
+            const {
+                as: r = "div",
+                bsPrefix: a,
+                slide: s = !0,
+                fade: o = !1,
+                controls: l = !0,
+                indicators: c = !0,
+                indicatorLabels: u = [],
+                activeIndex: d,
+                onSelect: p,
+                onSlide: f,
+                onSlid: m,
+                interval: g = 5e3,
+                keyboard: y = !0,
+                onKeyDown: h,
+                pause: x = "hover",
+                onMouseOver: O,
+                onMouseOut: w,
+                wrap: N = !0,
+                touch: j = !0,
+                onTouchStart: k,
+                onTouchMove: C,
+                onTouchEnd: T,
+                prevIcon: S = (0, _.jsx)("span", {
                     "aria-hidden": "true",
                     className: "carousel-control-prev-icon"
                 }),
-                prevLabel: "Previous",
-                nextIcon: (0, _.jsx)("span", {
+                prevLabel: R = "Previous",
+                nextIcon: D = (0, _.jsx)("span", {
                     "aria-hidden": "true",
                     className: "carousel-control-next-icon"
                 }),
-                nextLabel: "Next"
-            },
-            dr = i.forwardRef(((e, t) => {
-                const {
-                    as: n = "div",
-                    bsPrefix: r,
-                    slide: a,
-                    fade: s,
-                    controls: o,
-                    indicators: l,
-                    indicatorLabels: c,
-                    activeIndex: u,
-                    onSelect: d,
-                    onSlide: p,
-                    onSlid: f,
-                    interval: m,
-                    keyboard: g,
-                    onKeyDown: y,
-                    pause: h,
-                    onMouseOver: x,
-                    onMouseOut: O,
-                    wrap: w,
-                    touch: N,
-                    onTouchStart: E,
-                    onTouchMove: k,
-                    onTouchEnd: P,
-                    prevIcon: T,
-                    prevLabel: S,
-                    nextIcon: R,
-                    nextLabel: D,
-                    variant: L,
-                    className: $,
-                    children: I,
-                    ...A
-                } = v(e, {
-                    activeIndex: "onSelect"
-                }), M = j(r, "carousel"), F = C(), B = (0, i.useRef)(null), [z, K] = (0, i.useState)("next"), [H, W] = (0, i.useState)(!1), [U, q] = (0, i.useState)(!1), [V, G] = (0, i.useState)(u || 0);
-                (0, i.useEffect)((() => {
-                    U || u === V || (B.current ? K(B.current) : K((u || 0) > V ? "next" : "prev"), a && q(!0), G(u || 0))
-                }), [u, U, V, a]), (0, i.useEffect)((() => {
-                    B.current && (B.current = null)
-                }));
-                let Y, X = 0;
-                ! function(e, t) {
-                    let n = 0;
-                    i.Children.forEach(e, (e => {
-                        i.isValidElement(e) && ((e, t) => {
-                            ++X, t === u && (Y = e.props.interval)
-                        })(e, n++)
-                    }))
-                }(I);
-                const J = Ye(Y),
-                    Q = (0, i.useCallback)((e => {
-                        if (U) return;
-                        let t = V - 1;
-                        if (t < 0) {
-                            if (!w) return;
-                            t = X - 1
-                        }
-                        B.current = "prev", null == d || d(t, e)
-                    }), [U, V, d, w, X]),
-                    Z = Xe((e => {
-                        if (U) return;
-                        let t = V + 1;
-                        if (t >= X) {
-                            if (!w) return;
-                            t = 0
-                        }
-                        B.current = "next", null == d || d(t, e)
-                    })),
-                    ee = (0, i.useRef)();
-                (0, i.useImperativeHandle)(t, (() => ({
-                    element: ee.current,
-                    prev: Q,
-                    next: Z
-                })));
-                const te = Xe((() => {
-                        !document.hidden && function(e) {
-                            if (!(e && e.style && e.parentNode && e.parentNode.style)) return !1;
-                            const t = getComputedStyle(e);
-                            return "none" !== t.display && "hidden" !== t.visibility && "none" !== getComputedStyle(e.parentNode).display
-                        }(ee.current) && (F ? Q() : Z())
-                    })),
-                    ne = "next" === z ? "start" : "end";
-                var ae, oe, ie;
-                ae = () => {
-                    a || (null == p || p(V, ne), null == f || f(V, ne))
-                }, oe = [V], ie = (0, i.useRef)(!0), (0, i.useEffect)((function() {
-                    if (!ie.current) return ae();
-                    ie.current = !1
-                }), oe);
-                const le = `${M}-item-${z}`,
-                    ue = `${M}-item-${ne}`,
-                    de = (0, i.useCallback)((e => {
-                        se(e), null == p || p(V, ne)
-                    }), [p, V, ne]),
-                    pe = (0, i.useCallback)((() => {
-                        q(!1), null == f || f(V, ne)
-                    }), [f, V, ne]),
-                    fe = (0, i.useCallback)((e => {
-                        if (g && !/input|textarea/i.test(e.target.tagName)) switch (e.key) {
-                            case "ArrowLeft":
-                                return e.preventDefault(), void(F ? Z(e) : Q(e));
-                            case "ArrowRight":
-                                return e.preventDefault(), void(F ? Q(e) : Z(e))
-                        }
-                        null == y || y(e)
-                    }), [g, y, Q, Z, F]),
-                    me = (0, i.useCallback)((e => {
-                        "hover" === h && W(!0), null == x || x(e)
-                    }), [h, x]),
-                    ge = (0, i.useCallback)((e => {
-                        W(!1), null == O || O(e)
-                    }), [O]),
-                    be = (0, i.useRef)(0),
-                    ye = (0, i.useRef)(0),
-                    he = sr(),
-                    ve = (0, i.useCallback)((e => {
-                        be.current = e.touches[0].clientX, ye.current = 0, "hover" === h && W(!0), null == E || E(e)
-                    }), [h, E]),
-                    _e = (0, i.useCallback)((e => {
-                        e.touches && e.touches.length > 1 ? ye.current = 0 : ye.current = e.touches[0].clientX - be.current, null == k || k(e)
-                    }), [k]),
-                    xe = (0, i.useCallback)((e => {
-                        if (N) {
-                            const t = ye.current;
-                            Math.abs(t) > 40 && (t > 0 ? Q(e) : Z(e))
-                        }
-                        "hover" === h && he.set((() => {
-                            W(!1)
-                        }), m || void 0), null == P || P(e)
-                    }), [N, h, Q, Z, he, m, P]),
-                    Oe = null != m && !H && !U,
-                    we = (0, i.useRef)();
+                nextLabel: L = "Next",
+                variant: $,
+                className: I,
+                children: A,
+                ...F
+            } = v({
+                defaultActiveIndex: e,
+                ...t
+            }, {
+                activeIndex: "onSelect"
+            }), M = E(a, "carousel"), B = P(), z = (0, i.useRef)(null), [K, H] = (0, i.useState)("next"), [U, W] = (0, i.useState)(!1), [q, V] = (0, i.useState)(!1), [G, Y] = (0, i.useState)(d || 0);
+            (0, i.useEffect)((() => {
+                q || d === G || (z.current ? H(z.current) : H((d || 0) > G ? "next" : "prev"), s && V(!0), Y(d || 0))
+            }), [d, q, G, s]), (0, i.useEffect)((() => {
+                z.current && (z.current = null)
+            }));
+            let X, J = 0;
+            ! function(e, t) {
+                let n = 0;
+                i.Children.forEach(e, (e => {
+                    i.isValidElement(e) && ((e, t) => {
+                        ++J, t === d && (X = e.props.interval)
+                    })(e, n++)
+                }))
+            }(A);
+            const Q = Ge(X),
+                Z = (0, i.useCallback)((e => {
+                    if (q) return;
+                    let t = G - 1;
+                    if (t < 0) {
+                        if (!N) return;
+                        t = J - 1
+                    }
+                    z.current = "prev", null == p || p(t, e)
+                }), [q, G, p, N, J]),
+                ee = Ye((e => {
+                    if (q) return;
+                    let t = G + 1;
+                    if (t >= J) {
+                        if (!N) return;
+                        t = 0
+                    }
+                    z.current = "next", null == p || p(t, e)
+                })),
+                te = (0, i.useRef)();
+            (0, i.useImperativeHandle)(n, (() => ({
+                element: te.current,
+                prev: Z,
+                next: ee
+            })));
+            const re = Ye((() => {
+                    !document.hidden && function(e) {
+                        if (!(e && e.style && e.parentNode && e.parentNode.style)) return !1;
+                        const t = getComputedStyle(e);
+                        return "none" !== t.display && "hidden" !== t.visibility && "none" !== getComputedStyle(e.parentNode).display
+                    }(te.current) && (B ? Z() : ee())
+                })),
+                se = "next" === K ? "start" : "end";
+            ! function(e, t) {
+                const n = (0, i.useRef)(!0);
                 (0, i.useEffect)((() => {
-                    var e, t;
-                    if (!Oe) return;
-                    const n = F ? Q : Z;
-                    return we.current = window.setInterval(document.visibilityState ? te : n, null != (e = null != (t = J.current) ? t : m) ? e : void 0), () => {
-                        null !== we.current && clearInterval(we.current)
-                    }
-                }), [Oe, Q, Z, J, m, te, F]);
-                const Ne = (0, i.useMemo)((() => l && Array.from({
-                    length: X
-                }, ((e, t) => e => {
-                    null == d || d(t, e)
-                }))), [l, X, d]);
-                return (0, _.jsxs)(n, {
-                    ref: ee,
-                    ...A,
-                    onKeyDown: fe,
-                    onMouseOver: me,
-                    onMouseOut: ge,
-                    onTouchStart: ve,
-                    onTouchMove: _e,
-                    onTouchEnd: xe,
-                    className: b()($, M, a && "slide", s && `${M}-fade`, L && `${M}-${L}`),
-                    children: [l && (0, _.jsx)("div", {
-                        className: `${M}-indicators`,
-                        children: cr(I, ((e, t) => (0, _.jsx)("button", {
-                            type: "button",
-                            "data-bs-target": "",
-                            "aria-label": null != c && c.length ? c[t] : `Slide ${t+1}`,
-                            className: t === V ? "active" : void 0,
-                            onClick: Ne ? Ne[t] : void 0,
-                            "aria-current": t === V
-                        }, t)))
-                    }), (0, _.jsx)("div", {
-                        className: `${M}-inner`,
-                        children: cr(I, ((e, t) => {
-                            const n = t === V;
-                            return a ? (0, _.jsx)(ce, {
-                                in: n,
-                                onEnter: n ? de : void 0,
-                                onEntered: n ? pe : void 0,
-                                addEndListener: re,
-                                children: (t, r) => i.cloneElement(e, {
-                                    ...r,
-                                    className: b()(e.props.className, n && "entered" !== t && le, ("entered" === t || "exiting" === t) && "active", ("entering" === t || "exiting" === t) && ue)
-                                })
-                            }) : i.cloneElement(e, {
-                                className: b()(e.props.className, n && "active")
+                    if (!n.current) return e();
+                    n.current = !1
+                }), t)
+            }((() => {
+                s || (null == f || f(G, se), null == m || m(G, se))
+            }), [G]);
+            const oe = `${M}-item-${K}`,
+                ie = `${M}-item-${se}`,
+                ce = (0, i.useCallback)((e => {
+                    ae(e), null == f || f(G, se)
+                }), [f, G, se]),
+                ue = (0, i.useCallback)((() => {
+                    V(!1), null == m || m(G, se)
+                }), [m, G, se]),
+                de = (0, i.useCallback)((e => {
+                    if (y && !/input|textarea/i.test(e.target.tagName)) switch (e.key) {
+                        case "ArrowLeft":
+                            return e.preventDefault(), void(B ? ee(e) : Z(e));
+                        case "ArrowRight":
+                            return e.preventDefault(), void(B ? Z(e) : ee(e))
+                    }
+                    null == h || h(e)
+                }), [y, h, Z, ee, B]),
+                pe = (0, i.useCallback)((e => {
+                    "hover" === x && W(!0), null == O || O(e)
+                }), [x, O]),
+                fe = (0, i.useCallback)((e => {
+                    W(!1), null == w || w(e)
+                }), [w]),
+                me = (0, i.useRef)(0),
+                ge = (0, i.useRef)(0),
+                be = fr(),
+                ye = (0, i.useCallback)((e => {
+                    me.current = e.touches[0].clientX, ge.current = 0, "hover" === x && W(!0), null == k || k(e)
+                }), [x, k]),
+                he = (0, i.useCallback)((e => {
+                    e.touches && e.touches.length > 1 ? ge.current = 0 : ge.current = e.touches[0].clientX - me.current, null == C || C(e)
+                }), [C]),
+                ve = (0, i.useCallback)((e => {
+                    if (j) {
+                        const t = ge.current;
+                        Math.abs(t) > 40 && (t > 0 ? Z(e) : ee(e))
+                    }
+                    "hover" === x && be.set((() => {
+                        W(!1)
+                    }), g || void 0), null == T || T(e)
+                }), [j, x, Z, ee, be, g, T]),
+                _e = null != g && !U && !q,
+                xe = (0, i.useRef)();
+            (0, i.useEffect)((() => {
+                var e, t;
+                if (!_e) return;
+                const n = B ? Z : ee;
+                return xe.current = window.setInterval(document.visibilityState ? re : n, null != (e = null != (t = Q.current) ? t : g) ? e : void 0), () => {
+                    null !== xe.current && clearInterval(xe.current)
+                }
+            }), [_e, Z, ee, Q, g, re, B]);
+            const Oe = (0, i.useMemo)((() => c && Array.from({
+                length: J
+            }, ((e, t) => e => {
+                null == p || p(t, e)
+            }))), [c, J, p]);
+            return (0, _.jsxs)(r, {
+                ref: te,
+                ...F,
+                onKeyDown: de,
+                onMouseOver: pe,
+                onMouseOut: fe,
+                onTouchStart: ye,
+                onTouchMove: he,
+                onTouchEnd: ve,
+                className: b()(I, M, s && "slide", o && `${M}-fade`, $ && `${M}-${$}`),
+                children: [c && (0, _.jsx)("div", {
+                    className: `${M}-indicators`,
+                    children: hr(A, ((e, t) => (0, _.jsx)("button", {
+                        type: "button",
+                        "data-bs-target": "",
+                        "aria-label": null != u && u.length ? u[t] : `Slide ${t+1}`,
+                        className: t === G ? "active" : void 0,
+                        onClick: Oe ? Oe[t] : void 0,
+                        "aria-current": t === G
+                    }, t)))
+                }), (0, _.jsx)("div", {
+                    className: `${M}-inner`,
+                    children: hr(A, ((e, t) => {
+                        const n = t === G;
+                        return s ? (0, _.jsx)(le, {
+                            in: n,
+                            onEnter: n ? ce : void 0,
+                            onEntered: n ? ue : void 0,
+                            addEndListener: ne,
+                            children: (t, r) => i.cloneElement(e, {
+                                ...r,
+                                className: b()(e.props.className, n && "entered" !== t && oe, ("entered" === t || "exiting" === t) && "active", ("entering" === t || "exiting" === t) && ie)
                             })
-                        }))
-                    }), o && (0, _.jsxs)(_.Fragment, {
-                        children: [(w || 0 !== u) && (0, _.jsxs)(lt, {
-                            className: `${M}-control-prev`,
-                            onClick: Q,
-                            children: [T, S && (0, _.jsx)("span", {
-                                className: "visually-hidden",
-                                children: S
-                            })]
-                        }), (w || u !== X - 1) && (0, _.jsxs)(lt, {
-                            className: `${M}-control-next`,
-                            onClick: Z,
-                            children: [R, D && (0, _.jsx)("span", {
-                                className: "visually-hidden",
-                                children: D
-                            })]
+                        }) : i.cloneElement(e, {
+                            className: b()(e.props.className, n && "active")
+                        })
+                    }))
+                }), l && (0, _.jsxs)(_.Fragment, {
+                    children: [(N || 0 !== d) && (0, _.jsxs)(dt, {
+                        className: `${M}-control-prev`,
+                        onClick: Z,
+                        children: [S, R && (0, _.jsx)("span", {
+                            className: "visually-hidden",
+                            children: R
+                        })]
+                    }), (N || d !== J - 1) && (0, _.jsxs)(dt, {
+                        className: `${M}-control-next`,
+                        onClick: ee,
+                        children: [D, L && (0, _.jsx)("span", {
+                            className: "visually-hidden",
+                            children: L
                         })]
                     })]
-                })
-            }));
-        dr.displayName = "Carousel", dr.defaultProps = ur;
-        const pr = Object.assign(dr, {
-            Caption: or,
-            Item: lr
+                })]
+            })
+        }));
+        vr.displayName = "Carousel";
+        const _r = Object.assign(vr, {
+            Caption: gr,
+            Item: yr
         });
-        var fr = ["items", "active_index", "style", "class_name", "className", "loading_state", "setProps", "interval"],
-            mr = function(t) {
+        var xr = ["items", "active_index", "style", "class_name", "className", "loading_state", "setProps", "interval"],
+            Or = function(t) {
                 var n = t.items,
                     r = t.active_index,
                     a = t.style,
                     s = t.class_name,
                     i = t.className,
                     c = t.loading_state,
                     u = t.setProps,
                     d = t.interval,
-                    p = o(t, fr),
+                    p = o(t, xr),
                     f = n.map((function(t) {
                         t.imgClassName = void 0 !== t.imgClassName ? t.imgClassName : "d-block w-100";
                         var n = t.href ? {
                             href: t.href,
                             external_link: t.external_link,
                             target: t.target || "_self"
                         } : {};
-                        return l().createElement(pr.Item, e({
+                        return l().createElement(_r.Item, e({
                             key: t.key,
-                            as: t.href ? Kt : "div"
+                            as: t.href ? Bt : "div"
                         }, n), l().createElement("img", {
                             src: t.src,
                             className: t.img_class_name || t.imgClassName,
                             style: t.img_style,
                             alt: t.alt
-                        }), l().createElement(pr.Caption, {
+                        }), l().createElement(_r.Caption, {
                             className: t.caption_class_name || t.captionClassName
                         }, t.header && l().createElement("h5", null, t.header), t.caption && l().createElement("p", null, t.caption)))
                     }));
                 return l().createElement("div", {
                     style: a,
                     className: s || i
-                }, l().createElement(pr, e({
+                }, l().createElement(_r, e({
                     "data-dash-is-loading": c && c.is_loading || void 0,
                     activeIndex: r,
                     onSelect: function(e) {
                         return u({
                             active_index: e
                         })
                     },
                     interval: d || null
                 }, m(["persistence", "persisted_props", "persistence_type", "setProps"], p)), f))
             };
-        mr.defaultProps = {
+        Or.defaultProps = {
             active_index: 0,
             controls: !0,
             indicators: !0,
             persisted_props: ["active_index"],
             persistence_type: "local"
-        }, mr.propTypes = {
+        }, Or.propTypes = {
             id: u().string,
             style: u().object,
             class_name: u().string,
             className: u().string,
             items: u().arrayOf(u().exact({
                 key: u().string,
                 src: u().string,
@@ -3401,16 +3485,16 @@
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["active_index"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
         };
-        const gr = mr;
-        var br = function(e) {
+        const wr = Or;
+        var Nr = function(e) {
             var t = e.value,
                 n = e.disabled,
                 r = e.className,
                 a = e.class_name,
                 s = e.style,
                 o = e.id,
                 i = e.input_class_name,
@@ -3444,15 +3528,15 @@
             }), l().createElement("label", {
                 id: p,
                 style: f,
                 className: b()(m || g, "form-check-label", "form-label"),
                 htmlFor: o
             }, d))
         };
-        br.propTypes = {
+        Nr.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             input_style: u().object,
             inputStyle: u().object,
             input_class_name: u().string,
@@ -3471,129 +3555,129 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
-        }, br.defaultProps = {
+        }, Nr.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             persisted_props: ["value"],
             persistence_type: "local",
             value: !1,
             disabled: !1
         };
-        const yr = br;
+        const Er = Nr;
 
-        function hr(e) {
+        function jr(e) {
             for (var t, n = []; !(t = e.next()).done;) n.push(t.value);
             return n
         }
 
-        function vr(e, t, n) {
+        function kr(e, t, n) {
             for (var r = 0, a = n.length; r < a;) {
                 if (e(t, n[r])) return !0;
                 r += 1
             }
             return !1
         }
 
-        function _r(e, t) {
+        function Pr(e, t) {
             return Object.prototype.hasOwnProperty.call(t, e)
         }
-        const xr = "function" == typeof Object.is ? Object.is : function(e, t) {
+        const Cr = "function" == typeof Object.is ? Object.is : function(e, t) {
             return e === t ? 0 !== e || 1 / e == 1 / t : e != e && t != t
         };
-        var Or = Object.prototype.toString;
-        const wr = function() {
-            return "[object Arguments]" === Or.call(arguments) ? function(e) {
-                return "[object Arguments]" === Or.call(e)
+        var Tr = Object.prototype.toString;
+        const Sr = function() {
+            return "[object Arguments]" === Tr.call(arguments) ? function(e) {
+                return "[object Arguments]" === Tr.call(e)
             } : function(e) {
-                return _r("callee", e)
+                return Pr("callee", e)
             }
         }();
-        var Nr = !{
+        var Rr = !{
                 toString: null
             }.propertyIsEnumerable("toString"),
-            Er = ["constructor", "valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
-            jr = function() {
+            Dr = ["constructor", "valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
+            Lr = function() {
                 return arguments.propertyIsEnumerable("length")
             }(),
-            kr = function(e, t) {
+            $r = function(e, t) {
                 for (var n = 0; n < e.length;) {
                     if (e[n] === t) return !0;
                     n += 1
                 }
                 return !1
             };
-        const Pr = "function" != typeof Object.keys || jr ? p((function(e) {
+        const Ir = "function" != typeof Object.keys || Lr ? p((function(e) {
             if (Object(e) !== e) return [];
             var t, n, r = [],
-                a = jr && wr(e);
-            for (t in e) !_r(t, e) || a && "length" === t || (r[r.length] = t);
-            if (Nr)
-                for (n = Er.length - 1; n >= 0;) _r(t = Er[n], e) && !kr(r, t) && (r[r.length] = t), n -= 1;
+                a = Lr && Sr(e);
+            for (t in e) !Pr(t, e) || a && "length" === t || (r[r.length] = t);
+            if (Rr)
+                for (n = Dr.length - 1; n >= 0;) Pr(t = Dr[n], e) && !$r(r, t) && (r[r.length] = t), n -= 1;
             return r
         })) : p((function(e) {
             return Object(e) !== e ? [] : Object.keys(e)
         }));
 
-        function Cr(e, t, n, r) {
-            var a = hr(e);
+        function Ar(e, t, n, r) {
+            var a = jr(e);
 
             function s(e, t) {
-                return Tr(e, t, n.slice(), r.slice())
+                return Fr(e, t, n.slice(), r.slice())
             }
-            return !vr((function(e, t) {
-                return !vr(s, t, e)
-            }), hr(t), a)
+            return !kr((function(e, t) {
+                return !kr(s, t, e)
+            }), jr(t), a)
         }
 
-        function Tr(e, t, n, r) {
-            if (xr(e, t)) return !0;
-            var a, s, o = $e(e);
-            if (o !== $e(t)) return !1;
+        function Fr(e, t, n, r) {
+            if (Cr(e, t)) return !0;
+            var a, s, o = Re(e);
+            if (o !== Re(t)) return !1;
             if (null == e || null == t) return !1;
             if ("function" == typeof e["fantasy-land/equals"] || "function" == typeof t["fantasy-land/equals"]) return "function" == typeof e["fantasy-land/equals"] && e["fantasy-land/equals"](t) && "function" == typeof t["fantasy-land/equals"] && t["fantasy-land/equals"](e);
             if ("function" == typeof e.equals || "function" == typeof t.equals) return "function" == typeof e.equals && e.equals(t) && "function" == typeof t.equals && t.equals(e);
             switch (o) {
                 case "Arguments":
                 case "Array":
                 case "Object":
                     if ("function" == typeof e.constructor && "Promise" === (a = e.constructor, null == (s = String(a).match(/^function (\w*)/)) ? "" : s[1])) return e === t;
                     break;
                 case "Boolean":
                 case "Number":
                 case "String":
-                    if (typeof e != typeof t || !xr(e.valueOf(), t.valueOf())) return !1;
+                    if (typeof e != typeof t || !Cr(e.valueOf(), t.valueOf())) return !1;
                     break;
                 case "Date":
-                    if (!xr(e.valueOf(), t.valueOf())) return !1;
+                    if (!Cr(e.valueOf(), t.valueOf())) return !1;
                     break;
                 case "Error":
                     return e.name === t.name && e.message === t.message;
                 case "RegExp":
                     if (e.source !== t.source || e.global !== t.global || e.ignoreCase !== t.ignoreCase || e.multiline !== t.multiline || e.sticky !== t.sticky || e.unicode !== t.unicode) return !1
             }
             for (var i = n.length - 1; i >= 0;) {
                 if (n[i] === e) return r[i] === t;
                 i -= 1
             }
             switch (o) {
                 case "Map":
-                    return e.size === t.size && Cr(e.entries(), t.entries(), n.concat([e]), r.concat([t]));
+                    return e.size === t.size && Ar(e.entries(), t.entries(), n.concat([e]), r.concat([t]));
                 case "Set":
-                    return e.size === t.size && Cr(e.values(), t.values(), n.concat([e]), r.concat([t]));
+                    return e.size === t.size && Ar(e.values(), t.values(), n.concat([e]), r.concat([t]));
                 case "Arguments":
                 case "Array":
                 case "Object":
                 case "Boolean":
                 case "Number":
                 case "String":
                 case "Date":
@@ -3609,30 +3693,30 @@
                 case "Float32Array":
                 case "Float64Array":
                 case "ArrayBuffer":
                     break;
                 default:
                     return !1
             }
-            var l = Pr(e);
-            if (l.length !== Pr(t).length) return !1;
+            var l = Ir(e);
+            if (l.length !== Ir(t).length) return !1;
             var c = n.concat([e]),
                 u = r.concat([t]);
             for (i = l.length - 1; i >= 0;) {
                 var d = l[i];
-                if (!_r(d, t) || !Tr(t[d], e[d], c, u)) return !1;
+                if (!Pr(d, t) || !Fr(t[d], e[d], c, u)) return !1;
                 i -= 1
             }
             return !0
         }
-        const Sr = f((function(e, t) {
-            return Tr(e, t, [], [])
+        const Mr = f((function(e, t) {
+            return Fr(e, t, [], [])
         }));
 
-        function Rr(e, t) {
+        function Br(e, t) {
             return function(e, t, n) {
                 var r, a;
                 if ("function" == typeof e.indexOf) switch (typeof t) {
                     case "number":
                         if (0 === t) {
                             for (r = 1 / t; n < e.length;) {
                                 if (0 === (a = e[n]) && 1 / a === r) return n;
@@ -3653,23 +3737,23 @@
                     case "function":
                     case "undefined":
                         return e.indexOf(t, n);
                     case "object":
                         if (null === t) return e.indexOf(t, n)
                 }
                 for (; n < e.length;) {
-                    if (Sr(e[n], t)) return n;
+                    if (Mr(e[n], t)) return n;
                     n += 1
                 }
                 return -1
             }(t, e, 0) >= 0
         }
-        const Dr = f(Rr);
+        const zr = f(Br);
 
-        function Lr(e, t) {
+        function Kr(e, t) {
             switch (e) {
                 case 0:
                     return function() {
                         return t.apply(this, arguments)
                     };
                 case 1:
                     return function(e) {
@@ -3712,188 +3796,188 @@
                         return t.apply(this, arguments)
                     };
                 default:
                     throw new Error("First argument to _arity must be a non-negative integer no greater than ten")
             }
         }
 
-        function $r(e, t, n) {
+        function Hr(e, t, n) {
             return function() {
                 for (var r = [], a = 0, s = e, o = 0; o < t.length || a < arguments.length;) {
                     var i;
                     o < t.length && (!d(t[o]) || a >= arguments.length) ? i = t[o] : (i = arguments[a], a += 1), r[o] = i, d(i) || (s -= 1), o += 1
                 }
-                return s <= 0 ? n.apply(this, r) : Lr(s, $r(e, r, n))
+                return s <= 0 ? n.apply(this, r) : Kr(s, Hr(e, r, n))
             }
         }
-        const Ir = f((function(e, t) {
-                return 1 === e ? p(t) : Lr(e, $r(e, [], t))
+        const Ur = f((function(e, t) {
+                return 1 === e ? p(t) : Kr(e, Hr(e, [], t))
             })),
-            Ar = p((function(e) {
-                return Ir(e.length, (function(t, n) {
+            Wr = p((function(e) {
+                return Ur(e.length, (function(t, n) {
                     var r = Array.prototype.slice.call(arguments, 0);
                     return r[0] = n, r[1] = t, e.apply(this, r)
                 }))
             })),
-            Mr = Array.isArray || function(e) {
+            qr = Array.isArray || function(e) {
                 return null != e && e.length >= 0 && "[object Array]" === Object.prototype.toString.call(e)
             };
 
-        function Fr(e, t, n) {
+        function Vr(e, t, n) {
             return function() {
                 if (0 === arguments.length) return n();
                 var r = Array.prototype.slice.call(arguments, 0),
                     a = r.pop();
-                if (!Mr(a)) {
+                if (!qr(a)) {
                     for (var s = 0; s < e.length;) {
                         if ("function" == typeof a[e[s]]) return a[e[s]].apply(a, r);
                         s += 1
                     }
                     if (function(e) {
                             return null != e && "function" == typeof e["@@transducer/step"]
                         }(a)) return t.apply(null, r)(a)
                 }
                 return n.apply(this, arguments)
             }
         }
-        const Br = p((function(e) {
-            return !!Mr(e) || !!e && "object" == typeof e && ! function(e) {
+        const Gr = p((function(e) {
+            return !!qr(e) || !!e && "object" == typeof e && ! function(e) {
                 return "[object String]" === Object.prototype.toString.call(e)
             }(e) && (1 === e.nodeType ? !!e.length : 0 === e.length || e.length > 0 && e.hasOwnProperty(0) && e.hasOwnProperty(e.length - 1))
         }));
-        var zr = function() {
+        var Yr = function() {
             function e(e) {
                 this.f = e
             }
             return e.prototype["@@transducer/init"] = function() {
                 throw new Error("init not implemented on XWrap")
             }, e.prototype["@@transducer/result"] = function(e) {
                 return e
             }, e.prototype["@@transducer/step"] = function(e, t) {
                 return this.f(e, t)
             }, e
         }();
-        const Kr = f((function(e, t) {
-            return Lr(e.length, (function() {
+        const Xr = f((function(e, t) {
+            return Kr(e.length, (function() {
                 return e.apply(t, arguments)
             }))
         }));
 
-        function Hr(e, t, n) {
+        function Jr(e, t, n) {
             for (var r = n.next(); !r.done;) {
                 if ((t = e["@@transducer/step"](t, r.value)) && t["@@transducer/reduced"]) {
                     t = t["@@transducer/value"];
                     break
                 }
                 r = n.next()
             }
             return e["@@transducer/result"](t)
         }
 
-        function Wr(e, t, n, r) {
-            return e["@@transducer/result"](n[r](Kr(e["@@transducer/step"], e), t))
+        function Qr(e, t, n, r) {
+            return e["@@transducer/result"](n[r](Xr(e["@@transducer/step"], e), t))
         }
-        var Ur = "undefined" != typeof Symbol ? Symbol.iterator : "@@iterator";
-        const qr = function() {
+        var Zr = "undefined" != typeof Symbol ? Symbol.iterator : "@@iterator";
+        const ea = function() {
                 return this.xf["@@transducer/init"]()
             },
-            Vr = function(e) {
+            ta = function(e) {
                 return this.xf["@@transducer/result"](e)
             };
-        var Gr = function() {
+        var na = function() {
             function e(e, t) {
                 this.xf = t, this.f = e
             }
-            return e.prototype["@@transducer/init"] = qr, e.prototype["@@transducer/result"] = Vr, e.prototype["@@transducer/step"] = function(e, t) {
+            return e.prototype["@@transducer/init"] = ea, e.prototype["@@transducer/result"] = ta, e.prototype["@@transducer/step"] = function(e, t) {
                 return this.f(t) ? this.xf["@@transducer/step"](e, t) : e
             }, e
         }();
-        const Yr = f(Fr(["filter"], f((function(e, t) {
-                return new Gr(e, t)
+        const ra = f(Vr(["filter"], f((function(e, t) {
+                return new na(e, t)
             })), (function(e, t) {
                 return n = t, "[object Object]" === Object.prototype.toString.call(n) ? function(e, t, n) {
                     if ("function" == typeof e && (e = function(e) {
-                            return new zr(e)
-                        }(e)), Br(n)) return function(e, t, n) {
+                            return new Yr(e)
+                        }(e)), Gr(n)) return function(e, t, n) {
                         for (var r = 0, a = n.length; r < a;) {
                             if ((t = e["@@transducer/step"](t, n[r])) && t["@@transducer/reduced"]) {
                                 t = t["@@transducer/value"];
                                 break
                             }
                             r += 1
                         }
                         return e["@@transducer/result"](t)
                     }(e, t, n);
-                    if ("function" == typeof n["fantasy-land/reduce"]) return Wr(e, t, n, "fantasy-land/reduce");
-                    if (null != n[Ur]) return Hr(e, t, n[Ur]());
-                    if ("function" == typeof n.next) return Hr(e, t, n);
-                    if ("function" == typeof n.reduce) return Wr(e, t, n, "reduce");
+                    if ("function" == typeof n["fantasy-land/reduce"]) return Qr(e, t, n, "fantasy-land/reduce");
+                    if (null != n[Zr]) return Jr(e, t, n[Zr]());
+                    if ("function" == typeof n.next) return Jr(e, t, n);
+                    if ("function" == typeof n.reduce) return Qr(e, t, n, "reduce");
                     throw new TypeError("reduce: list must be array or iterable")
                 }((function(n, r) {
                     return e(t[r]) && (n[r] = t[r]), n
-                }), {}, Pr(t)) : function(e, t) {
+                }), {}, Ir(t)) : function(e, t) {
                     for (var n = 0, r = t.length, a = []; n < r;) e(t[n]) && (a[a.length] = t[n]), n += 1;
                     return a
                 }(e, t);
                 var n
             }))),
-            Xr = f((function(e, t) {
-                return Yr((n = e, function() {
+            aa = f((function(e, t) {
+                return ra((n = e, function() {
                     return !n.apply(this, arguments)
                 }), t);
                 var n
             })),
-            Jr = f((function(e, t) {
-                return Xr(Ar(Rr)(e), t)
+            sa = f((function(e, t) {
+                return aa(Wr(Br)(e), t)
             })),
-            Qr = f((function(e, t) {
+            oa = f((function(e, t) {
                 return function(e, t) {
                     var n;
                     t = t || [];
                     var r = (e = e || []).length,
                         a = t.length,
                         s = [];
                     for (n = 0; n < r;) s[s.length] = e[n], n += 1;
                     for (n = 0; n < a;) s[s.length] = t[n], n += 1;
                     return s
                 }(t, [e])
             }));
 
-        function Zr(e, t) {
+        function ia(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function ea(e) {
+        function la(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Zr(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Zr(Object(n)).forEach((function(t) {
+                t % 2 ? ia(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ia(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var ta = function(e) {
+        var ca = function(e) {
             var t = e.className,
                 n = e.class_name,
                 r = e.id,
                 a = e.options,
                 s = e.style,
                 o = e.key,
                 i = e.loading_state,
                 c = e.name,
-                u = Me(a).map((function(t) {
+                u = Ie(a).map((function(t) {
                     return function(t) {
                         var n = e.id,
                             r = e.inputClassName,
                             a = e.input_class_name,
                             s = e.inputCheckedClassName,
                             o = e.input_checked_class_name,
                             i = e.inputStyle,
@@ -3908,17 +3992,17 @@
                             v = e.label_style,
                             _ = e.labelCheckedStyle,
                             x = e.label_checked_style,
                             O = e.setProps,
                             w = e.inline,
                             N = e.value,
                             E = e.switch,
-                            j = Dr(t.value, N),
-                            k = j ? ea(ea({}, u || i), p || d) : u || i,
-                            P = j ? ea(ea({}, v || h), x || _) : v || h,
+                            j = zr(t.value, N),
+                            k = j ? la(la({}, u || i), p || d) : u || i,
+                            P = j ? la(la({}, v || h), x || _) : v || h,
                             C = t.input_id || "_dbcprivate_checklist_".concat(n, "_input_").concat(t.value);
                         return l().createElement("div", {
                             className: b()("form-check", w && "form-check-inline", E && "form-switch"),
                             key: t.value
                         }, l().createElement("input", {
                             id: C,
                             name: c,
@@ -3926,15 +4010,15 @@
                             checked: j,
                             className: b()("form-check-input", a || r, j && (o || s)),
                             disabled: Boolean(t.disabled),
                             style: k,
                             type: "checkbox",
                             onChange: function() {
                                 var e;
-                                e = Dr(t.value, N) ? Jr([t.value], N) : Qr(t.value, N), O({
+                                e = zr(t.value, N) ? sa([t.value], N) : oa(t.value, N), O({
                                     value: e
                                 })
                             }
                         }), l().createElement("label", {
                             id: t.label_id,
                             style: P,
                             className: b()("form-check-label", m || f, j && (y || g)),
@@ -3947,15 +4031,15 @@
                 id: r,
                 style: s,
                 className: n || t,
                 key: o,
                 "data-dash-is-loading": i && i.is_loading || void 0
             }, u)
         };
-        ta.propTypes = {
+        ca.propTypes = {
             options: u().oneOfType([u().arrayOf(u().oneOfType([u().string, u().number])), u().object, u().arrayOf(u().exact({
                 label: u().node.isRequired,
                 value: u().oneOfType([u().string, u().number]).isRequired,
                 disabled: u().bool,
                 input_id: u().string,
                 label_id: u().string
             }))]),
@@ -3989,39 +4073,39 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             name: u().string
-        }, ta.defaultProps = {
+        }, ca.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             options: [],
             value: [],
             persisted_props: ["value"],
             persistence_type: "local"
         };
-        const na = ta;
+        const ua = ca;
 
-        function ra({
+        function da({
             as: e,
             bsPrefix: t,
             className: n,
             ...r
         }) {
-            t = j(t, "col");
-            const a = k(),
-                s = P(),
+            t = E(t, "col");
+            const a = j(),
+                s = k(),
                 o = [],
                 i = [];
             return a.forEach((e => {
                 const n = r[e];
                 let a, l, c;
                 delete r[e], "object" == typeof n && null != n ? ({
                     span: a,
@@ -4035,122 +4119,122 @@
                 className: b()(n, ...o, ...i)
             }, {
                 as: e,
                 bsPrefix: t,
                 spans: o
             }]
         }
-        const aa = i.forwardRef(((e, t) => {
+        const pa = i.forwardRef(((e, t) => {
             const [{
                 className: n,
                 ...r
             }, {
                 as: a = "div",
                 bsPrefix: s,
                 spans: o
-            }] = ra(e);
+            }] = da(e);
             return (0, _.jsx)(a, {
                 ...r,
                 ref: t,
                 className: b()(n, !o.length && s)
             })
         }));
-        aa.displayName = "Col";
-        const sa = aa;
-        var oa = ["children", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "className", "class_name", "loading_state"],
-            ia = {
+        pa.displayName = "Col";
+        const fa = pa;
+        var ma = ["children", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "className", "class_name", "loading_state"],
+            ga = {
                 start: "align-self-start",
                 center: "align-self-center",
                 end: "align-self-end",
                 stretch: "align-self-stretch",
                 baseline: "align-self-baseline"
             },
-            la = function(t) {
+            ba = function(t) {
                 var n = t.children,
                     r = t.width,
                     a = t.xs,
                     s = t.sm,
                     i = t.md,
                     c = t.lg,
                     u = t.xl,
                     d = t.xxl,
                     p = t.align,
                     f = t.className,
                     g = t.class_name,
                     y = t.loading_state,
-                    h = o(t, oa);
+                    h = o(t, ma);
                 [r, a, s, i, c, u, d].forEach((function(e) {
-                    "object" === De(e) && null !== e && (e.span = e.size)
+                    "object" === Te(e) && null !== e && (e.span = e.size)
                 }));
-                var v = p && ia[p],
+                var v = p && ga[p],
                     _ = b()(g || f, v);
-                return l().createElement(sa, e({
+                return l().createElement(fa, e({
                     xs: a || r,
                     sm: s,
                     md: i,
                     lg: c,
                     xl: u,
                     xxl: d,
                     className: _
                 }, m(["setProps"], h), {
                     "data-dash-is-loading": y && y.is_loading || void 0
                 }), n)
             },
-            ca = u().oneOfType([u().number, u().string]),
-            ua = u().oneOfType([u().string, u().number, u().bool, u().shape({
+            ya = u().oneOfType([u().number, u().string]),
+            ha = u().oneOfType([u().string, u().number, u().bool, u().shape({
                 size: u().oneOfType([u().bool, u().number, u().string]),
-                order: ca,
-                offset: ca
+                order: ya,
+                offset: ya
             })]);
-        la.propTypes = {
+        ba.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
-            width: ua,
-            xs: ua,
-            sm: ua,
-            md: ua,
-            lg: ua,
-            xl: ua,
-            xxl: ua,
+            width: ha,
+            xs: ha,
+            sm: ha,
+            md: ha,
+            lg: ha,
+            xl: ha,
+            xxl: ha,
             align: u().oneOf(["start", "center", "end", "stretch", "baseline"]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const da = la;
-        var pa = ["children", "is_open", "navbar", "loading_state", "className", "class_name", "tag"],
-            fa = l().forwardRef((function(t, n) {
+        const va = ba;
+        var _a = ["children", "is_open", "navbar", "loading_state", "className", "class_name", "tag"],
+            xa = l().forwardRef((function(t, n) {
                 var r = t.children,
                     a = t.is_open,
                     s = t.navbar,
                     i = t.loading_state,
                     c = t.className,
                     u = t.class_name,
                     d = t.tag,
-                    p = o(t, pa);
-                return l().createElement(ge, e({
+                    p = o(t, _a);
+                return l().createElement(pe, e({
                     in: a,
                     as: d,
                     className: u || c
                 }, m(["setProps"], p), {
                     "data-dash-is-loading": i && i.is_loading || void 0
                 }), l().createElement("div", {
                     ref: n,
                     className: s && "navbar-collapse"
                 }, r))
             }));
-        fa.defaultProps = {
+        xa.defaultProps = {
             dimension: "height"
-        }, fa.propTypes = {
+        }, xa.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             is_open: u().bool,
@@ -4158,118 +4242,117 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             dimension: u().oneOf(["height", "width"])
         };
-        const ma = fa,
-            ga = i.forwardRef((({
+        const Oa = xa,
+            wa = i.forwardRef((({
                 bsPrefix: e,
-                fluid: t,
+                fluid: t = !1,
                 as: n = "div",
                 className: r,
                 ...a
             }, s) => {
-                const o = j(e, "container"),
+                const o = E(e, "container"),
                     i = "string" == typeof t ? `-${t}` : "-fluid";
                 return (0, _.jsx)(n, {
                     ref: s,
                     ...a,
                     className: b()(r, t ? `${o}${i}` : o)
                 })
             }));
-        ga.displayName = "Container", ga.defaultProps = {
-            fluid: !1
-        };
-        const ba = ga;
-        var ya = ["children", "loading_state", "className", "class_name", "tag"],
-            ha = function(t) {
+        wa.displayName = "Container";
+        const Na = wa;
+        var Ea = ["children", "loading_state", "className", "class_name", "tag"],
+            ja = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, ya);
-                return l().createElement(ba, e({
+                    c = o(t, Ea);
+                return l().createElement(Na, e({
                     as: i,
                     className: s || a
                 }, m(["setProps"], c), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        ha.propTypes = {
+        ja.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             fluid: u().oneOfType([u().bool, u().string]),
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const va = ha;
-        var _a = Function.prototype.bind.call(Function.prototype.call, [].slice);
+        const ka = ja;
+        var Pa = Function.prototype.bind.call(Function.prototype.call, [].slice);
 
-        function xa(e, t) {
-            return _a(e.querySelectorAll(t))
+        function Ca(e, t) {
+            return Pa(e.querySelectorAll(t))
         }
 
-        function Oa(e, t, n) {
+        function Ta(e, t, n) {
             const r = (0, i.useRef)(void 0 !== e),
                 [a, s] = (0, i.useState)(t),
                 o = void 0 !== e,
                 l = r.current;
-            return r.current = o, !o && l && a !== t && s(t), [o ? e : a, (0, i.useCallback)(((e, ...t) => {
-                n && n(e, ...t), s(e)
+            return r.current = o, !o && l && a !== t && s(t), [o ? e : a, (0, i.useCallback)(((...e) => {
+                const [t, ...r] = e;
+                let a = null == n ? void 0 : n(t, ...r);
+                return s(t), a
             }), [n])]
         }
 
-        function wa() {
-            return (0, i.useReducer)((function(e) {
-                return !e
-            }), !1)[1]
+        function Sa() {
+            const [, e] = (0, i.useReducer)((e => !e), !1);
+            return e
         }
-        const Na = i.createContext(null);
-        var Ea = Object.prototype.hasOwnProperty;
+        const Ra = i.createContext(null);
+        var Da = Object.prototype.hasOwnProperty;
 
-        function ja(e, t, n) {
+        function La(e, t, n) {
             for (n of e.keys())
-                if (ka(n, t)) return n
+                if ($a(n, t)) return n
         }
 
-        function ka(e, t) {
+        function $a(e, t) {
             var n, r, a;
             if (e === t) return !0;
             if (e && t && (n = e.constructor) === t.constructor) {
                 if (n === Date) return e.getTime() === t.getTime();
                 if (n === RegExp) return e.toString() === t.toString();
                 if (n === Array) {
                     if ((r = e.length) === t.length)
-                        for (; r-- && ka(e[r], t[r]););
+                        for (; r-- && $a(e[r], t[r]););
                     return -1 === r
                 }
                 if (n === Set) {
                     if (e.size !== t.size) return !1;
                     for (r of e) {
-                        if ((a = r) && "object" == typeof a && !(a = ja(t, a))) return !1;
+                        if ((a = r) && "object" == typeof a && !(a = La(t, a))) return !1;
                         if (!t.has(a)) return !1
                     }
                     return !0
                 }
                 if (n === Map) {
                     if (e.size !== t.size) return !1;
                     for (r of e) {
-                        if ((a = r[0]) && "object" == typeof a && !(a = ja(t, a))) return !1;
-                        if (!ka(r[1], t.get(a))) return !1
+                        if ((a = r[0]) && "object" == typeof a && !(a = La(t, a))) return !1;
+                        if (!$a(r[1], t.get(a))) return !1
                     }
                     return !0
                 }
                 if (n === ArrayBuffer) e = new Uint8Array(e), t = new Uint8Array(t);
                 else if (n === DataView) {
                     if ((r = e.byteLength) === t.byteLength)
                         for (; r-- && e.getInt8(r) === t.getInt8(r););
@@ -4278,70 +4361,70 @@
                 if (ArrayBuffer.isView(e)) {
                     if ((r = e.byteLength) === t.byteLength)
                         for (; r-- && e[r] === t[r];);
                     return -1 === r
                 }
                 if (!n || "object" == typeof e) {
                     for (n in r = 0, e) {
-                        if (Ea.call(e, n) && ++r && !Ea.call(t, n)) return !1;
-                        if (!(n in t) || !ka(e[n], t[n])) return !1
+                        if (Da.call(e, n) && ++r && !Da.call(t, n)) return !1;
+                        if (!(n in t) || !$a(e[n], t[n])) return !1
                     }
                     return Object.keys(t).length === r
                 }
             }
             return e != e && t != t
         }
 
-        function Pa(e) {
+        function Ia(e) {
             return e.split("-")[0]
         }
 
-        function Ca(e) {
+        function Aa(e) {
             if (null == e) return window;
             if ("[object Window]" !== e.toString()) {
                 var t = e.ownerDocument;
                 return t && t.defaultView || window
             }
             return e
         }
 
-        function Ta(e) {
-            return e instanceof Ca(e).Element || e instanceof Element
+        function Fa(e) {
+            return e instanceof Aa(e).Element || e instanceof Element
         }
 
-        function Sa(e) {
-            return e instanceof Ca(e).HTMLElement || e instanceof HTMLElement
+        function Ma(e) {
+            return e instanceof Aa(e).HTMLElement || e instanceof HTMLElement
         }
 
-        function Ra(e) {
-            return "undefined" != typeof ShadowRoot && (e instanceof Ca(e).ShadowRoot || e instanceof ShadowRoot)
+        function Ba(e) {
+            return "undefined" != typeof ShadowRoot && (e instanceof Aa(e).ShadowRoot || e instanceof ShadowRoot)
         }
-        var Da = Math.max,
-            La = Math.min,
-            $a = Math.round;
+        var za = Math.max,
+            Ka = Math.min,
+            Ha = Math.round;
 
-        function Ia() {
+        function Ua() {
             var e = navigator.userAgentData;
-            return null != e && e.brands ? e.brands.map((function(e) {
+            return null != e && e.brands && Array.isArray(e.brands) ? e.brands.map((function(e) {
                 return e.brand + "/" + e.version
             })).join(" ") : navigator.userAgent
         }
 
-        function Aa() {
-            return !/^((?!chrome|android).)*safari/i.test(Ia())
+        function Wa() {
+            return !/^((?!chrome|android).)*safari/i.test(Ua())
         }
 
-        function Ma(e, t, n) {
+        function qa(e, t, n) {
             void 0 === t && (t = !1), void 0 === n && (n = !1);
             var r = e.getBoundingClientRect(),
                 a = 1,
                 s = 1;
-            t && Sa(e) && (a = e.offsetWidth > 0 && $a(r.width) / e.offsetWidth || 1, s = e.offsetHeight > 0 && $a(r.height) / e.offsetHeight || 1);
-            var o = (Ta(e) ? Ca(e) : window).visualViewport,
-                i = !Aa() && n,
+            t && Ma(e) && (a = e.offsetWidth > 0 && Ha(r.width) / e.offsetWidth || 1, s = e.offsetHeight > 0 && Ha(r.height) / e.offsetHeight || 1);
+            var o = (Fa(e) ? Aa(e) : window).visualViewport,
+                i = !Wa() && n,
                 l = (r.left + (i && o ? o.offsetLeft : 0)) / a,
                 c = (r.top + (i && o ? o.offsetTop : 0)) / s,
                 u = r.width / a,
                 d = r.height / s;
             return {
                 width: u,
                 height: d,
@@ -4350,175 +4433,173 @@
                 bottom: c + d,
                 left: l,
                 x: l,
                 y: c
             }
         }
 
-        function Fa(e) {
-            var t = Ma(e),
+        function Va(e) {
+            var t = qa(e),
                 n = e.offsetWidth,
                 r = e.offsetHeight;
             return Math.abs(t.width - n) <= 1 && (n = t.width), Math.abs(t.height - r) <= 1 && (r = t.height), {
                 x: e.offsetLeft,
                 y: e.offsetTop,
                 width: n,
                 height: r
             }
         }
 
-        function Ba(e, t) {
+        function Ga(e, t) {
             var n = t.getRootNode && t.getRootNode();
             if (e.contains(t)) return !0;
-            if (n && Ra(n)) {
+            if (n && Ba(n)) {
                 var r = t;
                 do {
                     if (r && e.isSameNode(r)) return !0;
                     r = r.parentNode || r.host
                 } while (r)
             }
             return !1
         }
 
-        function za(e) {
+        function Ya(e) {
             return e ? (e.nodeName || "").toLowerCase() : null
         }
 
-        function Ka(e) {
-            return Ca(e).getComputedStyle(e)
+        function Xa(e) {
+            return Aa(e).getComputedStyle(e)
         }
 
-        function Ha(e) {
-            return ["table", "td", "th"].indexOf(za(e)) >= 0
+        function Ja(e) {
+            return ["table", "td", "th"].indexOf(Ya(e)) >= 0
         }
 
-        function Wa(e) {
-            return ((Ta(e) ? e.ownerDocument : e.document) || window.document).documentElement
+        function Qa(e) {
+            return ((Fa(e) ? e.ownerDocument : e.document) || window.document).documentElement
         }
 
-        function Ua(e) {
-            return "html" === za(e) ? e : e.assignedSlot || e.parentNode || (Ra(e) ? e.host : null) || Wa(e)
+        function Za(e) {
+            return "html" === Ya(e) ? e : e.assignedSlot || e.parentNode || (Ba(e) ? e.host : null) || Qa(e)
         }
 
-        function qa(e) {
-            return Sa(e) && "fixed" !== Ka(e).position ? e.offsetParent : null
+        function es(e) {
+            return Ma(e) && "fixed" !== Xa(e).position ? e.offsetParent : null
         }
 
-        function Va(e) {
-            for (var t = Ca(e), n = qa(e); n && Ha(n) && "static" === Ka(n).position;) n = qa(n);
-            return n && ("html" === za(n) || "body" === za(n) && "static" === Ka(n).position) ? t : n || function(e) {
-                var t = /firefox/i.test(Ia());
-                if (/Trident/i.test(Ia()) && Sa(e) && "fixed" === Ka(e).position) return null;
-                var n = Ua(e);
-                for (Ra(n) && (n = n.host); Sa(n) && ["html", "body"].indexOf(za(n)) < 0;) {
-                    var r = Ka(n);
+        function ts(e) {
+            for (var t = Aa(e), n = es(e); n && Ja(n) && "static" === Xa(n).position;) n = es(n);
+            return n && ("html" === Ya(n) || "body" === Ya(n) && "static" === Xa(n).position) ? t : n || function(e) {
+                var t = /firefox/i.test(Ua());
+                if (/Trident/i.test(Ua()) && Ma(e) && "fixed" === Xa(e).position) return null;
+                var n = Za(e);
+                for (Ba(n) && (n = n.host); Ma(n) && ["html", "body"].indexOf(Ya(n)) < 0;) {
+                    var r = Xa(n);
                     if ("none" !== r.transform || "none" !== r.perspective || "paint" === r.contain || -1 !== ["transform", "perspective"].indexOf(r.willChange) || t && "filter" === r.willChange || t && r.filter && "none" !== r.filter) return n;
                     n = n.parentNode
                 }
                 return null
             }(e) || t
         }
 
-        function Ga(e) {
+        function ns(e) {
             return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
         }
 
-        function Ya(e, t, n) {
-            return Da(e, La(t, n))
+        function rs(e, t, n) {
+            return za(e, Ka(t, n))
         }
 
-        function Xa(e) {
+        function as(e) {
             return Object.assign({}, {
                 top: 0,
                 right: 0,
                 bottom: 0,
                 left: 0
             }, e)
         }
 
-        function Ja(e, t) {
+        function ss(e, t) {
             return t.reduce((function(t, n) {
                 return t[n] = e, t
             }), {})
         }
-        var Qa = "top",
-            Za = "bottom",
-            es = "right",
-            ts = "left",
-            ns = "auto",
-            rs = [Qa, Za, es, ts],
-            as = "start",
-            ss = "end",
-            os = "clippingParents",
-            is = "viewport",
-            ls = "popper",
-            cs = "reference",
-            us = rs.reduce((function(e, t) {
-                return e.concat([t + "-" + as, t + "-" + ss])
+        var os = "top",
+            is = "bottom",
+            ls = "right",
+            cs = "left",
+            us = "auto",
+            ds = [os, is, ls, cs],
+            ps = "start",
+            fs = "end",
+            ms = "viewport",
+            gs = "popper",
+            bs = ds.reduce((function(e, t) {
+                return e.concat([t + "-" + ps, t + "-" + fs])
             }), []),
-            ds = [].concat(rs, [ns]).reduce((function(e, t) {
-                return e.concat([t, t + "-" + as, t + "-" + ss])
+            ys = [].concat(ds, [us]).reduce((function(e, t) {
+                return e.concat([t, t + "-" + ps, t + "-" + fs])
             }), []),
-            ps = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
-        const fs = {
+            hs = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+        const vs = {
             name: "arrow",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t, n = e.state,
                     r = e.name,
                     a = e.options,
                     s = n.elements.arrow,
                     o = n.modifiersData.popperOffsets,
-                    i = Pa(n.placement),
-                    l = Ga(i),
-                    c = [ts, es].indexOf(i) >= 0 ? "height" : "width";
+                    i = Ia(n.placement),
+                    l = ns(i),
+                    c = [cs, ls].indexOf(i) >= 0 ? "height" : "width";
                 if (s && o) {
                     var u = function(e, t) {
-                            return Xa("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
+                            return as("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
                                 placement: t.placement
-                            })) : e) ? e : Ja(e, rs))
+                            })) : e) ? e : ss(e, ds))
                         }(a.padding, n),
-                        d = Fa(s),
-                        p = "y" === l ? Qa : ts,
-                        f = "y" === l ? Za : es,
+                        d = Va(s),
+                        p = "y" === l ? os : cs,
+                        f = "y" === l ? is : ls,
                         m = n.rects.reference[c] + n.rects.reference[l] - o[l] - n.rects.popper[c],
                         g = o[l] - n.rects.reference[l],
-                        b = Va(s),
+                        b = ts(s),
                         y = b ? "y" === l ? b.clientHeight || 0 : b.clientWidth || 0 : 0,
                         h = m / 2 - g / 2,
                         v = u[p],
                         _ = y - d[c] - u[f],
                         x = y / 2 - d[c] / 2 + h,
-                        O = Ya(v, x, _),
+                        O = rs(v, x, _),
                         w = l;
                     n.modifiersData[r] = ((t = {})[w] = O, t.centerOffset = O - x, t)
                 }
             },
             effect: function(e) {
                 var t = e.state,
                     n = e.options.element,
                     r = void 0 === n ? "[data-popper-arrow]" : n;
-                null != r && ("string" != typeof r || (r = t.elements.popper.querySelector(r))) && Ba(t.elements.popper, r) && (t.elements.arrow = r)
+                null != r && ("string" != typeof r || (r = t.elements.popper.querySelector(r))) && Ga(t.elements.popper, r) && (t.elements.arrow = r)
             },
             requires: ["popperOffsets"],
             requiresIfExists: ["preventOverflow"]
         };
 
-        function ms(e) {
+        function _s(e) {
             return e.split("-")[1]
         }
-        var gs = {
+        var xs = {
             top: "auto",
             right: "auto",
             bottom: "auto",
             left: "auto"
         };
 
-        function bs(e) {
+        function Os(e) {
             var t, n = e.popper,
                 r = e.popperRect,
                 a = e.placement,
                 s = e.variation,
                 o = e.offsets,
                 i = e.position,
                 l = e.gpuAcceleration,
@@ -4535,399 +4616,399 @@
                 }) : {
                     x: f,
                     y: g
                 };
             f = b.x, g = b.y;
             var y = o.hasOwnProperty("x"),
                 h = o.hasOwnProperty("y"),
-                v = ts,
-                _ = Qa,
+                v = cs,
+                _ = os,
                 x = window;
             if (c) {
-                var O = Va(n),
+                var O = ts(n),
                     w = "clientHeight",
                     N = "clientWidth";
-                O === Ca(n) && "static" !== Ka(O = Wa(n)).position && "absolute" === i && (w = "scrollHeight", N = "scrollWidth"), (a === Qa || (a === ts || a === es) && s === ss) && (_ = Za, g -= (d && O === x && x.visualViewport ? x.visualViewport.height : O[w]) - r.height, g *= l ? 1 : -1), a !== ts && (a !== Qa && a !== Za || s !== ss) || (v = es, f -= (d && O === x && x.visualViewport ? x.visualViewport.width : O[N]) - r.width, f *= l ? 1 : -1)
+                O === Aa(n) && "static" !== Xa(O = Qa(n)).position && "absolute" === i && (w = "scrollHeight", N = "scrollWidth"), (a === os || (a === cs || a === ls) && s === fs) && (_ = is, g -= (d && O === x && x.visualViewport ? x.visualViewport.height : O[w]) - r.height, g *= l ? 1 : -1), a !== cs && (a !== os && a !== is || s !== fs) || (v = ls, f -= (d && O === x && x.visualViewport ? x.visualViewport.width : O[N]) - r.width, f *= l ? 1 : -1)
             }
             var E, j = Object.assign({
                     position: i
-                }, c && gs),
-                k = !0 === u ? function(e) {
-                    var t = e.x,
-                        n = e.y,
-                        r = window.devicePixelRatio || 1;
+                }, c && xs),
+                k = !0 === u ? function(e, t) {
+                    var n = e.x,
+                        r = e.y,
+                        a = t.devicePixelRatio || 1;
                     return {
-                        x: $a(t * r) / r || 0,
-                        y: $a(n * r) / r || 0
+                        x: Ha(n * a) / a || 0,
+                        y: Ha(r * a) / a || 0
                     }
                 }({
                     x: f,
                     y: g
-                }) : {
+                }, Aa(n)) : {
                     x: f,
                     y: g
                 };
             return f = k.x, g = k.y, l ? Object.assign({}, j, ((E = {})[_] = h ? "0" : "", E[v] = y ? "0" : "", E.transform = (x.devicePixelRatio || 1) <= 1 ? "translate(" + f + "px, " + g + "px)" : "translate3d(" + f + "px, " + g + "px, 0)", E)) : Object.assign({}, j, ((t = {})[_] = h ? g + "px" : "", t[v] = y ? f + "px" : "", t.transform = "", t))
         }
-        const ys = {
+        const ws = {
             name: "computeStyles",
             enabled: !0,
             phase: "beforeWrite",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = n.gpuAcceleration,
                     a = void 0 === r || r,
                     s = n.adaptive,
                     o = void 0 === s || s,
                     i = n.roundOffsets,
                     l = void 0 === i || i,
                     c = {
-                        placement: Pa(t.placement),
-                        variation: ms(t.placement),
+                        placement: Ia(t.placement),
+                        variation: _s(t.placement),
                         popper: t.elements.popper,
                         popperRect: t.rects.popper,
                         gpuAcceleration: a,
                         isFixed: "fixed" === t.options.strategy
                     };
-                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, bs(Object.assign({}, c, {
+                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, Os(Object.assign({}, c, {
                     offsets: t.modifiersData.popperOffsets,
                     position: t.options.strategy,
                     adaptive: o,
                     roundOffsets: l
-                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, bs(Object.assign({}, c, {
+                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, Os(Object.assign({}, c, {
                     offsets: t.modifiersData.arrow,
                     position: "absolute",
                     adaptive: !1,
                     roundOffsets: l
                 })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
                     "data-popper-placement": t.placement
                 })
             },
             data: {}
         };
-        var hs = {
+        var Ns = {
             passive: !0
         };
-        const vs = {
+        const Es = {
             name: "eventListeners",
             enabled: !0,
             phase: "write",
             fn: function() {},
             effect: function(e) {
                 var t = e.state,
                     n = e.instance,
                     r = e.options,
                     a = r.scroll,
                     s = void 0 === a || a,
                     o = r.resize,
                     i = void 0 === o || o,
-                    l = Ca(t.elements.popper),
+                    l = Aa(t.elements.popper),
                     c = [].concat(t.scrollParents.reference, t.scrollParents.popper);
                 return s && c.forEach((function(e) {
-                        e.addEventListener("scroll", n.update, hs)
-                    })), i && l.addEventListener("resize", n.update, hs),
+                        e.addEventListener("scroll", n.update, Ns)
+                    })), i && l.addEventListener("resize", n.update, Ns),
                     function() {
                         s && c.forEach((function(e) {
-                            e.removeEventListener("scroll", n.update, hs)
-                        })), i && l.removeEventListener("resize", n.update, hs)
+                            e.removeEventListener("scroll", n.update, Ns)
+                        })), i && l.removeEventListener("resize", n.update, Ns)
                     }
             },
             data: {}
         };
-        var _s = {
+        var js = {
             left: "right",
             right: "left",
             bottom: "top",
             top: "bottom"
         };
 
-        function xs(e) {
+        function ks(e) {
             return e.replace(/left|right|bottom|top/g, (function(e) {
-                return _s[e]
+                return js[e]
             }))
         }
-        var Os = {
+        var Ps = {
             start: "end",
             end: "start"
         };
 
-        function ws(e) {
+        function Cs(e) {
             return e.replace(/start|end/g, (function(e) {
-                return Os[e]
+                return Ps[e]
             }))
         }
 
-        function Ns(e) {
-            var t = Ca(e);
+        function Ts(e) {
+            var t = Aa(e);
             return {
                 scrollLeft: t.pageXOffset,
                 scrollTop: t.pageYOffset
             }
         }
 
-        function Es(e) {
-            return Ma(Wa(e)).left + Ns(e).scrollLeft
+        function Ss(e) {
+            return qa(Qa(e)).left + Ts(e).scrollLeft
         }
 
-        function js(e) {
-            var t = Ka(e),
+        function Rs(e) {
+            var t = Xa(e),
                 n = t.overflow,
                 r = t.overflowX,
                 a = t.overflowY;
             return /auto|scroll|overlay|hidden/.test(n + a + r)
         }
 
-        function ks(e) {
-            return ["html", "body", "#document"].indexOf(za(e)) >= 0 ? e.ownerDocument.body : Sa(e) && js(e) ? e : ks(Ua(e))
+        function Ds(e) {
+            return ["html", "body", "#document"].indexOf(Ya(e)) >= 0 ? e.ownerDocument.body : Ma(e) && Rs(e) ? e : Ds(Za(e))
         }
 
-        function Ps(e, t) {
+        function Ls(e, t) {
             var n;
             void 0 === t && (t = []);
-            var r = ks(e),
+            var r = Ds(e),
                 a = r === (null == (n = e.ownerDocument) ? void 0 : n.body),
-                s = Ca(r),
-                o = a ? [s].concat(s.visualViewport || [], js(r) ? r : []) : r,
+                s = Aa(r),
+                o = a ? [s].concat(s.visualViewport || [], Rs(r) ? r : []) : r,
                 i = t.concat(o);
-            return a ? i : i.concat(Ps(Ua(o)))
+            return a ? i : i.concat(Ls(Za(o)))
         }
 
-        function Cs(e) {
+        function $s(e) {
             return Object.assign({}, e, {
                 left: e.x,
                 top: e.y,
                 right: e.x + e.width,
                 bottom: e.y + e.height
             })
         }
 
-        function Ts(e, t, n) {
-            return t === is ? Cs(function(e, t) {
-                var n = Ca(e),
-                    r = Wa(e),
+        function Is(e, t, n) {
+            return t === ms ? $s(function(e, t) {
+                var n = Aa(e),
+                    r = Qa(e),
                     a = n.visualViewport,
                     s = r.clientWidth,
                     o = r.clientHeight,
                     i = 0,
                     l = 0;
                 if (a) {
                     s = a.width, o = a.height;
-                    var c = Aa();
+                    var c = Wa();
                     (c || !c && "fixed" === t) && (i = a.offsetLeft, l = a.offsetTop)
                 }
                 return {
                     width: s,
                     height: o,
-                    x: i + Es(e),
+                    x: i + Ss(e),
                     y: l
                 }
-            }(e, n)) : Ta(t) ? function(e, t) {
-                var n = Ma(e, !1, "fixed" === t);
+            }(e, n)) : Fa(t) ? function(e, t) {
+                var n = qa(e, !1, "fixed" === t);
                 return n.top = n.top + e.clientTop, n.left = n.left + e.clientLeft, n.bottom = n.top + e.clientHeight, n.right = n.left + e.clientWidth, n.width = e.clientWidth, n.height = e.clientHeight, n.x = n.left, n.y = n.top, n
-            }(t, n) : Cs(function(e) {
-                var t, n = Wa(e),
-                    r = Ns(e),
+            }(t, n) : $s(function(e) {
+                var t, n = Qa(e),
+                    r = Ts(e),
                     a = null == (t = e.ownerDocument) ? void 0 : t.body,
-                    s = Da(n.scrollWidth, n.clientWidth, a ? a.scrollWidth : 0, a ? a.clientWidth : 0),
-                    o = Da(n.scrollHeight, n.clientHeight, a ? a.scrollHeight : 0, a ? a.clientHeight : 0),
-                    i = -r.scrollLeft + Es(e),
+                    s = za(n.scrollWidth, n.clientWidth, a ? a.scrollWidth : 0, a ? a.clientWidth : 0),
+                    o = za(n.scrollHeight, n.clientHeight, a ? a.scrollHeight : 0, a ? a.clientHeight : 0),
+                    i = -r.scrollLeft + Ss(e),
                     l = -r.scrollTop;
-                return "rtl" === Ka(a || n).direction && (i += Da(n.clientWidth, a ? a.clientWidth : 0) - s), {
+                return "rtl" === Xa(a || n).direction && (i += za(n.clientWidth, a ? a.clientWidth : 0) - s), {
                     width: s,
                     height: o,
                     x: i,
                     y: l
                 }
-            }(Wa(e)))
+            }(Qa(e)))
         }
 
-        function Ss(e) {
+        function As(e) {
             var t, n = e.reference,
                 r = e.element,
                 a = e.placement,
-                s = a ? Pa(a) : null,
-                o = a ? ms(a) : null,
+                s = a ? Ia(a) : null,
+                o = a ? _s(a) : null,
                 i = n.x + n.width / 2 - r.width / 2,
                 l = n.y + n.height / 2 - r.height / 2;
             switch (s) {
-                case Qa:
+                case os:
                     t = {
                         x: i,
                         y: n.y - r.height
                     };
                     break;
-                case Za:
+                case is:
                     t = {
                         x: i,
                         y: n.y + n.height
                     };
                     break;
-                case es:
+                case ls:
                     t = {
                         x: n.x + n.width,
                         y: l
                     };
                     break;
-                case ts:
+                case cs:
                     t = {
                         x: n.x - r.width,
                         y: l
                     };
                     break;
                 default:
                     t = {
                         x: n.x,
                         y: n.y
                     }
             }
-            var c = s ? Ga(s) : null;
+            var c = s ? ns(s) : null;
             if (null != c) {
                 var u = "y" === c ? "height" : "width";
                 switch (o) {
-                    case as:
+                    case ps:
                         t[c] = t[c] - (n[u] / 2 - r[u] / 2);
                         break;
-                    case ss:
+                    case fs:
                         t[c] = t[c] + (n[u] / 2 - r[u] / 2)
                 }
             }
             return t
         }
 
-        function Rs(e, t) {
+        function Fs(e, t) {
             void 0 === t && (t = {});
             var n = t,
                 r = n.placement,
                 a = void 0 === r ? e.placement : r,
                 s = n.strategy,
                 o = void 0 === s ? e.strategy : s,
                 i = n.boundary,
-                l = void 0 === i ? os : i,
+                l = void 0 === i ? "clippingParents" : i,
                 c = n.rootBoundary,
-                u = void 0 === c ? is : c,
+                u = void 0 === c ? ms : c,
                 d = n.elementContext,
-                p = void 0 === d ? ls : d,
+                p = void 0 === d ? gs : d,
                 f = n.altBoundary,
                 m = void 0 !== f && f,
                 g = n.padding,
                 b = void 0 === g ? 0 : g,
-                y = Xa("number" != typeof b ? b : Ja(b, rs)),
-                h = p === ls ? cs : ls,
+                y = as("number" != typeof b ? b : ss(b, ds)),
+                h = p === gs ? "reference" : gs,
                 v = e.rects.popper,
                 _ = e.elements[m ? h : p],
                 x = function(e, t, n, r) {
                     var a = "clippingParents" === t ? function(e) {
-                            var t = Ps(Ua(e)),
-                                n = ["absolute", "fixed"].indexOf(Ka(e).position) >= 0 && Sa(e) ? Va(e) : e;
-                            return Ta(n) ? t.filter((function(e) {
-                                return Ta(e) && Ba(e, n) && "body" !== za(e)
+                            var t = Ls(Za(e)),
+                                n = ["absolute", "fixed"].indexOf(Xa(e).position) >= 0 && Ma(e) ? ts(e) : e;
+                            return Fa(n) ? t.filter((function(e) {
+                                return Fa(e) && Ga(e, n) && "body" !== Ya(e)
                             })) : []
                         }(e) : [].concat(t),
                         s = [].concat(a, [n]),
                         o = s[0],
                         i = s.reduce((function(t, n) {
-                            var a = Ts(e, n, r);
-                            return t.top = Da(a.top, t.top), t.right = La(a.right, t.right), t.bottom = La(a.bottom, t.bottom), t.left = Da(a.left, t.left), t
-                        }), Ts(e, o, r));
+                            var a = Is(e, n, r);
+                            return t.top = za(a.top, t.top), t.right = Ka(a.right, t.right), t.bottom = Ka(a.bottom, t.bottom), t.left = za(a.left, t.left), t
+                        }), Is(e, o, r));
                     return i.width = i.right - i.left, i.height = i.bottom - i.top, i.x = i.left, i.y = i.top, i
-                }(Ta(_) ? _ : _.contextElement || Wa(e.elements.popper), l, u, o),
-                O = Ma(e.elements.reference),
-                w = Ss({
+                }(Fa(_) ? _ : _.contextElement || Qa(e.elements.popper), l, u, o),
+                O = qa(e.elements.reference),
+                w = As({
                     reference: O,
                     element: v,
                     strategy: "absolute",
                     placement: a
                 }),
-                N = Cs(Object.assign({}, v, w)),
-                E = p === ls ? N : O,
+                N = $s(Object.assign({}, v, w)),
+                E = p === gs ? N : O,
                 j = {
                     top: x.top - E.top + y.top,
                     bottom: E.bottom - x.bottom + y.bottom,
                     left: x.left - E.left + y.left,
                     right: E.right - x.right + y.right
                 },
                 k = e.modifiersData.offset;
-            if (p === ls && k) {
+            if (p === gs && k) {
                 var P = k[a];
                 Object.keys(j).forEach((function(e) {
-                    var t = [es, Za].indexOf(e) >= 0 ? 1 : -1,
-                        n = [Qa, Za].indexOf(e) >= 0 ? "y" : "x";
+                    var t = [ls, is].indexOf(e) >= 0 ? 1 : -1,
+                        n = [os, is].indexOf(e) >= 0 ? "y" : "x";
                     j[e] += P[n] * t
                 }))
             }
             return j
         }
-        const Ds = {
+        const Ms = {
             name: "flip",
             enabled: !0,
             phase: "main",
             fn: function(e) {
                 var t = e.state,
                     n = e.options,
                     r = e.name;
                 if (!t.modifiersData[r]._skip) {
-                    for (var a = n.mainAxis, s = void 0 === a || a, o = n.altAxis, i = void 0 === o || o, l = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, p = n.altBoundary, f = n.flipVariations, m = void 0 === f || f, g = n.allowedAutoPlacements, b = t.options.placement, y = Pa(b), h = l || (y !== b && m ? function(e) {
-                            if (Pa(e) === ns) return [];
-                            var t = xs(e);
-                            return [ws(e), t, ws(t)]
-                        }(b) : [xs(b)]), v = [b].concat(h).reduce((function(e, n) {
-                            return e.concat(Pa(n) === ns ? function(e, t) {
+                    for (var a = n.mainAxis, s = void 0 === a || a, o = n.altAxis, i = void 0 === o || o, l = n.fallbackPlacements, c = n.padding, u = n.boundary, d = n.rootBoundary, p = n.altBoundary, f = n.flipVariations, m = void 0 === f || f, g = n.allowedAutoPlacements, b = t.options.placement, y = Ia(b), h = l || (y !== b && m ? function(e) {
+                            if (Ia(e) === us) return [];
+                            var t = ks(e);
+                            return [Cs(e), t, Cs(t)]
+                        }(b) : [ks(b)]), v = [b].concat(h).reduce((function(e, n) {
+                            return e.concat(Ia(n) === us ? function(e, t) {
                                 void 0 === t && (t = {});
                                 var n = t,
                                     r = n.placement,
                                     a = n.boundary,
                                     s = n.rootBoundary,
                                     o = n.padding,
                                     i = n.flipVariations,
                                     l = n.allowedAutoPlacements,
-                                    c = void 0 === l ? ds : l,
-                                    u = ms(r),
-                                    d = u ? i ? us : us.filter((function(e) {
-                                        return ms(e) === u
-                                    })) : rs,
+                                    c = void 0 === l ? ys : l,
+                                    u = _s(r),
+                                    d = u ? i ? bs : bs.filter((function(e) {
+                                        return _s(e) === u
+                                    })) : ds,
                                     p = d.filter((function(e) {
                                         return c.indexOf(e) >= 0
                                     }));
                                 0 === p.length && (p = d);
                                 var f = p.reduce((function(t, n) {
-                                    return t[n] = Rs(e, {
+                                    return t[n] = Fs(e, {
                                         placement: n,
                                         boundary: a,
                                         rootBoundary: s,
                                         padding: o
-                                    })[Pa(n)], t
+                                    })[Ia(n)], t
                                 }), {});
                                 return Object.keys(f).sort((function(e, t) {
                                     return f[e] - f[t]
                                 }))
                             }(t, {
                                 placement: n,
                                 boundary: u,
                                 rootBoundary: d,
                                 padding: c,
                                 flipVariations: m,
                                 allowedAutoPlacements: g
                             }) : n)
                         }), []), _ = t.rects.reference, x = t.rects.popper, O = new Map, w = !0, N = v[0], E = 0; E < v.length; E++) {
                         var j = v[E],
-                            k = Pa(j),
-                            P = ms(j) === as,
-                            C = [Qa, Za].indexOf(k) >= 0,
+                            k = Ia(j),
+                            P = _s(j) === ps,
+                            C = [os, is].indexOf(k) >= 0,
                             T = C ? "width" : "height",
-                            S = Rs(t, {
+                            S = Fs(t, {
                                 placement: j,
                                 boundary: u,
                                 rootBoundary: d,
                                 altBoundary: p,
                                 padding: c
                             }),
-                            R = C ? P ? es : ts : P ? Za : Qa;
-                        _[T] > x[T] && (R = xs(R));
-                        var D = xs(R),
+                            R = C ? P ? ls : cs : P ? is : os;
+                        _[T] > x[T] && (R = ks(R));
+                        var D = ks(R),
                             L = [];
                         if (s && L.push(S[k] <= 0), i && L.push(S[R] <= 0, S[D] <= 0), L.every((function(e) {
                                 return e
                             }))) {
                             N = j, w = !1;
                             break
                         }
@@ -4948,67 +5029,67 @@
             },
             requiresIfExists: ["offset"],
             data: {
                 _skip: !1
             }
         };
 
-        function Ls(e, t, n) {
+        function Bs(e, t, n) {
             return void 0 === n && (n = {
                 x: 0,
                 y: 0
             }), {
                 top: e.top - t.height - n.y,
                 right: e.right - t.width + n.x,
                 bottom: e.bottom - t.height + n.y,
                 left: e.left - t.width - n.x
             }
         }
 
-        function $s(e) {
-            return [Qa, es, Za, ts].some((function(t) {
+        function zs(e) {
+            return [os, ls, is, cs].some((function(t) {
                 return e[t] >= 0
             }))
         }
-        const Is = {
+        const Ks = {
                 name: "offset",
                 enabled: !0,
                 phase: "main",
                 requires: ["popperOffsets"],
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         r = e.name,
                         a = n.offset,
                         s = void 0 === a ? [0, 0] : a,
-                        o = ds.reduce((function(e, n) {
+                        o = ys.reduce((function(e, n) {
                             return e[n] = function(e, t, n) {
-                                var r = Pa(e),
-                                    a = [ts, Qa].indexOf(r) >= 0 ? -1 : 1,
+                                var r = Ia(e),
+                                    a = [cs, os].indexOf(r) >= 0 ? -1 : 1,
                                     s = "function" == typeof n ? n(Object.assign({}, t, {
                                         placement: e
                                     })) : n,
                                     o = s[0],
                                     i = s[1];
-                                return o = o || 0, i = (i || 0) * a, [ts, es].indexOf(r) >= 0 ? {
+                                return o = o || 0, i = (i || 0) * a, [cs, ls].indexOf(r) >= 0 ? {
                                     x: i,
                                     y: o
                                 } : {
                                     x: o,
                                     y: i
                                 }
                             }(n, t.rects, s), e
                         }), {}),
                         i = o[t.placement],
                         l = i.x,
                         c = i.y;
                     null != t.modifiersData.popperOffsets && (t.modifiersData.popperOffsets.x += l, t.modifiersData.popperOffsets.y += c), t.modifiersData[r] = o
                 }
             },
-            As = {
+            Hs = {
                 name: "preventOverflow",
                 enabled: !0,
                 phase: "main",
                 fn: function(e) {
                     var t = e.state,
                         n = e.options,
                         r = e.name,
@@ -5020,24 +5101,24 @@
                         c = n.rootBoundary,
                         u = n.altBoundary,
                         d = n.padding,
                         p = n.tether,
                         f = void 0 === p || p,
                         m = n.tetherOffset,
                         g = void 0 === m ? 0 : m,
-                        b = Rs(t, {
+                        b = Fs(t, {
                             boundary: l,
                             rootBoundary: c,
                             padding: d,
                             altBoundary: u
                         }),
-                        y = Pa(t.placement),
-                        h = ms(t.placement),
+                        y = Ia(t.placement),
+                        h = _s(t.placement),
                         v = !h,
-                        _ = Ga(y),
+                        _ = ns(y),
                         x = "x" === _ ? "y" : "x",
                         O = t.modifiersData.popperOffsets,
                         w = t.rects.reference,
                         N = t.rects.popper,
                         E = "function" == typeof g ? g(Object.assign({}, t.rects, {
                             placement: t.placement
                         })) : g,
@@ -5051,100 +5132,100 @@
                         k = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
                         P = {
                             x: 0,
                             y: 0
                         };
                     if (O) {
                         if (s) {
-                            var C, T = "y" === _ ? Qa : ts,
-                                S = "y" === _ ? Za : es,
+                            var C, T = "y" === _ ? os : cs,
+                                S = "y" === _ ? is : ls,
                                 R = "y" === _ ? "height" : "width",
                                 D = O[_],
                                 L = D + b[T],
                                 $ = D - b[S],
                                 I = f ? -N[R] / 2 : 0,
-                                A = h === as ? w[R] : N[R],
-                                M = h === as ? -N[R] : -w[R],
-                                F = t.elements.arrow,
-                                B = f && F ? Fa(F) : {
+                                A = h === ps ? w[R] : N[R],
+                                F = h === ps ? -N[R] : -w[R],
+                                M = t.elements.arrow,
+                                B = f && M ? Va(M) : {
                                     width: 0,
                                     height: 0
                                 },
                                 z = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
                                     top: 0,
                                     right: 0,
                                     bottom: 0,
                                     left: 0
                                 },
                                 K = z[T],
                                 H = z[S],
-                                W = Ya(0, w[R], B[R]),
-                                U = v ? w[R] / 2 - I - W - K - j.mainAxis : A - W - K - j.mainAxis,
-                                q = v ? -w[R] / 2 + I + W + H + j.mainAxis : M + W + H + j.mainAxis,
-                                V = t.elements.arrow && Va(t.elements.arrow),
+                                U = rs(0, w[R], B[R]),
+                                W = v ? w[R] / 2 - I - U - K - j.mainAxis : A - U - K - j.mainAxis,
+                                q = v ? -w[R] / 2 + I + U + H + j.mainAxis : F + U + H + j.mainAxis,
+                                V = t.elements.arrow && ts(t.elements.arrow),
                                 G = V ? "y" === _ ? V.clientTop || 0 : V.clientLeft || 0 : 0,
                                 Y = null != (C = null == k ? void 0 : k[_]) ? C : 0,
                                 X = D + q - Y,
-                                J = Ya(f ? La(L, D + U - Y - G) : L, D, f ? Da($, X) : $);
+                                J = rs(f ? Ka(L, D + W - Y - G) : L, D, f ? za($, X) : $);
                             O[_] = J, P[_] = J - D
                         }
                         if (i) {
-                            var Q, Z = "x" === _ ? Qa : ts,
-                                ee = "x" === _ ? Za : es,
+                            var Q, Z = "x" === _ ? os : cs,
+                                ee = "x" === _ ? is : ls,
                                 te = O[x],
                                 ne = "y" === x ? "height" : "width",
                                 re = te + b[Z],
                                 ae = te - b[ee],
-                                se = -1 !== [Qa, ts].indexOf(y),
+                                se = -1 !== [os, cs].indexOf(y),
                                 oe = null != (Q = null == k ? void 0 : k[x]) ? Q : 0,
                                 ie = se ? re : te - w[ne] - N[ne] - oe + j.altAxis,
                                 le = se ? te + w[ne] + N[ne] - oe - j.altAxis : ae,
                                 ce = f && se ? function(e, t, n) {
-                                    var r = Ya(e, t, n);
+                                    var r = rs(e, t, n);
                                     return r > n ? n : r
-                                }(ie, te, le) : Ya(f ? ie : re, te, f ? le : ae);
+                                }(ie, te, le) : rs(f ? ie : re, te, f ? le : ae);
                             O[x] = ce, P[x] = ce - te
                         }
                         t.modifiersData[r] = P
                     }
                 },
                 requiresIfExists: ["offset"]
             };
 
-        function Ms(e, t, n) {
+        function Us(e, t, n) {
             void 0 === n && (n = !1);
-            var r, a, s = Sa(t),
-                o = Sa(t) && function(e) {
+            var r, a, s = Ma(t),
+                o = Ma(t) && function(e) {
                     var t = e.getBoundingClientRect(),
-                        n = $a(t.width) / e.offsetWidth || 1,
-                        r = $a(t.height) / e.offsetHeight || 1;
+                        n = Ha(t.width) / e.offsetWidth || 1,
+                        r = Ha(t.height) / e.offsetHeight || 1;
                     return 1 !== n || 1 !== r
                 }(t),
-                i = Wa(t),
-                l = Ma(e, o, n),
+                i = Qa(t),
+                l = qa(e, o, n),
                 c = {
                     scrollLeft: 0,
                     scrollTop: 0
                 },
                 u = {
                     x: 0,
                     y: 0
                 };
-            return (s || !s && !n) && (("body" !== za(t) || js(i)) && (c = (r = t) !== Ca(r) && Sa(r) ? {
+            return (s || !s && !n) && (("body" !== Ya(t) || Rs(i)) && (c = (r = t) !== Aa(r) && Ma(r) ? {
                 scrollLeft: (a = r).scrollLeft,
                 scrollTop: a.scrollTop
-            } : Ns(r)), Sa(t) ? ((u = Ma(t, !0)).x += t.clientLeft, u.y += t.clientTop) : i && (u.x = Es(i))), {
+            } : Ts(r)), Ma(t) ? ((u = qa(t, !0)).x += t.clientLeft, u.y += t.clientTop) : i && (u.x = Ss(i))), {
                 x: l.left + c.scrollLeft - u.x,
                 y: l.top + c.scrollTop - u.y,
                 width: l.width,
                 height: l.height
             }
         }
 
-        function Fs(e) {
+        function Ws(e) {
             var t = new Map,
                 n = new Set,
                 r = [];
 
             function a(e) {
                 n.add(e.name), [].concat(e.requires || [], e.requiresIfExists || []).forEach((function(e) {
                     if (!n.has(e)) {
@@ -5155,39 +5236,39 @@
             }
             return e.forEach((function(e) {
                 t.set(e.name, e)
             })), e.forEach((function(e) {
                 n.has(e.name) || a(e)
             })), r
         }
-        var Bs = {
+        var qs = {
             placement: "bottom",
             modifiers: [],
             strategy: "absolute"
         };
 
-        function zs() {
+        function Vs() {
             for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
             return !t.some((function(e) {
                 return !(e && "function" == typeof e.getBoundingClientRect)
             }))
         }
-        const Ks = function(e) {
+        const Gs = function(e) {
                 void 0 === e && (e = {});
                 var t = e,
                     n = t.defaultModifiers,
                     r = void 0 === n ? [] : n,
                     a = t.defaultOptions,
-                    s = void 0 === a ? Bs : a;
+                    s = void 0 === a ? qs : a;
                 return function(e, t, n) {
                     void 0 === n && (n = s);
                     var a, o, i = {
                             placement: "bottom",
                             orderedModifiers: [],
-                            options: Object.assign({}, Bs, s),
+                            options: Object.assign({}, qs, s),
                             modifiersData: {},
                             elements: {
                                 reference: e,
                                 popper: t
                             },
                             attributes: {},
                             styles: {}
@@ -5195,20 +5276,20 @@
                         l = [],
                         c = !1,
                         u = {
                             state: i,
                             setOptions: function(n) {
                                 var a = "function" == typeof n ? n(i.options) : n;
                                 d(), i.options = Object.assign({}, s, i.options, a), i.scrollParents = {
-                                    reference: Ta(e) ? Ps(e) : e.contextElement ? Ps(e.contextElement) : [],
-                                    popper: Ps(t)
+                                    reference: Fa(e) ? Ls(e) : e.contextElement ? Ls(e.contextElement) : [],
+                                    popper: Ls(t)
                                 };
                                 var o, c, p = function(e) {
-                                    var t = Fs(e);
-                                    return ps.reduce((function(e, n) {
+                                    var t = Ws(e);
+                                    return hs.reduce((function(e, n) {
                                         return e.concat(t.filter((function(e) {
                                             return e.phase === n
                                         })))
                                     }), [])
                                 }((o = [].concat(r, i.options.modifiers), c = o.reduce((function(e, t) {
                                     var n = e[t.name];
                                     return e[t.name] = n ? Object.assign({}, n, t, {
@@ -5237,18 +5318,18 @@
                                 })), u.update()
                             },
                             forceUpdate: function() {
                                 if (!c) {
                                     var e = i.elements,
                                         t = e.reference,
                                         n = e.popper;
-                                    if (zs(t, n)) {
+                                    if (Vs(t, n)) {
                                         i.rects = {
-                                            reference: Ms(t, Va(n), "fixed" === i.options.strategy),
-                                            popper: Fa(n)
+                                            reference: Us(t, ts(n), "fixed" === i.options.strategy),
+                                            popper: Va(n)
                                         }, i.reset = !1, i.placement = i.options.placement, i.orderedModifiers.forEach((function(e) {
                                             return i.modifiersData[e.name] = Object.assign({}, e.data)
                                         }));
                                         for (var r = 0; r < i.orderedModifiers.length; r++)
                                             if (!0 !== i.reset) {
                                                 var a = i.orderedModifiers[r],
                                                     s = a.fn,
@@ -5276,15 +5357,15 @@
                                     }))
                                 }))), o
                             }),
                             destroy: function() {
                                 d(), c = !0
                             }
                         };
-                    if (!zs(e, t)) return u;
+                    if (!Vs(e, t)) return u;
 
                     function d() {
                         l.forEach((function(e) {
                             return e()
                         })), l = []
                     }
                     return u.setOptions(n).then((function(e) {
@@ -5299,24 +5380,24 @@
                     requiresIfExists: ["preventOverflow"],
                     fn: function(e) {
                         var t = e.state,
                             n = e.name,
                             r = t.rects.reference,
                             a = t.rects.popper,
                             s = t.modifiersData.preventOverflow,
-                            o = Rs(t, {
+                            o = Fs(t, {
                                 elementContext: "reference"
                             }),
-                            i = Rs(t, {
+                            i = Fs(t, {
                                 altBoundary: !0
                             }),
-                            l = Ls(o, r),
-                            c = Ls(i, a, s),
-                            u = $s(l),
-                            d = $s(c);
+                            l = Bs(o, r),
+                            c = Bs(i, a, s),
+                            u = zs(l),
+                            d = zs(c);
                         t.modifiersData[n] = {
                             referenceClippingOffsets: l,
                             popperEscapeOffsets: c,
                             isReferenceHidden: u,
                             hasPopperEscaped: d
                         }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
                             "data-popper-reference-hidden": u,
@@ -5326,32 +5407,32 @@
                 }, {
                     name: "popperOffsets",
                     enabled: !0,
                     phase: "read",
                     fn: function(e) {
                         var t = e.state,
                             n = e.name;
-                        t.modifiersData[n] = Ss({
+                        t.modifiersData[n] = As({
                             reference: t.rects.reference,
                             element: t.rects.popper,
                             strategy: "absolute",
                             placement: t.placement
                         })
                     },
                     data: {}
-                }, ys, vs, Is, Ds, As, fs]
+                }, ws, Es, Ks, Ms, Hs, vs]
             }),
-            Hs = ["enabled", "placement", "strategy", "modifiers"],
-            Ws = {
+            Ys = ["enabled", "placement", "strategy", "modifiers"],
+            Xs = {
                 name: "applyStyles",
                 enabled: !1,
                 phase: "afterWrite",
                 fn: () => {}
             },
-            Us = {
+            Js = {
                 name: "ariaDescribedBy",
                 enabled: !0,
                 phase: "afterWrite",
                 effect: ({
                     state: e
                 }) => () => {
                     const {
@@ -5374,50 +5455,53 @@
                     if (n.id && "tooltip" === a && "setAttribute" in r) {
                         const e = r.getAttribute("aria-describedby");
                         if (e && -1 !== e.split(",").indexOf(n.id)) return;
                         r.setAttribute("aria-describedby", e ? `${e},${n.id}` : n.id)
                     }
                 }
             },
-            qs = [],
-            Vs = function(e, t, n = {}) {
+            Qs = [],
+            Zs = function(e, t, n = {}) {
                 let {
                     enabled: r = !0,
                     placement: a = "bottom",
                     strategy: s = "absolute",
-                    modifiers: o = qs
+                    modifiers: o = Qs
                 } = n, l = function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(n, Hs);
+                }(n, Ys);
                 const c = (0, i.useRef)(o),
                     u = (0, i.useRef)(),
                     d = (0, i.useCallback)((() => {
                         var e;
                         null == (e = u.current) || e.update()
                     }), []),
                     p = (0, i.useCallback)((() => {
                         var e;
                         null == (e = u.current) || e.forceUpdate()
                     }), []),
-                    [f, m] = (y = (0, i.useState)({
+                    [f, m] = function(e) {
+                        const t = tt();
+                        return [e[0], (0, i.useCallback)((n => {
+                            if (t()) return e[1](n)
+                        }), [t, e[1]])]
+                    }((0, i.useState)({
                         placement: a,
                         update: d,
                         forceUpdate: p,
                         attributes: {},
                         styles: {
                             popper: {},
                             arrow: {}
                         }
-                    }), h = Qe(), [y[0], (0, i.useCallback)((function(e) {
-                        if (h()) return y[1](e)
-                    }), [h, y[1]])]),
+                    })),
                     g = (0, i.useMemo)((() => ({
                         name: "updateStateModifier",
                         enabled: !0,
                         phase: "write",
                         requires: ["computeStyles"],
                         fn: ({
                             state: e
@@ -5432,92 +5516,93 @@
                                 attributes: n,
                                 update: d,
                                 forceUpdate: p,
                                 placement: e.placement
                             })
                         }
                     })), [d, p, m]),
-                    b = (0, i.useMemo)((() => (ka(c.current, o) || (c.current = o), c.current)), [o]);
-                var y, h;
+                    b = (0, i.useMemo)((() => ($a(c.current, o) || (c.current = o), c.current)), [o]);
                 return (0, i.useEffect)((() => {
                     u.current && r && u.current.setOptions({
                         placement: a,
                         strategy: s,
-                        modifiers: [...b, g, Ws]
+                        modifiers: [...b, g, Xs]
                     })
                 }), [s, a, g, r, b]), (0, i.useEffect)((() => {
-                    if (r && null != e && null != t) return u.current = Ks(e, t, Object.assign({}, l, {
+                    if (r && null != e && null != t) return u.current = Gs(e, t, Object.assign({}, l, {
                         placement: a,
                         strategy: s,
-                        modifiers: [...b, Us, g]
+                        modifiers: [...b, Js, g]
                     })), () => {
                         null != u.current && (u.current.destroy(), u.current = void 0, m((e => Object.assign({}, e, {
                             attributes: {},
                             styles: {
                                 popper: {}
                             }
                         }))))
                     }
                 }), [r, e, t]), f
             };
 
-        function Gs(e, t) {
+        function eo(e, t) {
             return e.contains ? e.contains(t) : e.compareDocumentPosition ? e === t || !!(16 & e.compareDocumentPosition(t)) : void 0
         }
-        var Ys = n(3),
-            Xs = n.n(Ys);
-        const Js = () => {},
-            Qs = e => e && ("current" in e ? e.current : e),
-            Zs = {
+        var to = n(2),
+            no = n.n(to);
+        const ro = () => {},
+            ao = e => e && ("current" in e ? e.current : e),
+            so = {
                 click: "mousedown",
                 mouseup: "mousedown",
                 pointerup: "pointerdown"
             },
-            eo = function(e, t = Js, {
+            oo = function(e, t = ro, {
                 disabled: n,
                 clickTrigger: r = "click"
             } = {}) {
                 const a = (0, i.useRef)(!1),
                     s = (0, i.useRef)(!1),
                     o = (0, i.useCallback)((t => {
-                        const n = Qs(e);
+                        const n = ao(e);
                         var r;
-                        Xs()(!!n, "ClickOutside captured a close event but does not have a ref to compare it to. useClickOutside(), should be passed a ref that resolves to a DOM node"), a.current = !n || !!((r = t).metaKey || r.altKey || r.ctrlKey || r.shiftKey) || ! function(e) {
+                        no()(!!n, "ClickOutside captured a close event but does not have a ref to compare it to. useClickOutside(), should be passed a ref that resolves to a DOM node"), a.current = !n || !!((r = t).metaKey || r.altKey || r.ctrlKey || r.shiftKey) || ! function(e) {
                             return 0 === e.button
-                        }(t) || !!Gs(n, t.target) || s.current, s.current = !1
+                        }(t) || !!eo(n, t.target) || s.current, s.current = !1
                     }), [e]),
-                    l = Xe((t => {
-                        const n = Qs(e);
-                        n && Gs(n, t.target) && (s.current = !0)
+                    l = Ye((t => {
+                        const n = ao(e);
+                        n && eo(n, t.target) && (s.current = !0)
                     })),
-                    c = Xe((e => {
+                    c = Ye((e => {
                         a.current || t(e)
                     }));
                 (0, i.useEffect)((() => {
+                    var t, a;
                     if (n || null == e) return;
-                    const t = T(Qs(e));
-                    let a = (t.defaultView || window).event,
-                        s = null;
-                    Zs[r] && (s = ee(t, Zs[r], l, !0));
-                    const i = ee(t, r, o, !0),
-                        u = ee(t, r, (e => {
-                            e !== a ? c(e) : a = void 0
+                    const s = C(ao(e)),
+                        i = s.defaultView || window;
+                    let u = null != (t = i.event) ? t : null == (a = i.parent) ? void 0 : a.event,
+                        d = null;
+                    so[r] && (d = Z(s, so[r], l, !0));
+                    const p = Z(s, r, o, !0),
+                        f = Z(s, r, (e => {
+                            e !== u ? c(e) : u = void 0
                         }));
-                    let d = [];
-                    return "ontouchstart" in t.documentElement && (d = [].slice.call(t.body.children).map((e => ee(e, "mousemove", Js)))), () => {
-                        null == s || s(), i(), u(), d.forEach((e => e()))
+                    let m = [];
+                    return "ontouchstart" in s.documentElement && (m = [].slice.call(s.body.children).map((e => Z(e, "mousemove", ro)))), () => {
+                        null == d || d(), p(), f(), m.forEach((e => e()))
                     }
                 }), [e, n, r, o, l, c])
             };
 
-        function to(e = {}) {
+        function io(e = {}) {
             return Array.isArray(e) ? e : Object.keys(e).map((t => (e[t].name = t, e[t])))
         }
 
-        function no({
+        function lo({
             enabled: e,
             enableEvents: t,
             placement: n,
             flip: r,
             offset: a,
             fixed: s,
             containerPadding: o,
@@ -5531,15 +5616,15 @@
                     t[e.name] = e
                 })), t) : e || t
             }(l.modifiers);
             return Object.assign({}, l, {
                 placement: n,
                 enabled: e,
                 strategy: s ? "fixed" : l.strategy,
-                modifiers: to(Object.assign({}, m, {
+                modifiers: io(Object.assign({}, m, {
                     eventListeners: {
                         enabled: t,
                         options: null == (c = m.eventListeners) ? void 0 : c.options
                     },
                     preventOverflow: Object.assign({}, m.preventOverflow, {
                         options: o ? Object.assign({
                             padding: o
@@ -5558,20 +5643,20 @@
                     }),
                     flip: Object.assign({
                         enabled: !!r
                     }, m.flip)
                 }))
             })
         }
-        const ro = ["children"],
-            ao = () => {};
+        const co = ["children"],
+            uo = () => {};
 
-        function so(e = {}) {
-            const t = (0, i.useContext)(Na),
-                [n, r] = Je(),
+        function po(e = {}) {
+            const t = (0, i.useContext)(Ra),
+                [n, r] = et(),
                 a = (0, i.useRef)(!1),
                 {
                     flip: s,
                     offset: o,
                     rootCloseEvent: l,
                     fixed: c = !1,
                     placement: u,
@@ -5582,25 +5667,25 @@
                 m = null == (null == t ? void 0 : t.show) ? !!e.show : t.show;
             m && !a.current && (a.current = !0);
             const {
                 placement: g,
                 setMenu: b,
                 menuElement: y,
                 toggleElement: h
-            } = t || {}, v = Vs(h, y, no({
+            } = t || {}, v = Zs(h, y, lo({
                 placement: u || g || "bottom-start",
                 enabled: f,
                 enableEvents: null == p ? m : p,
                 offset: o,
                 flip: s,
                 fixed: c,
                 arrowElement: n,
                 popperConfig: d
             })), _ = Object.assign({
-                ref: b || ao,
+                ref: b || uo,
                 "aria-labelledby": null == h ? void 0 : h.id
             }, v.attributes.popper, {
                 style: v.styles.popper
             }), x = {
                 show: m,
                 placement: g,
                 hasShown: a.current,
@@ -5608,400 +5693,453 @@
                 popper: f ? v : null,
                 arrowProps: f ? Object.assign({
                     ref: r
                 }, v.attributes.arrow, {
                     style: v.styles.arrow
                 }) : {}
             };
-            return eo(y, (e => {
+            return oo(y, (e => {
                 null == t || t.toggle(!1, e)
             }), {
                 clickTrigger: l,
                 disabled: !m
             }), [_, x]
         }
 
-        function oo(e) {
+        function fo(e) {
             let {
                 children: t
             } = e, n = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, ro);
-            const [r, a] = so(n);
+            }(e, co);
+            const [r, a] = po(n);
             return (0, _.jsx)(_.Fragment, {
                 children: t(r, a)
             })
         }
-        oo.displayName = "DropdownMenu", oo.defaultProps = {
+        fo.displayName = "DropdownMenu", fo.defaultProps = {
             usePopper: !0
         };
-        const io = oo,
-            lo = {
+        const mo = fo,
+            go = {
                 prefix: String(Math.round(1e10 * Math.random())),
                 current: 0
             },
-            co = i.createContext(lo);
-        let uo = Boolean("undefined" != typeof window && window.document && window.document.createElement),
-            po = new WeakMap;
-
-        function fo(e) {
-            let t = (0, i.useContext)(co);
-            t !== lo || uo || console.warn("When server rendering, you must wrap your application in an <SSRProvider> to ensure consistent ids are generated between the client and server.");
+            bo = i.createContext(go),
+            yo = i.createContext(!1);
+        let ho = Boolean("undefined" != typeof window && window.document && window.document.createElement),
+            vo = new WeakMap;
+        const _o = "function" == typeof i.useId ? function(e) {
+            let t = i.useId(),
+                [n] = (0, i.useState)("function" == typeof i.useSyncExternalStore ? i.useSyncExternalStore(wo, xo, Oo) : (0, i.useContext)(yo));
+            return e || `${n?"react-aria":`react-aria${go.prefix}`}-${t}`
+        } : function(e) {
+            let t = (0, i.useContext)(bo);
+            t !== go || ho || console.warn("When server rendering, you must wrap your application in an <SSRProvider> to ensure consistent ids are generated between the client and server.");
             let n = function(e = !1) {
-                let t = (0, i.useContext)(co),
-                    n = (0, i.useRef)(null);
-                if (null === n.current && !e) {
-                    var r, a;
-                    let e = null === (r = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED) || void 0 === r || null === (a = r.ReactCurrentOwner) || void 0 === a ? void 0 : a.current;
-                    if (e) {
-                        let n = po.get(e);
-                        null == n ? po.set(e, {
-                            id: t.current,
-                            state: e.memoizedState
-                        }) : e.memoizedState !== n.state && (t.current = n.id, po.delete(e))
-                    }
-                    n.current = ++t.current
-                }
-                return n.current
-            }(!!e);
-            return e || `react-aria${t.prefix}-${n}`
+                    let t = (0, i.useContext)(bo),
+                        n = (0, i.useRef)(null);
+                    if (null === n.current && !e) {
+                        var r, a;
+                        let e = null === (a = i.__SECRET_INTERNALS_DO_NOT_USE_OR_YOU_WILL_BE_FIRED) || void 0 === a || null === (r = a.ReactCurrentOwner) || void 0 === r ? void 0 : r.current;
+                        if (e) {
+                            let n = vo.get(e);
+                            null == n ? vo.set(e, {
+                                id: t.current,
+                                state: e.memoizedState
+                            }) : e.memoizedState !== n.state && (t.current = n.id, vo.delete(e))
+                        }
+                        n.current = ++t.current
+                    }
+                    return n.current
+                }(!!e),
+                r = `react-aria${t.prefix}`;
+            return e || `${r}-${n}`
+        };
+
+        function xo() {
+            return !1
+        }
+
+        function Oo() {
+            return !0
+        }
+
+        function wo(e) {
+            return () => {}
         }
-        const mo = e => {
+        const No = e => {
                 var t;
                 return "menu" === (null == (t = e.getAttribute("role")) ? void 0 : t.toLowerCase())
             },
-            go = () => {};
+            Eo = () => {};
 
-        function bo() {
-            const e = fo(),
+        function jo() {
+            const e = _o(),
                 {
                     show: t = !1,
-                    toggle: n = go,
+                    toggle: n = Eo,
                     setToggle: r,
                     menuElement: a
-                } = (0, i.useContext)(Na) || {},
+                } = (0, i.useContext)(Ra) || {},
                 s = (0, i.useCallback)((e => {
                     n(!t, e)
                 }), [t, n]),
                 o = {
                     id: e,
-                    ref: r || go,
+                    ref: r || Eo,
                     onClick: s,
                     "aria-expanded": !!t
                 };
-            return a && mo(a) && (o["aria-haspopup"] = !0), [o, {
+            return a && No(a) && (o["aria-haspopup"] = !0), [o, {
                 show: t,
                 toggle: n
             }]
         }
 
-        function yo({
+        function ko({
             children: e
         }) {
-            const [t, n] = bo();
+            const [t, n] = jo();
             return (0, _.jsx)(_.Fragment, {
                 children: e(t, n)
             })
         }
-        yo.displayName = "DropdownToggle";
-        const ho = yo,
-            vo = (e, t = null) => null != e ? String(e) : t || null,
-            _o = i.createContext(null),
-            xo = i.createContext(null);
-        xo.displayName = "NavContext";
-        const Oo = xo,
-            wo = "data-rr-ui-";
+        ko.displayName = "DropdownToggle";
+        const Po = ko,
+            Co = (e, t = null) => null != e ? String(e) : t || null,
+            To = i.createContext(null),
+            So = i.createContext(null);
+        So.displayName = "NavContext";
+        const Ro = So,
+            Do = "data-rr-ui-";
 
-        function No(e) {
-            return `${wo}${e}`
+        function Lo(e) {
+            return `${Do}${e}`
         }
-        const Eo = ["eventKey", "disabled", "onClick", "active", "as"];
+        const $o = ["eventKey", "disabled", "onClick", "active", "as"];
 
-        function jo({
+        function Io({
             key: e,
             href: t,
             active: n,
             disabled: r,
             onClick: a
         }) {
-            const s = (0, i.useContext)(_o),
-                o = (0, i.useContext)(Oo),
+            const s = (0, i.useContext)(To),
+                o = (0, i.useContext)(Ro),
                 {
                     activeKey: l
                 } = o || {},
-                c = vo(e, t),
-                u = null == n && null != e ? vo(l) === c : n;
+                c = Co(e, t),
+                u = null == n && null != e ? Co(l) === c : n;
             return [{
-                onClick: Xe((e => {
+                onClick: Ye((e => {
                     r || (null == a || a(e), s && !e.isPropagationStopped() && s(c, e))
                 })),
                 "aria-disabled": r || void 0,
                 "aria-selected": u,
-                [No("dropdown-item")]: ""
+                [Lo("dropdown-item")]: ""
             }, {
                 isActive: u
             }]
         }
-        const ko = i.forwardRef(((e, t) => {
+        const Ao = i.forwardRef(((e, t) => {
             let {
                 eventKey: n,
                 disabled: r,
                 onClick: a,
                 active: s,
-                as: o = st
+                as: o = lt
             } = e, i = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, Eo);
-            const [l] = jo({
+            }(e, $o);
+            const [l] = Io({
                 key: n,
                 href: i.href,
                 disabled: r,
                 onClick: a,
                 active: s
             });
             return (0, _.jsx)(o, Object.assign({}, i, {
                 ref: t
             }, l))
         }));
-        ko.displayName = "DropdownItem";
-        const Po = ko,
-            Co = (0, i.createContext)(G ? window : void 0);
+        Ao.displayName = "DropdownItem";
+        const Fo = Ao,
+            Mo = (0, i.createContext)(V ? window : void 0);
 
-        function To() {
-            return (0, i.useContext)(Co)
+        function Bo() {
+            return (0, i.useContext)(Mo)
         }
 
-        function So() {
-            const e = wa(),
+        function zo() {
+            const e = Sa(),
                 t = (0, i.useRef)(null),
                 n = (0, i.useCallback)((n => {
                     t.current = n, e()
                 }), [e]);
             return [t, n]
         }
 
-        function Ro({
+        function Ko({
             defaultShow: e,
             show: t,
             onSelect: n,
             onToggle: r,
-            itemSelector: a = `* [${No("dropdown-item")}]`,
+            itemSelector: a = `* [${Lo("dropdown-item")}]`,
             focusFirstItemOnShow: s,
             placement: o = "bottom-start",
             children: l
         }) {
-            const c = To(),
-                [u, d] = Oa(t, e, r),
-                [p, f] = So(),
+            const c = Bo(),
+                [u, d] = Ta(t, e, r),
+                [p, f] = zo(),
                 m = p.current,
-                [g, b] = So(),
+                [g, b] = zo(),
                 y = g.current,
-                h = Ze(u),
+                h = nt(u),
                 v = (0, i.useRef)(null),
                 x = (0, i.useRef)(!1),
-                O = (0, i.useContext)(_o),
+                O = (0, i.useContext)(To),
                 w = (0, i.useCallback)(((e, t, n = (null == t ? void 0 : t.type)) => {
                     d(e, {
                         originalEvent: t,
                         source: n
                     })
                 }), [d]),
-                N = Xe(((e, t) => {
+                N = Ye(((e, t) => {
                     null == n || n(e, t), w(!1, t, "select"), t.isPropagationStopped() || null == O || O(e, t)
                 })),
                 E = (0, i.useMemo)((() => ({
                     toggle: w,
                     placement: o,
                     show: u,
                     menuElement: m,
                     toggleElement: y,
                     setMenu: f,
                     setToggle: b
                 })), [w, o, u, m, y, f, b]);
             m && h && !u && (x.current = m.contains(m.ownerDocument.activeElement));
-            const j = Xe((() => {
+            const j = Ye((() => {
                     y && y.focus && y.focus()
                 })),
-                k = Xe((() => {
+                k = Ye((() => {
                     const e = v.current;
                     let t = s;
-                    if (null == t && (t = !(!p.current || !mo(p.current)) && "keyboard"), !1 === t || "keyboard" === t && !/^key.+$/.test(e)) return;
-                    const n = xa(p.current, a)[0];
+                    if (null == t && (t = !(!p.current || !No(p.current)) && "keyboard"), !1 === t || "keyboard" === t && !/^key.+$/.test(e)) return;
+                    const n = Ca(p.current, a)[0];
                     n && n.focus && n.focus()
                 }));
             (0, i.useEffect)((() => {
                 u ? k() : x.current && (x.current = !1, j())
             }), [u, x, j, k]), (0, i.useEffect)((() => {
                 v.current = null
             }));
             const P = (e, t) => {
                 if (!p.current) return null;
-                const n = xa(p.current, a);
+                const n = Ca(p.current, a);
                 let r = n.indexOf(e) + t;
                 return r = Math.max(0, Math.min(r, n.length)), n[r]
             };
-            return function(e, t, n, r) {
-                void 0 === r && (r = !1);
-                var a = Xe((e => {
-                    var t, n;
-                    const {
-                        key: r
-                    } = e, a = e.target, s = null == (t = p.current) ? void 0 : t.contains(a), o = null == (n = g.current) ? void 0 : n.contains(a);
-                    if (/input|textarea/i.test(a.tagName) && (" " === r || "Escape" !== r && s || "Escape" === r && "search" === a.type)) return;
-                    if (!s && !o) return;
-                    if (!("Tab" !== r || p.current && u)) return;
-                    v.current = e.type;
-                    const i = {
-                        originalEvent: e,
-                        source: e.type
-                    };
-                    switch (r) {
-                        case "ArrowUp": {
-                            const t = P(a, -1);
-                            return t && t.focus && t.focus(), void e.preventDefault()
-                        }
-                        case "ArrowDown":
-                            if (e.preventDefault(), u) {
-                                const e = P(a, 1);
-                                e && e.focus && e.focus()
-                            } else d(!0, i);
-                            return;
-                        case "Tab":
-                            Q(a.ownerDocument, "keyup", (e => {
-                                var t;
-                                ("Tab" !== e.key || e.target) && null != (t = p.current) && t.contains(e.target) || d(!1, i)
-                            }), {
-                                once: !0
-                            });
-                            break;
-                        case "Escape":
-                            "Escape" === r && (e.preventDefault(), e.stopPropagation()), d(!1, i)
-                    }
-                }));
-                (0, i.useEffect)((function() {
-                    var n = "function" == typeof e ? e() : e;
-                    return n.addEventListener(t, a, r),
-                        function() {
-                            return n.removeEventListener(t, a, r)
-                        }
+            return function(e, t, n, r = !1) {
+                const a = Ye(n);
+                (0, i.useEffect)((() => {
+                    const n = "function" == typeof e ? e() : e;
+                    return n.addEventListener(t, a, r), () => n.removeEventListener(t, a, r)
                 }), [e])
-            }((0, i.useCallback)((() => c.document), [c]), "keydown"), (0, _.jsx)(_o.Provider, {
+            }((0, i.useCallback)((() => c.document), [c]), "keydown", (e => {
+                var t, n;
+                const {
+                    key: r
+                } = e, a = e.target, s = null == (t = p.current) ? void 0 : t.contains(a), o = null == (n = g.current) ? void 0 : n.contains(a);
+                if (/input|textarea/i.test(a.tagName) && (" " === r || "Escape" !== r && s || "Escape" === r && "search" === a.type)) return;
+                if (!s && !o) return;
+                if (!("Tab" !== r || p.current && u)) return;
+                v.current = e.type;
+                const i = {
+                    originalEvent: e,
+                    source: e.type
+                };
+                switch (r) {
+                    case "ArrowUp": {
+                        const t = P(a, -1);
+                        return t && t.focus && t.focus(), void e.preventDefault()
+                    }
+                    case "ArrowDown":
+                        if (e.preventDefault(), u) {
+                            const e = P(a, 1);
+                            e && e.focus && e.focus()
+                        } else d(!0, i);
+                        return;
+                    case "Tab":
+                        J(a.ownerDocument, "keyup", (e => {
+                            var t;
+                            ("Tab" !== e.key || e.target) && null != (t = p.current) && t.contains(e.target) || d(!1, i)
+                        }), {
+                            once: !0
+                        });
+                        break;
+                    case "Escape":
+                        "Escape" === r && (e.preventDefault(), e.stopPropagation()), d(!1, i)
+                }
+            })), (0, _.jsx)(To.Provider, {
                 value: N,
-                children: (0, _.jsx)(Na.Provider, {
+                children: (0, _.jsx)(Ra.Provider, {
                     value: E,
                     children: l
                 })
             })
         }
-        Co.Provider, Ro.displayName = "Dropdown", Ro.Menu = io, Ro.Toggle = ho, Ro.Item = Po;
-        const Do = Ro,
-            Lo = i.createContext({});
-        Lo.displayName = "DropdownContext";
-        const $o = Lo,
-            Io = i.forwardRef((({
+        Mo.Provider, Ko.displayName = "Dropdown", Ko.Menu = mo, Ko.Toggle = Po, Ko.Item = Fo;
+        const Ho = Ko,
+            Uo = i.createContext({});
+        Uo.displayName = "DropdownContext";
+        const Wo = Uo,
+            qo = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "hr",
+                role: r = "separator",
+                ...a
+            }, s) => (t = E(t, "dropdown-divider"), (0, _.jsx)(n, {
+                ref: s,
+                className: b()(e, t),
+                role: r,
+                ...a
+            }))));
+        qo.displayName = "DropdownDivider";
+        const Vo = qo,
+            Go = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                role: r = "heading",
+                ...a
+            }, s) => (t = E(t, "dropdown-header"), (0, _.jsx)(n, {
+                ref: s,
+                className: b()(e, t),
+                role: r,
+                ...a
+            }))));
+        Go.displayName = "DropdownHeader";
+        const Yo = Go,
+            Xo = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 eventKey: n,
                 disabled: r = !1,
                 onClick: a,
                 active: s,
-                as: o = lt,
+                as: o = dt,
                 ...i
             }, l) => {
-                const c = j(e, "dropdown-item"),
-                    [u, d] = jo({
+                const c = E(e, "dropdown-item"),
+                    [u, d] = Io({
                         key: n,
                         href: i.href,
                         disabled: r,
                         onClick: a,
                         active: s
                     });
                 return (0, _.jsx)(o, {
                     ...i,
                     ...u,
                     ref: l,
                     className: b()(t, c, d.isActive && "active", r && "disabled")
                 })
             }));
-        Io.displayName = "DropdownItem";
-        const Ao = Io,
-            Mo = i.createContext(null);
-        Mo.displayName = "InputGroupContext";
-        const Fo = Mo,
-            Bo = i.createContext(null);
-        Bo.displayName = "NavbarContext";
-        const zo = Bo;
+        Xo.displayName = "DropdownItem";
+        const Jo = Xo,
+            Qo = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "span",
+                ...r
+            }, a) => (t = E(t, "dropdown-item-text"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Qo.displayName = "DropdownItemText";
+        const Zo = Qo,
+            ei = i.createContext(null);
+        ei.displayName = "InputGroupContext";
+        const ti = ei,
+            ni = i.createContext(null);
+        ni.displayName = "NavbarContext";
+        const ri = ni;
 
-        function Ko(e, t) {
+        function ai(e, t) {
             return e
         }
 
-        function Ho(e, t, n) {
+        function si(e, t, n) {
             let r = e ? n ? "bottom-start" : "bottom-end" : n ? "bottom-end" : "bottom-start";
             return "up" === t ? r = e ? n ? "top-start" : "top-end" : n ? "top-end" : "top-start" : "end" === t ? r = e ? n ? "left-end" : "right-end" : n ? "left-start" : "right-start" : "start" === t ? r = e ? n ? "right-end" : "left-end" : n ? "right-start" : "left-start" : "down-centered" === t ? r = "bottom" : "up-centered" === t && (r = "top"), r
         }
-        const Wo = i.forwardRef((({
+        const oi = i.forwardRef((({
             bsPrefix: e,
             className: t,
             align: n,
             rootCloseEvent: r,
-            flip: a,
+            flip: a = !0,
             show: s,
             renderOnMount: o,
             as: l = "div",
             popperConfig: c,
             variant: u,
             ...d
         }, p) => {
             let f = !1;
-            const m = (0, i.useContext)(zo),
-                g = j(e, "dropdown-menu"),
+            const m = (0, i.useContext)(ri),
+                g = E(e, "dropdown-menu"),
                 {
                     align: y,
                     drop: h,
                     isRTL: v
-                } = (0, i.useContext)($o);
+                } = (0, i.useContext)(Wo);
             n = n || y;
-            const x = (0, i.useContext)(Fo),
+            const x = (0, i.useContext)(ti),
                 O = [];
             if (n)
                 if ("object" == typeof n) {
                     const e = Object.keys(n);
                     if (e.length) {
                         const t = e[0],
                             r = n[t];
                         f = "start" === r, O.push(`${g}-${t}-${r}`)
                     }
                 } else "end" === n && (f = !0);
-            const w = Ho(f, h, v),
+            const w = si(f, h, v),
                 [N, {
-                    hasShown: E,
+                    hasShown: j,
                     popper: k,
                     show: P,
                     toggle: C
-                }] = so({
+                }] = po({
                     flip: a,
                     rootCloseEvent: r,
                     show: s,
                     usePopper: !m && 0 === O.length,
                     offset: [0, 2],
                     popperConfig: c,
                     placement: w
                 });
-            if (N.ref = ie(Ko(p), N.ref), tt((() => {
+            if (N.ref = oe(ai(p), N.ref), at((() => {
                     P && (null == k || k.update())
-                }), [P]), !E && !o && !x) return null;
+                }), [P]), !j && !o && !x) return null;
             "string" != typeof l && (N.show = P, N.close = () => null == C ? void 0 : C(!1), N.align = n);
             let T = d.style;
             return null != k && k.placement && (T = {
                 ...d.style,
                 ...N.style
             }, d["x-placement"] = k.placement), (0, _.jsx)(l, {
                 ...d,
@@ -6009,221 +6147,200 @@
                 style: T,
                 ...(O.length || m) && {
                     "data-bs-popper": "static"
                 },
                 className: b()(t, g, P && "show", f && `${g}-end`, u && `${g}-${u}`, ...O)
             })
         }));
-        Wo.displayName = "DropdownMenu", Wo.defaultProps = {
-            flip: !0
-        };
-        const Uo = Wo,
-            qo = i.forwardRef((({
+        oi.displayName = "DropdownMenu";
+        const ii = oi,
+            li = i.forwardRef((({
                 bsPrefix: e,
                 split: t,
                 className: n,
                 childBsPrefix: r,
                 as: a = nn,
                 ...s
             }, o) => {
-                const l = j(e, "dropdown-toggle"),
-                    c = (0, i.useContext)(Na);
+                const l = E(e, "dropdown-toggle"),
+                    c = (0, i.useContext)(Ra);
                 void 0 !== r && (s.bsPrefix = r);
-                const [u] = bo();
-                return u.ref = ie(u.ref, Ko(o)), (0, _.jsx)(a, {
+                const [u] = jo();
+                return u.ref = oe(u.ref, ai(o)), (0, _.jsx)(a, {
                     className: b()(n, l, t && `${l}-split`, (null == c ? void 0 : c.show) && "show"),
                     ...u,
                     ...s
                 })
             }));
-        qo.displayName = "DropdownToggle";
-        const Vo = qo,
-            Go = ht("dropdown-header", {
-                defaultProps: {
-                    role: "heading"
-                }
-            }),
-            Yo = ht("dropdown-divider", {
-                Component: "hr",
-                defaultProps: {
-                    role: "separator"
-                }
-            }),
-            Xo = ht("dropdown-item-text", {
-                Component: "span"
-            }),
-            Jo = i.forwardRef(((e, t) => {
+        li.displayName = "DropdownToggle";
+        const ci = li,
+            ui = i.forwardRef(((e, t) => {
                 const {
                     bsPrefix: n,
-                    drop: r,
+                    drop: r = "down",
                     show: a,
                     className: s,
-                    align: o,
+                    align: o = "start",
                     onSelect: l,
                     onToggle: c,
                     focusFirstItemOnShow: u,
                     as: d = "div",
                     navbar: p,
-                    autoClose: f,
+                    autoClose: f = !0,
                     ...m
                 } = v(e, {
                     show: "onToggle"
-                }), g = (0, i.useContext)(Fo), y = j(n, "dropdown"), h = C(), x = Xe(((e, t) => {
-                    var n;
-                    t.originalEvent.currentTarget !== document || "keydown" === t.source && "Escape" !== t.originalEvent.key || (t.source = "rootClose"), n = t.source, (!1 === f ? "click" === n : "inside" === f ? "rootClose" !== n : "outside" !== f || "select" !== n) && (null == c || c(e, t))
-                })), O = Ho("end" === o, r, h), w = (0, i.useMemo)((() => ({
+                }), g = (0, i.useContext)(ti), y = E(n, "dropdown"), h = P(), x = Ye(((e, t) => {
+                    var n, r, a;
+                    (null == (n = t.originalEvent) || null == (r = n.target) ? void 0 : r.classList.contains("dropdown-toggle")) && "mousedown" === t.source || (t.originalEvent.currentTarget !== document || "keydown" === t.source && "Escape" !== t.originalEvent.key || (t.source = "rootClose"), a = t.source, (!1 === f ? "click" === a : "inside" === f ? "rootClose" !== a : "outside" !== f || "select" !== a) && (null == c || c(e, t)))
+                })), O = si("end" === o, r, h), w = (0, i.useMemo)((() => ({
                     align: o,
                     drop: r,
                     isRTL: h
                 })), [o, r, h]), N = {
                     down: y,
                     "down-centered": `${y}-center`,
                     up: "dropup",
                     "up-centered": "dropup-center dropup",
                     end: "dropend",
                     start: "dropstart"
                 };
-                return (0, _.jsx)($o.Provider, {
+                return (0, _.jsx)(Wo.Provider, {
                     value: w,
-                    children: (0, _.jsx)(Do, {
+                    children: (0, _.jsx)(Ho, {
                         placement: O,
                         show: a,
                         onSelect: l,
                         onToggle: x,
                         focusFirstItemOnShow: u,
                         itemSelector: `.${y}-item:not(.disabled):not(:disabled)`,
                         children: g ? m.children : (0, _.jsx)(d, {
                             ...m,
                             ref: t,
                             className: b()(s, a && "show", N[r])
                         })
                     })
                 })
             }));
-        Jo.displayName = "Dropdown", Jo.defaultProps = {
-            navbar: !1,
-            align: "start",
-            autoClose: !0,
-            drop: "down"
-        };
-        const Qo = Object.assign(Jo, {
-            Toggle: Vo,
-            Menu: Uo,
-            Item: Ao,
-            ItemText: Xo,
-            Divider: Yo,
-            Header: Go
+        ui.displayName = "Dropdown";
+        const di = Object.assign(ui, {
+            Toggle: ci,
+            Menu: ii,
+            Item: Jo,
+            ItemText: Zo,
+            Divider: Vo,
+            Header: Yo
         });
-        n(7);
-        const Zo = i.createContext(null),
-            ei = ["as", "active", "eventKey"];
+        n(6);
+        const pi = i.createContext(null),
+            fi = ["as", "active", "eventKey"];
 
-        function ti({
+        function mi({
             key: e,
             onClick: t,
             active: n,
             id: r,
             role: a,
             disabled: s
         }) {
-            const o = (0, i.useContext)(_o),
-                l = (0, i.useContext)(Oo),
-                c = (0, i.useContext)(Zo);
+            const o = (0, i.useContext)(To),
+                l = (0, i.useContext)(Ro),
+                c = (0, i.useContext)(pi);
             let u = n;
             const d = {
                 role: a
             };
             if (l) {
                 a || "tablist" !== l.role || (d.role = "tab");
                 const t = l.getControllerId(null != e ? e : null),
                     s = l.getControlledId(null != e ? e : null);
-                d[No("event-key")] = e, d.id = t || r, u = null == n && null != e ? l.activeKey === e : n, !u && (null != c && c.unmountOnExit || null != c && c.mountOnEnter) || (d["aria-controls"] = s)
+                d[Lo("event-key")] = e, d.id = t || r, u = null == n && null != e ? l.activeKey === e : n, !u && (null != c && c.unmountOnExit || null != c && c.mountOnEnter) || (d["aria-controls"] = s)
             }
-            return "tab" === d.role && (d["aria-selected"] = u, u || (d.tabIndex = -1), s && (d.tabIndex = -1, d["aria-disabled"] = !0)), d.onClick = Xe((n => {
+            return "tab" === d.role && (d["aria-selected"] = u, u || (d.tabIndex = -1), s && (d.tabIndex = -1, d["aria-disabled"] = !0)), d.onClick = Ye((n => {
                 s || (null == t || t(n), null != e && o && !n.isPropagationStopped() && o(e, n))
             })), [d, {
                 isActive: u
             }]
         }
-        const ni = i.forwardRef(((e, t) => {
+        const gi = i.forwardRef(((e, t) => {
             let {
-                as: n = st,
+                as: n = lt,
                 active: r,
                 eventKey: a
             } = e, s = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, ei);
-            const [o, i] = ti(Object.assign({
-                key: vo(a, s.href),
+            }(e, fi);
+            const [o, i] = mi(Object.assign({
+                key: Co(a, s.href),
                 active: r
             }, s));
-            return o[No("active")] = i.isActive, (0, _.jsx)(n, Object.assign({}, s, o, {
+            return o[Lo("active")] = i.isActive, (0, _.jsx)(n, Object.assign({}, s, o, {
                 ref: t
             }))
         }));
-        ni.displayName = "NavItem";
-        const ri = ni,
-            ai = ["as", "onSelect", "activeKey", "role", "onKeyDown"],
-            si = () => {},
-            oi = No("event-key"),
-            ii = i.forwardRef(((e, t) => {
+        gi.displayName = "NavItem";
+        const bi = gi,
+            yi = ["as", "onSelect", "activeKey", "role", "onKeyDown"],
+            hi = () => {},
+            vi = Lo("event-key"),
+            _i = i.forwardRef(((e, t) => {
                 let {
                     as: n = "div",
                     onSelect: r,
                     activeKey: a,
                     role: s,
                     onKeyDown: o
                 } = e, l = function(e, t) {
                     if (null == e) return {};
                     var n, r, a = {},
                         s = Object.keys(e);
                     for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                     return a
-                }(e, ai);
-                const c = wa(),
+                }(e, yi);
+                const c = Sa(),
                     u = (0, i.useRef)(!1),
-                    d = (0, i.useContext)(_o),
-                    p = (0, i.useContext)(Zo);
+                    d = (0, i.useContext)(To),
+                    p = (0, i.useContext)(pi);
                 let f, m;
                 p && (s = s || "tablist", a = p.activeKey, f = p.getControlledId, m = p.getControllerId);
                 const g = (0, i.useRef)(null),
                     b = e => {
                         const t = g.current;
                         if (!t) return null;
-                        const n = xa(t, `[${oi}]:not([aria-disabled=true])`),
+                        const n = Ca(t, `[${vi}]:not([aria-disabled=true])`),
                             r = t.querySelector("[aria-selected=true]");
                         if (!r || r !== document.activeElement) return null;
                         const a = n.indexOf(r);
                         if (-1 === a) return null;
                         let s = a + e;
                         return s >= n.length && (s = 0), s < 0 && (s = n.length - 1), n[s]
                     },
                     y = (e, t) => {
                         null != e && (null == r || r(e, t), null == d || d(e, t))
                     };
                 (0, i.useEffect)((() => {
                     if (g.current && u.current) {
-                        const e = g.current.querySelector(`[${oi}][aria-selected=true]`);
+                        const e = g.current.querySelector(`[${vi}][aria-selected=true]`);
                         null == e || e.focus()
                     }
                     u.current = !1
                 }));
-                const h = ie(t, g);
-                return (0, _.jsx)(_o.Provider, {
+                const h = oe(t, g);
+                return (0, _.jsx)(To.Provider, {
                     value: y,
-                    children: (0, _.jsx)(Oo.Provider, {
+                    children: (0, _.jsx)(Ro.Provider, {
                         value: {
                             role: s,
-                            activeKey: vo(a),
-                            getControlledId: f || si,
-                            getControllerId: m || si
+                            activeKey: Co(a),
+                            getControlledId: f || hi,
+                            getControllerId: m || hi
                         },
                         children: (0, _.jsx)(n, Object.assign({}, l, {
                             onKeyDown: e => {
                                 if (null == o || o(e), !p) return;
                                 let t;
                                 switch (e.key) {
                                     case "ArrowLeft":
@@ -6241,65 +6358,77 @@
                             },
                             ref: h,
                             role: s
                         }))
                     })
                 })
             }));
-        ii.displayName = "Nav";
-        const li = Object.assign(ii, {
-                Item: ri
+        _i.displayName = "Nav";
+        const xi = Object.assign(_i, {
+                Item: bi
             }),
-            ci = ht("nav-item"),
-            ui = i.forwardRef((({
+            Oi = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "nav-item"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Oi.displayName = "NavItem";
+        const wi = Oi,
+            Ni = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                as: n = lt,
+                as: n = dt,
                 active: r,
                 eventKey: a,
-                ...s
-            }, o) => {
-                e = j(e, "nav-link");
-                const [i, l] = ti({
-                    key: vo(a, s.href),
+                disabled: s = !1,
+                ...o
+            }, i) => {
+                e = E(e, "nav-link");
+                const [l, c] = mi({
+                    key: Co(a, o.href),
                     active: r,
-                    ...s
+                    disabled: s,
+                    ...o
                 });
                 return (0, _.jsx)(n, {
-                    ...s,
-                    ...i,
-                    ref: o,
-                    className: b()(t, e, s.disabled && "disabled", l.isActive && "active")
+                    ...o,
+                    ...l,
+                    ref: i,
+                    disabled: s,
+                    className: b()(t, e, s && "disabled", c.isActive && "active")
                 })
             }));
-        ui.displayName = "NavLink", ui.defaultProps = {
-            disabled: !1
-        };
-        const di = ui,
-            pi = i.forwardRef(((e, t) => {
+        Ni.displayName = "NavLink";
+        const Ei = Ni,
+            ji = i.forwardRef(((e, t) => {
                 const {
                     as: n = "div",
                     bsPrefix: r,
                     variant: a,
-                    fill: s,
-                    justify: o,
+                    fill: s = !1,
+                    justify: o = !1,
                     navbar: l,
                     navbarScroll: c,
                     className: u,
                     activeKey: d,
                     ...p
                 } = v(e, {
                     activeKey: "onSelect"
-                }), f = j(r, "nav");
+                }), f = E(r, "nav");
                 let m, g, y = !1;
-                const h = (0, i.useContext)(zo),
-                    x = (0, i.useContext)(gn);
+                const h = (0, i.useContext)(ri),
+                    x = (0, i.useContext)(yn);
                 return h ? (m = h.bsPrefix, y = null == l || l) : x && ({
                     cardHeaderBsPrefix: g
-                } = x), (0, _.jsx)(li, {
+                } = x), (0, _.jsx)(xi, {
                     as: n,
                     ref: t,
                     activeKey: d,
                     className: b()(u, {
                         [f]: !y,
                         [`${m}-nav`]: y,
                         [`${m}-nav-scroll`]: y && c,
@@ -6307,67 +6436,64 @@
                         [`${f}-${a}`]: !!a,
                         [`${f}-fill`]: s,
                         [`${f}-justified`]: o
                     }),
                     ...p
                 })
             }));
-        pi.displayName = "Nav", pi.defaultProps = {
-            justify: !1,
-            fill: !1
-        };
-        const fi = Object.assign(pi, {
-            Item: ci,
-            Link: di
+        ji.displayName = "Nav";
+        const ki = Object.assign(ji, {
+            Item: wi,
+            Link: Ei
         });
-        var mi = l().createContext({}),
-            gi = ["caret", "bsPrefix", "split", "className", "childBsPrefix", "as"];
-        const bi = l().forwardRef((function(t, n) {
+        var Pi = l().createContext({}),
+            Ci = ["caret", "bsPrefix", "split", "className", "childBsPrefix", "as"];
+        const Ti = l().forwardRef((function(t, n) {
             var r = t.caret,
                 a = t.bsPrefix,
                 s = t.split,
                 c = t.className,
                 u = t.childBsPrefix,
                 d = t.as,
                 p = void 0 === d ? nn : d,
-                f = o(t, gi),
-                m = j(a, "dropdown-toggle"),
-                g = (0, i.useContext)(Na),
-                y = (0, i.useContext)(Fo);
+                f = o(t, Ci),
+                m = E(a, "dropdown-toggle"),
+                g = (0, i.useContext)(Ra),
+                y = (0, i.useContext)(ti);
             void 0 !== u && (f.bsPrefix = u);
-            var h = Le(bo(), 1)[0];
-            return h.ref = ie(h.ref, Ko(n)), l().createElement(p, e({
+            var h = Se(jo(), 1)[0];
+            return h.ref = oe(h.ref, ai(n)), l().createElement(p, e({
                 className: b()(c, r && m, s && "".concat(m, "-split"), !!y && (null == g ? void 0 : g.show) && "show")
             }, h, f))
         }));
-        var yi = ["children", "nav", "label", "disabled", "caret", "in_navbar", "addon_type", "size", "right", "align_end", "menu_variant", "direction", "loading_state", "color", "group", "toggle_style", "toggleClassName", "toggle_class_name", "className", "class_name"];
+        var Si = ["children", "nav", "label", "disabled", "caret", "in_navbar", "addon_type", "size", "right", "align_end", "menu_variant", "direction", "loading_state", "color", "group", "toggle_style", "toggleClassName", "toggle_class_name", "className", "class_name"];
 
-        function hi(e, t) {
+        function Ri(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function vi(e) {
+        function Di(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? hi(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : hi(Object(n)).forEach((function(t) {
+                t % 2 ? Ri(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ri(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var _i = function(t) {
+        var Li = function(t) {
             var n = t.children,
                 r = t.nav,
                 a = t.label,
                 s = t.disabled,
                 c = t.caret,
                 u = t.in_navbar,
                 d = (t.addon_type, t.size),
@@ -6379,61 +6505,61 @@
                 h = t.color,
                 v = t.group,
                 _ = t.toggle_style,
                 x = t.toggleClassName,
                 O = t.toggle_class_name,
                 w = t.className,
                 N = t.class_name,
-                E = o(t, yi),
-                j = Le((0, i.useState)(!1), 2),
+                E = o(t, Si),
+                j = Se((0, i.useState)(!1), 2),
                 k = j[0],
                 P = j[1],
-                C = Et.has(h) || "link" === h,
+                C = Ot.has(h) || "link" === h,
                 T = function() {
                     s || P(!k)
                 };
-            return l().createElement(mi.Provider, {
+            return l().createElement(Pi.Provider, {
                 value: {
                     toggle: T,
                     isOpen: k
                 }
-            }, l().createElement(Qo, e({
-                as: r ? fi.Item : v ? ln : void 0,
+            }, l().createElement(di, e({
+                as: r ? ki.Item : v ? ln : void 0,
                 show: k,
                 disabled: s,
                 navbar: u,
                 className: N || w,
                 drop: "left" === b ? "start" : "right" === b ? "end" : b,
                 onToggle: function(e, t) {
                     t && "select" === t.source || P(e)
                 },
                 align: f || p ? "end" : "start"
             }, m(["setProps"], E), {
                 "data-dash-is-loading": y && y.is_loading || void 0
-            }), l().createElement(bi, {
+            }), l().createElement(Ti, {
                 caret: c,
-                as: r ? fi.Link : void 0,
+                as: r ? ki.Link : void 0,
                 onClick: T,
                 disabled: s,
                 size: d,
                 variant: C ? h : void 0,
-                style: C ? _ : vi({
+                style: C ? _ : Di({
                     backgroundColor: h
                 }, _),
                 className: O || x
-            }, a), l().createElement(Qo.Menu, {
+            }, a), l().createElement(di.Menu, {
                 renderOnMount: !0,
                 variant: "dark" === g ? "dark" : void 0
             }, n)))
         };
-        _i.defaultProps = {
+        Li.defaultProps = {
             caret: !0,
             disabled: !1,
             menu_variant: "light"
-        }, _i.propTypes = {
+        }, Li.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             label: u().node,
@@ -6454,50 +6580,51 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             group: u().bool
         };
-        const xi = _i;
-        var Oi = ["children", "href", "loading_state", "target", "disabled", "n_clicks", "toggle", "setProps", "className", "class_name", "header", "divider"],
-            wi = function(t) {
+        const $i = Li;
+        var Ii = ["children", "href", "loading_state", "target", "disabled", "n_clicks", "toggle", "setProps", "className", "class_name", "header", "divider"],
+            Ai = function(t) {
                 var n = t.children,
                     r = t.href,
                     a = t.loading_state,
                     s = t.target,
                     c = t.disabled,
                     u = t.n_clicks,
                     d = t.toggle,
                     p = t.setProps,
                     f = t.className,
                     g = t.class_name,
                     b = t.header,
                     y = t.divider,
-                    h = o(t, Oi),
-                    v = (0, i.useContext)(mi),
-                    _ = r && !c;
-                return h[_ ? "preOnClick" : "onClick"] = function(e) {
+                    h = o(t, Ii),
+                    v = Fe(r, p),
+                    _ = (0, i.useContext)(Pi),
+                    x = v && !c;
+                return h[x ? "preOnClick" : "onClick"] = function(e) {
                     return function(e) {
                         !c && p && p({
                             n_clicks: u + 1,
                             n_clicks_timestamp: Date.now()
-                        }), d && v.isOpen && v.toggle(e)
+                        }), d && _.isOpen && _.toggle(e)
                     }(e)
-                }, b ? l().createElement(Qo.Header, null, n) : y ? l().createElement(Qo.Divider, null) : l().createElement(Qo.Item, e({
-                    as: _ ? Kt : "button",
-                    href: _ ? r : void 0,
+                }, b ? l().createElement(di.Header, null, n) : y ? l().createElement(di.Divider, null) : l().createElement(di.Item, e({
+                    as: x ? Bt : "button",
+                    href: x ? v : void 0,
                     disabled: c,
-                    target: _ ? s : void 0,
+                    target: x ? s : void 0,
                     className: g || f
                 }, m(["setProps"], h), {
                     "data-dash-is-loading": a && a.is_loading || void 0
                 }), n)
             };
-        wi.propTypes = {
+        Ai.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             active: u().bool,
@@ -6511,59 +6638,59 @@
             n_clicks_timestamp: u().number,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
-        }, wi.defaultProps = {
+        }, Ai.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1,
             toggle: !0
         };
-        const Ni = wi;
-        var Ei = ["children", "is_in", "loading_state", "style", "className", "class_name", "tag"];
+        const Fi = Ai;
+        var Mi = ["children", "is_in", "loading_state", "style", "className", "class_name", "tag"];
 
-        function ji(e, t) {
+        function Bi(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function ki(e) {
+        function zi(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? ji(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ji(Object(n)).forEach((function(t) {
+                t % 2 ? Bi(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Bi(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Pi = l().forwardRef((function(t, n) {
+        var Ki = l().forwardRef((function(t, n) {
             var r = t.children,
                 a = t.is_in,
                 s = t.loading_state,
                 c = t.style,
                 u = t.className,
                 d = t.class_name,
                 p = t.tag,
-                f = o(t, Ei),
-                g = Le((0, i.useState)(!a), 2),
+                f = o(t, Mi),
+                g = Se((0, i.useState)(!a), 2),
                 b = g[0],
                 y = g[1];
-            return l().createElement(dt, e({
+            return l().createElement(bt, e({
                 in: a,
-                style: b ? ki({
+                style: b ? zi({
                     visibility: "hidden"
                 }, c) : c,
                 onEnter: function() {
                     return y(!1)
                 },
                 onExited: function() {
                     return y(!0)
@@ -6572,15 +6699,15 @@
                 as: p
             }, m(["setProps"], f), {
                 "data-dash-is-loading": s && s.is_loading || void 0
             }), l().createElement("div", {
                 ref: n
             }, r))
         }));
-        Pi.propTypes = {
+        Ki.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             is_in: u().bool,
@@ -6594,76 +6721,76 @@
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ci = Pi,
-            Ti = {
+        const Hi = Ki,
+            Ui = {
                 type: u().string,
                 tooltip: u().bool,
                 as: u().elementType
             },
-            Si = i.forwardRef((({
+            Wi = i.forwardRef((({
                 as: e = "div",
                 className: t,
                 type: n = "valid",
                 tooltip: r = !1,
                 ...a
             }, s) => (0, _.jsx)(e, {
                 ...a,
                 ref: s,
                 className: b()(t, `${n}-${r?"tooltip":"feedback"}`)
             })));
-        Si.displayName = "Feedback", Si.propTypes = Ti;
-        const Ri = Si,
-            Di = i.createContext({}),
-            Li = i.forwardRef((({
+        Wi.displayName = "Feedback", Wi.propTypes = Ui;
+        const qi = Wi,
+            Vi = i.createContext({}),
+            Gi = i.forwardRef((({
                 id: e,
                 bsPrefix: t,
                 className: n,
                 type: r = "checkbox",
                 isValid: a = !1,
                 isInvalid: s = !1,
                 as: o = "input",
                 ...l
             }, c) => {
                 const {
                     controlId: u
-                } = (0, i.useContext)(Di);
-                return t = j(t, "form-check-input"), (0, _.jsx)(o, {
+                } = (0, i.useContext)(Vi);
+                return t = E(t, "form-check-input"), (0, _.jsx)(o, {
                     ...l,
                     ref: c,
                     type: r,
                     id: e || u,
                     className: b()(n, t, a && "is-valid", s && "is-invalid")
                 })
             }));
-        Li.displayName = "FormCheckInput";
-        const $i = Li,
-            Ii = i.forwardRef((({
+        Gi.displayName = "FormCheckInput";
+        const Yi = Gi,
+            Xi = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 htmlFor: n,
                 ...r
             }, a) => {
                 const {
                     controlId: s
-                } = (0, i.useContext)(Di);
-                return e = j(e, "form-check-label"), (0, _.jsx)("label", {
+                } = (0, i.useContext)(Vi);
+                return e = E(e, "form-check-label"), (0, _.jsx)("label", {
                     ...r,
                     ref: a,
                     htmlFor: n || s,
                     className: b()(t, e)
                 })
             }));
-        Ii.displayName = "FormCheckLabel";
-        const Ai = Ii,
-            Mi = i.forwardRef((({
+        Xi.displayName = "FormCheckLabel";
+        const Ji = Xi,
+            Qi = i.forwardRef((({
                 id: e,
                 bsPrefix: t,
                 bsSwitchPrefix: n,
                 inline: r = !1,
                 reverse: a = !1,
                 disabled: s = !1,
                 isValid: o = !1,
@@ -6676,54 +6803,54 @@
                 title: m = "",
                 type: g = "checkbox",
                 label: y,
                 children: h,
                 as: v = "input",
                 ...x
             }, O) => {
-                t = j(t, "form-check"), n = j(n, "form-switch");
+                t = E(t, "form-check"), n = E(n, "form-switch");
                 const {
                     controlId: w
-                } = (0, i.useContext)(Di), N = (0, i.useMemo)((() => ({
+                } = (0, i.useContext)(Vi), N = (0, i.useMemo)((() => ({
                     controlId: e || w
-                })), [w, e]), E = !h && null != y && !1 !== y || function(e, t) {
+                })), [w, e]), j = !h && null != y && !1 !== y || function(e, t) {
                     return i.Children.toArray(e).some((e => i.isValidElement(e) && e.type === t))
-                }(h, Ai), k = (0, _.jsx)($i, {
+                }(h, Ji), k = (0, _.jsx)(Yi, {
                     ...x,
                     type: "switch" === g ? "checkbox" : g,
                     ref: O,
                     isValid: o,
                     isInvalid: l,
                     disabled: s,
                     as: v
                 });
-                return (0, _.jsx)(Di.Provider, {
+                return (0, _.jsx)(Vi.Provider, {
                     value: N,
                     children: (0, _.jsx)("div", {
                         style: f,
-                        className: b()(p, E && t, r && `${t}-inline`, a && `${t}-reverse`, "switch" === g && n),
+                        className: b()(p, j && t, r && `${t}-inline`, a && `${t}-reverse`, "switch" === g && n),
                         children: h || (0, _.jsxs)(_.Fragment, {
-                            children: [k, E && (0, _.jsx)(Ai, {
+                            children: [k, j && (0, _.jsx)(Ji, {
                                 title: m,
                                 children: y
-                            }), u && (0, _.jsx)(Ri, {
+                            }), u && (0, _.jsx)(qi, {
                                 type: d,
                                 tooltip: c,
                                 children: u
                             })]
                         })
                     })
                 })
             }));
-        Mi.displayName = "FormCheck";
-        const Fi = Object.assign(Mi, {
-                Input: $i,
-                Label: Ai
+        Qi.displayName = "FormCheck";
+        const Zi = Object.assign(Qi, {
+                Input: Yi,
+                Label: Ji
             }),
-            Bi = i.forwardRef((({
+            el = i.forwardRef((({
                 bsPrefix: e,
                 type: t,
                 size: n,
                 htmlSize: r,
                 id: a,
                 className: s,
                 isValid: o = !1,
@@ -6731,227 +6858,229 @@
                 plaintext: c,
                 readOnly: u,
                 as: d = "input",
                 ...p
             }, f) => {
                 const {
                     controlId: m
-                } = (0, i.useContext)(Di);
-                let g;
-                return e = j(e, "form-control"), g = c ? {
-                    [`${e}-plaintext`]: !0
-                } : {
-                    [e]: !0,
-                    [`${e}-${n}`]: n
-                }, (0, _.jsx)(d, {
+                } = (0, i.useContext)(Vi);
+                return e = E(e, "form-control"), (0, _.jsx)(d, {
                     ...p,
                     type: t,
                     size: r,
                     ref: f,
                     readOnly: u,
                     id: a || m,
-                    className: b()(s, g, o && "is-valid", l && "is-invalid", "color" === t && `${e}-color`)
+                    className: b()(s, c ? `${e}-plaintext` : e, n && `${e}-${n}`, "color" === t && `${e}-color`, o && "is-valid", l && "is-invalid")
                 })
             }));
-        Bi.displayName = "FormControl";
-        const zi = Object.assign(Bi, {
-                Feedback: Ri
+        el.displayName = "FormControl";
+        const tl = Object.assign(el, {
+                Feedback: qi
             }),
-            Ki = ht("form-floating"),
-            Hi = i.forwardRef((({
+            nl = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "form-floating"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        nl.displayName = "FormFloating";
+        const rl = nl,
+            al = i.forwardRef((({
                 controlId: e,
                 as: t = "div",
                 ...n
             }, r) => {
                 const a = (0, i.useMemo)((() => ({
                     controlId: e
                 })), [e]);
-                return (0, _.jsx)(Di.Provider, {
+                return (0, _.jsx)(Vi.Provider, {
                     value: a,
                     children: (0, _.jsx)(t, {
                         ...n,
                         ref: r
                     })
                 })
             }));
-        Hi.displayName = "FormGroup";
-        const Wi = Hi,
-            Ui = i.forwardRef((({
+        al.displayName = "FormGroup";
+        const sl = al,
+            ol = i.forwardRef((({
                 as: e = "label",
                 bsPrefix: t,
-                column: n,
-                visuallyHidden: r,
+                column: n = !1,
+                visuallyHidden: r = !1,
                 className: a,
                 htmlFor: s,
                 ...o
             }, l) => {
                 const {
                     controlId: c
-                } = (0, i.useContext)(Di);
-                t = j(t, "form-label");
+                } = (0, i.useContext)(Vi);
+                t = E(t, "form-label");
                 let u = "col-form-label";
                 "string" == typeof n && (u = `${u} ${u}-${n}`);
                 const d = b()(a, t, r && "visually-hidden", n && u);
-                return s = s || c, n ? (0, _.jsx)(sa, {
+                return s = s || c, n ? (0, _.jsx)(fa, {
                     ref: l,
                     as: "label",
                     className: d,
                     htmlFor: s,
                     ...o
                 }) : (0, _.jsx)(e, {
                     ref: l,
                     className: d,
                     htmlFor: s,
                     ...o
                 })
             }));
-        Ui.displayName = "FormLabel", Ui.defaultProps = {
-            column: !1,
-            visuallyHidden: !1
-        };
-        const qi = Ui,
-            Vi = i.forwardRef((({
+        ol.displayName = "FormLabel";
+        const il = ol,
+            ll = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 id: n,
                 ...r
             }, a) => {
                 const {
                     controlId: s
-                } = (0, i.useContext)(Di);
-                return e = j(e, "form-range"), (0, _.jsx)("input", {
+                } = (0, i.useContext)(Vi);
+                return e = E(e, "form-range"), (0, _.jsx)("input", {
                     ...r,
                     type: "range",
                     ref: a,
                     className: b()(t, e),
                     id: n || s
                 })
             }));
-        Vi.displayName = "FormRange";
-        const Gi = Vi,
-            Yi = i.forwardRef((({
+        ll.displayName = "FormRange";
+        const cl = ll,
+            ul = i.forwardRef((({
                 bsPrefix: e,
                 size: t,
                 htmlSize: n,
                 className: r,
                 isValid: a = !1,
                 isInvalid: s = !1,
                 id: o,
                 ...l
             }, c) => {
                 const {
                     controlId: u
-                } = (0, i.useContext)(Di);
-                return e = j(e, "form-select"), (0, _.jsx)("select", {
+                } = (0, i.useContext)(Vi);
+                return e = E(e, "form-select"), (0, _.jsx)("select", {
                     ...l,
                     size: n,
                     ref: c,
                     className: b()(r, e, t && `${e}-${t}`, a && "is-valid", s && "is-invalid"),
                     id: o || u
                 })
             }));
-        Yi.displayName = "FormSelect";
-        const Xi = Yi,
-            Ji = i.forwardRef((({
+        ul.displayName = "FormSelect";
+        const dl = ul,
+            pl = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n = "small",
                 muted: r,
                 ...a
-            }, s) => (e = j(e, "form-text"), (0, _.jsx)(n, {
+            }, s) => (e = E(e, "form-text"), (0, _.jsx)(n, {
                 ...a,
                 ref: s,
                 className: b()(t, e, r && "text-muted")
             }))));
-        Ji.displayName = "FormText";
-        const Qi = Ji,
-            Zi = i.forwardRef(((e, t) => (0, _.jsx)(Fi, {
+        pl.displayName = "FormText";
+        const fl = pl,
+            ml = i.forwardRef(((e, t) => (0, _.jsx)(Zi, {
                 ...e,
                 ref: t,
                 type: "switch"
             })));
-        Zi.displayName = "Switch";
-        const el = Object.assign(Zi, {
-                Input: Fi.Input,
-                Label: Fi.Label
+        ml.displayName = "Switch";
+        const gl = Object.assign(ml, {
+                Input: Zi.Input,
+                Label: Zi.Label
             }),
-            tl = i.forwardRef((({
+            bl = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 children: n,
                 controlId: r,
                 label: a,
                 ...s
-            }, o) => (e = j(e, "form-floating"), (0, _.jsxs)(Wi, {
+            }, o) => (e = E(e, "form-floating"), (0, _.jsxs)(sl, {
                 ref: o,
                 className: b()(t, e),
                 controlId: r,
                 ...s,
                 children: [n, (0, _.jsx)("label", {
                     htmlFor: r,
                     children: a
                 })]
             }))));
-        tl.displayName = "FloatingLabel";
-        const nl = tl,
-            rl = {
+        bl.displayName = "FloatingLabel";
+        const yl = bl,
+            hl = {
                 _ref: u().any,
                 validated: u().bool,
                 as: u().elementType
             },
-            al = i.forwardRef((({
+            vl = i.forwardRef((({
                 className: e,
                 validated: t,
                 as: n = "form",
                 ...r
             }, a) => (0, _.jsx)(n, {
                 ...r,
                 ref: a,
                 className: b()(e, t && "was-validated")
             })));
-        al.displayName = "Form", al.propTypes = rl;
-        const sl = Object.assign(al, {
-            Group: Wi,
-            Control: zi,
-            Floating: Ki,
-            Check: Fi,
-            Switch: el,
-            Label: qi,
-            Text: Qi,
-            Range: Gi,
-            Select: Xi,
-            FloatingLabel: nl
+        vl.displayName = "Form", vl.propTypes = hl;
+        const _l = Object.assign(vl, {
+            Group: sl,
+            Control: tl,
+            Floating: rl,
+            Check: Zi,
+            Switch: gl,
+            Label: il,
+            Text: fl,
+            Range: cl,
+            Select: dl,
+            FloatingLabel: yl
         });
-        var ol = ["children", "loading_state", "n_submit", "prevent_default_on_submit", "setProps", "className", "class_name"],
-            il = function(t) {
+        var xl = ["children", "loading_state", "n_submit", "prevent_default_on_submit", "setProps", "className", "class_name"],
+            Ol = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.n_submit,
                     s = t.prevent_default_on_submit,
                     i = t.setProps,
                     c = t.className,
                     u = t.class_name,
-                    d = o(t, ol);
-                return l().createElement(sl, e({
+                    d = o(t, xl);
+                return l().createElement(_l, e({
                     onSubmit: function(e) {
                         s && e.preventDefault(), i && i({
                             n_submit: a + 1,
                             n_submit_timestamp: Date.now()
                         })
                     },
                     className: u || c
                 }, m(["n_submit_timestamp"], d), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        il.defaultProps = {
+        Ol.defaultProps = {
             prevent_default_on_submit: !0,
             n_submit: 0,
             n_submit_timestamp: -1
-        }, il.propTypes = {
+        }, Ol.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             action: u().string,
@@ -6961,168 +7090,168 @@
             prevent_default_on_submit: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const ll = il;
-        var cl = ["children", "loading_state", "className", "class_name"],
-            ul = function(t) {
+        const wl = Ol;
+        var Nl = ["children", "loading_state", "className", "class_name"],
+            El = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, cl);
-                return l().createElement(zi.Feedback, e({
+                    i = o(t, Nl);
+                return l().createElement(tl.Feedback, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        ul.propTypes = {
+        El.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             type: u().string,
             tooltip: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const dl = ul;
-        var pl = ["children", "html_for", "className", "class_name", "loading_state"],
-            fl = function(t) {
+        const jl = El;
+        var kl = ["children", "html_for", "className", "class_name", "loading_state"],
+            Pl = function(t) {
                 var n = t.children,
                     r = t.html_for,
                     a = t.className,
                     s = t.class_name,
                     i = t.loading_state,
-                    c = o(t, pl);
-                return l().createElement(Ki, e({
+                    c = o(t, kl);
+                return l().createElement(rl, e({
                     htmlFor: r,
                     className: s || a
                 }, m(["setProps"], c), {
                     "data-dash-is-loading": i && i.is_loading || void 0
                 }), n)
             };
-        fl.propTypes = {
+        Pl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             html_for: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const ml = fl;
-        var gl = ["children", "loading_state", "color", "style", "className", "class_name"];
+        const Cl = Pl;
+        var Tl = ["children", "loading_state", "color", "style", "className", "class_name"];
 
-        function bl(e, t) {
+        function Sl(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function yl(e) {
+        function Rl(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? bl(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : bl(Object(n)).forEach((function(t) {
+                t % 2 ? Sl(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Sl(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var hl = function(t) {
+        var Dl = function(t) {
             var n = t.children,
                 r = t.loading_state,
                 a = t.color,
                 s = t.style,
                 i = t.className,
                 c = t.class_name,
-                u = o(t, gl),
-                d = jt.has(a),
+                u = o(t, Tl),
+                d = wt.has(a),
                 p = b()(c || i, d && "text-".concat(a));
-            return l().createElement(Qi, e({
-                style: d ? s : yl({
+            return l().createElement(fl, e({
+                style: d ? s : Rl({
                     color: a
                 }, s),
                 className: p
             }, m(["setProps"], u), {
                 "data-dash-is-loading": r && r.is_loading || void 0
             }), n)
         };
-        hl.propTypes = {
+        Dl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             color: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const vl = hl,
-            _l = p((function(e) {
+        const Ll = Dl,
+            $l = p((function(e) {
                 return null == e
             }));
-        var xl = n(12),
-            Ol = n.n(xl),
-            wl = ["type", "value", "n_blur", "n_submit", "valid", "invalid", "plaintext", "size", "html_size", "setProps", "debounce", "loading_state", "className", "class_name", "autoComplete", "autocomplete", "autoFocus", "autofocus", "inputMode", "inputmode", "maxLength", "maxlength", "minLength", "minlength", "readonly", "tabIndex", "tabindex"];
+        var Il = n(11),
+            Al = n.n(Il),
+            Fl = ["type", "value", "n_blur", "n_submit", "valid", "invalid", "plaintext", "size", "html_size", "setProps", "debounce", "loading_state", "className", "class_name", "autoComplete", "autocomplete", "autoFocus", "autofocus", "inputMode", "inputmode", "maxLength", "maxlength", "minLength", "minlength", "readonly", "tabIndex", "tabindex"];
 
-        function Nl(e, t) {
+        function Ml(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function El(e) {
+        function Bl(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Nl(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Nl(Object(n)).forEach((function(t) {
+                t % 2 ? Ml(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ml(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var jl = function(e) {
-                return Ol()(e) ? +e : NaN
+        var zl = function(e) {
+                return Al()(e) ? +e : NaN
             },
-            kl = function(e, t) {
+            Kl = function(e, t) {
                 return e === t || isNaN(e) && isNaN(t)
             },
-            Pl = function(t) {
+            Hl = function(t) {
                 var n = t.type,
                     r = t.value,
                     a = t.n_blur,
                     s = t.n_submit,
                     c = t.valid,
                     u = t.invalid,
                     d = t.plaintext,
@@ -7142,63 +7271,63 @@
                     k = t.maxLength,
                     P = t.maxlength,
                     C = t.minLength,
                     T = t.minlength,
                     S = t.readonly,
                     R = t.tabIndex,
                     D = t.tabindex,
-                    L = o(t, wl),
+                    L = o(t, Fl),
                     $ = (0, i.useRef)(null),
                     I = d ? "form-control-plaintext" : "form-control",
                     A = b()(_ || v, u && "is-invalid", c && "is-valid", !!p && "form-control-".concat(p), I);
                 (0, i.useEffect)((function() {
                     if ("number" === n) {
                         var e = $.current.value,
-                            t = $.current.checkValidity() ? jl(e) : NaN,
-                            a = jl(r);
-                        kl(a, t) || ($.current.value = _l(a) ? a : r)
+                            t = $.current.checkValidity() ? zl(e) : NaN,
+                            a = zl(r);
+                        Kl(a, t) || ($.current.value = $l(a) ? a : r)
                     } else {
                         var s = $.current.value;
                         r !== s && ($.current.value = null != r ? r : "")
                     }
                 }), [r]);
-                var M = function() {
+                var F = function() {
                     var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     if ("number" === n) {
                         var t = $.current.value,
-                            a = $.current.checkValidity() ? jl(t) : NaN,
-                            s = jl(r);
-                        kl(s, a) ? Object.keys(e).length && g(e) : g(El(El({}, e), {}, {
+                            a = $.current.checkValidity() ? zl(t) : NaN,
+                            s = zl(r);
+                        Kl(s, a) ? Object.keys(e).length && g(e) : g(Bl(Bl({}, e), {}, {
                             value: a
                         }))
                     } else e.value = $.current.value, g(e)
                 };
                 return l().createElement("input", e({
                     ref: $,
                     type: n,
                     className: A,
                     onChange: function() {
-                        y || M()
+                        y || F()
                     },
                     onBlur: function() {
                         if (g) {
                             var e = {
                                 n_blur: a + 1,
                                 n_blur_timestamp: Date.now()
                             };
-                            y ? M(e) : g(e)
+                            y ? F(e) : g(e)
                         }
                     },
                     onKeyPress: function(e) {
                         if (g && "Enter" === e.key) {
                             var t = {
                                 n_submit: s + 1,
                                 n_submit_timestamp: Date.now()
                             };
-                            y ? M(t) : g(t)
+                            y ? F(t) : g(t)
                         }
                     }
                 }, m(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], L), {
                     valid: c ? "true" : void 0,
                     invalid: u ? "true" : void 0,
                     "data-dash-is-loading": h && h.is_loading || void 0,
                     autoComplete: O || x,
@@ -7207,15 +7336,15 @@
                     maxLength: P || k,
                     minLength: T || C,
                     readOnly: S,
                     tabIndex: D || R,
                     size: f
                 }))
             };
-        Pl.propTypes = {
+        Hl.propTypes = {
             id: u().string,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             type: u().oneOf(["text", "number", "password", "email", "range", "search", "tel", "url", "hidden"]),
             value: u().oneOfType([u().string, u().number]),
@@ -7255,149 +7384,158 @@
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             tabindex: u().string,
             tabIndex: u().string
-        }, Pl.defaultProps = {
+        }, Hl.defaultProps = {
             n_blur: 0,
             n_blur_timestamp: -1,
             n_submit: 0,
             n_submit_timestamp: -1,
             debounce: !1,
             persisted_props: ["value"],
             persistence_type: "local",
             step: "any"
         };
-        const Cl = Pl,
-            Tl = ht("input-group-text", {
-                Component: "span"
-            }),
-            Sl = i.forwardRef((({
+        const Ul = Hl,
+            Wl = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "span",
+                ...r
+            }, a) => (t = E(t, "input-group-text"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Wl.displayName = "InputGroupText";
+        const ql = Wl,
+            Vl = i.forwardRef((({
                 bsPrefix: e,
                 size: t,
                 hasValidation: n,
                 className: r,
                 as: a = "div",
                 ...s
             }, o) => {
-                e = j(e, "input-group");
+                e = E(e, "input-group");
                 const l = (0, i.useMemo)((() => ({})), []);
-                return (0, _.jsx)(Fo.Provider, {
+                return (0, _.jsx)(ti.Provider, {
                     value: l,
                     children: (0, _.jsx)(a, {
                         ref: o,
                         ...s,
                         className: b()(r, e, t && `${e}-${t}`, n && "has-validation")
                     })
                 })
             }));
-        Sl.displayName = "InputGroup";
-        const Rl = Object.assign(Sl, {
-            Text: Tl,
-            Radio: e => (0, _.jsx)(Tl, {
-                children: (0, _.jsx)($i, {
+        Vl.displayName = "InputGroup";
+        const Gl = Object.assign(Vl, {
+            Text: ql,
+            Radio: e => (0, _.jsx)(ql, {
+                children: (0, _.jsx)(Yi, {
                     type: "radio",
                     ...e
                 })
             }),
-            Checkbox: e => (0, _.jsx)(Tl, {
-                children: (0, _.jsx)($i, {
+            Checkbox: e => (0, _.jsx)(ql, {
+                children: (0, _.jsx)(Yi, {
                     type: "checkbox",
                     ...e
                 })
             })
         });
-        var Dl = ["children", "loading_state", "className", "class_name"],
-            Ll = function(t) {
+        var Yl = ["children", "loading_state", "className", "class_name"],
+            Xl = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Dl);
-                return l().createElement(Rl, e({
+                    i = o(t, Yl);
+                return l().createElement(Gl, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Ll.propTypes = {
+        Xl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             size: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const $l = Ll;
-        var Il = ["children", "loading_state", "className", "class_name"],
-            Al = function(t) {
+        const Jl = Xl;
+        var Ql = ["children", "loading_state", "className", "class_name"],
+            Zl = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Il);
-                return l().createElement(Rl.Text, e({
+                    i = o(t, Ql);
+                return l().createElement(Gl.Text, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Al.propTypes = {
+        Zl.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             key: u().string,
             class_name: u().string,
             className: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ml = Al;
-        var Fl = ["children", "html_for", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "size", "className", "class_name", "color", "style", "loading_state", "check"];
+        const ec = Zl;
+        var tc = ["children", "html_for", "width", "xs", "sm", "md", "lg", "xl", "xxl", "align", "size", "className", "class_name", "color", "style", "loading_state", "check"];
 
-        function Bl(e, t) {
+        function nc(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function zl(e) {
+        function rc(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Bl(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Bl(Object(n)).forEach((function(t) {
+                t % 2 ? nc(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : nc(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Kl = {
+        var ac = {
                 start: "align-self-start",
                 center: "align-self-center",
                 end: "align-self-end"
             },
-            Hl = ["width", "xs", "sm", "md", "lg", "xl", "xxl"],
-            Wl = function(t) {
+            sc = ["width", "xs", "sm", "md", "lg", "xl", "xxl"],
+            oc = function(t) {
                 var n = t.children,
                     r = t.html_for,
                     a = t.width,
                     s = t.xs,
                     i = t.sm,
                     c = t.md,
                     u = t.lg,
@@ -7407,152 +7545,152 @@
                     g = t.size,
                     y = t.className,
                     h = t.class_name,
                     v = t.color,
                     _ = t.style,
                     x = t.loading_state,
                     O = t.check,
-                    w = o(t, Fl),
-                    N = jt.has(v),
-                    E = Hl.filter((function(e) {
+                    w = o(t, tc),
+                    N = wt.has(v),
+                    E = sc.filter((function(e) {
                         return t[e]
                     }));
                 [a, s, i, c, u, d, p].forEach((function(e) {
-                    "object" === De(e) && null !== e && (e.span = e.size)
+                    "object" === Te(e) && null !== e && (e.span = e.size)
                 }));
-                var j = f && Kl[f],
+                var j = f && ac[f],
                     k = b()(h || y, E.length && j, v && N && "text-".concat(v), O && "form-check-label");
-                return l().createElement(qi, e({
+                return l().createElement(il, e({
                     htmlFor: r,
                     column: g || E.length > 0,
                     xs: s || a,
                     sm: i,
                     md: c,
                     lg: u,
                     xl: d,
                     xxl: p,
                     className: k,
-                    style: N ? _ : zl({
+                    style: N ? _ : rc({
                         color: v
                     }, _)
                 }, m(["setProps"], w), {
                     "data-dash-is-loading": x && x.is_loading || void 0
                 }), n)
             },
-            Ul = u().oneOfType([u().number, u().string]),
-            ql = u().oneOfType([u().string, u().number, u().shape({
-                size: Ul,
-                order: Ul,
-                offset: Ul
+            ic = u().oneOfType([u().number, u().string]),
+            lc = u().oneOfType([u().string, u().number, u().shape({
+                size: ic,
+                order: ic,
+                offset: ic
             })]);
-        Wl.propTypes = {
+        oc.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             hidden: u().bool,
             size: u().string,
             html_for: u().string,
             check: u().bool,
-            width: ql,
-            xs: ql,
-            sm: ql,
-            md: ql,
-            lg: ql,
-            xl: ql,
+            width: lc,
+            xs: lc,
+            sm: lc,
+            md: lc,
+            lg: lc,
+            xl: lc,
             align: u().oneOf(["start", "center", "end"]),
             color: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
-        }, Wl.defaultProps = {
+        }, oc.defaultProps = {
             align: "center"
         };
-        const Vl = Wl,
-            Gl = i.forwardRef((({
+        const cc = oc,
+            uc = i.forwardRef((({
                 bsPrefix: e,
                 active: t,
                 disabled: n,
                 eventKey: r,
                 className: a,
                 variant: s,
                 action: o,
                 as: i,
                 ...l
             }, c) => {
-                e = j(e, "list-group-item");
-                const [u, d] = ti({
-                    key: vo(r, l.href),
+                e = E(e, "list-group-item");
+                const [u, d] = mi({
+                    key: Co(r, l.href),
                     active: t,
                     ...l
-                }), p = Xe((e => {
+                }), p = Ye((e => {
                     if (n) return e.preventDefault(), void e.stopPropagation();
                     u.onClick(e)
                 }));
                 n && void 0 === l.tabIndex && (l.tabIndex = -1, l["aria-disabled"] = !0);
                 const f = i || (o ? l.href ? "a" : "button" : "div");
                 return (0, _.jsx)(f, {
                     ref: c,
                     ...l,
                     ...u,
                     onClick: p,
                     className: b()(a, e, d.isActive && "active", n && "disabled", s && `${e}-${s}`, o && `${e}-action`)
                 })
             }));
-        Gl.displayName = "ListGroupItem";
-        const Yl = Gl,
-            Xl = i.forwardRef(((e, t) => {
+        uc.displayName = "ListGroupItem";
+        const dc = uc,
+            pc = i.forwardRef(((e, t) => {
                 const {
                     className: n,
                     bsPrefix: r,
                     variant: a,
                     horizontal: s,
                     numbered: o,
                     as: i = "div",
                     ...l
                 } = v(e, {
                     activeKey: "onSelect"
-                }), c = j(r, "list-group");
+                }), c = E(r, "list-group");
                 let u;
-                return s && (u = !0 === s ? "horizontal" : `horizontal-${s}`), (0, _.jsx)(li, {
+                return s && (u = !0 === s ? "horizontal" : `horizontal-${s}`), (0, _.jsx)(xi, {
                     ref: t,
                     ...l,
                     as: i,
                     className: b()(n, c, a && `${c}-${a}`, u && `${c}-${u}`, o && `${c}-numbered`)
                 })
             }));
-        Xl.displayName = "ListGroup";
-        const Jl = Object.assign(Xl, {
-            Item: Yl
+        pc.displayName = "ListGroup";
+        const fc = Object.assign(pc, {
+            Item: dc
         });
-        var Ql = ["children", "loading_state", "className", "class_name", "flush", "tag"],
-            Zl = function(t) {
+        var mc = ["children", "loading_state", "className", "class_name", "flush", "tag"],
+            gc = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.flush,
                     c = t.tag,
-                    u = o(t, Ql);
-                return l().createElement(Jl, e({
+                    u = o(t, mc);
+                return l().createElement(fc, e({
                     className: s || a,
                     variant: i ? "flush" : null,
                     as: c
                 }, m(["setProps"], u), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Zl.defaultProps = {
+        gc.defaultProps = {
             tag: "ul",
             numbered: !1
-        }, Zl.propTypes = {
+        }, gc.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
@@ -7561,77 +7699,78 @@
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             horizontal: u().oneOfType([u().bool, u().string]),
             numbered: u().bool
         };
-        const ec = Zl;
-        var tc = ["children", "disabled", "href", "loading_state", "target", "n_clicks", "setProps", "color", "style", "className", "class_name"];
+        const bc = gc;
+        var yc = ["children", "disabled", "href", "loading_state", "target", "n_clicks", "setProps", "color", "style", "className", "class_name"];
 
-        function nc(e, t) {
+        function hc(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function rc(e) {
+        function vc(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? nc(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : nc(Object(n)).forEach((function(t) {
+                t % 2 ? hc(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : hc(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var ac = function(t) {
+        var _c = function(t) {
             var n = t.children,
                 r = t.disabled,
                 a = t.href,
                 s = t.loading_state,
                 i = t.target,
                 c = t.n_clicks,
                 u = t.setProps,
                 d = t.color,
                 p = t.style,
                 f = t.className,
                 g = t.class_name,
-                b = o(t, tc),
-                y = Et.has(d),
-                h = a && !r;
-            return b[h ? "preOnClick" : "onClick"] = function() {
+                b = o(t, yc),
+                y = Fe(a, u),
+                h = Ot.has(d),
+                v = y && !r;
+            return b[v ? "preOnClick" : "onClick"] = function() {
                 !r && u && u({
                     n_clicks: c + 1,
                     n_clicks_timestamp: Date.now()
                 })
-            }, l().createElement(Yl, e({
-                as: h ? Kt : "li",
-                href: a,
-                target: h ? i : void 0,
+            }, l().createElement(dc, e({
+                as: v ? Bt : "li",
+                href: y,
+                target: v ? i : void 0,
                 disabled: r,
-                variant: y ? d : null,
-                style: y ? p : rc({
+                variant: h ? d : null,
+                style: h ? p : vc({
                     backgroundColor: d
                 }, p),
                 className: g || f
             }, m(["n_clicks_timestamp"], b), {
                 "data-dash-is-loading": s && s.is_loading || void 0
             }), n)
         };
-        ac.defaultProps = {
+        _c.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, ac.propTypes = {
+        }, _c.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
@@ -7646,36 +7785,36 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
         };
-        const sc = ac;
-        var oc;
+        const xc = _c;
+        var Oc;
 
-        function ic(e) {
-            if ((!oc && 0 !== oc || e) && G) {
+        function wc(e) {
+            if ((!Oc && 0 !== Oc || e) && V) {
                 var t = document.createElement("div");
-                t.style.position = "absolute", t.style.top = "-9999px", t.style.width = "50px", t.style.height = "50px", t.style.overflow = "scroll", document.body.appendChild(t), oc = t.offsetWidth - t.clientWidth, document.body.removeChild(t)
+                t.style.position = "absolute", t.style.top = "-9999px", t.style.width = "50px", t.style.height = "50px", t.style.overflow = "scroll", document.body.appendChild(t), Oc = t.offsetWidth - t.clientWidth, document.body.removeChild(t)
             }
-            return oc
+            return Oc
         }
 
-        function lc(e) {
-            void 0 === e && (e = T());
+        function Nc(e) {
+            void 0 === e && (e = C());
             try {
                 var t = e.activeElement;
                 return t && t.nodeName ? t : null
             } catch (t) {
                 return e.body
             }
         }
-        const cc = No("modal-open"),
-            uc = class {
+        const Ec = Lo("modal-open"),
+            jc = class {
                 constructor({
                     ownerDocument: e,
                     handleContainerOverflow: t = !0,
                     isRTL: n = !1
                 } = {}) {
                     this.handleContainerOverflow = t, this.isRTL = n, this.modals = [], this.ownerDocument = e
                 }
@@ -7695,22 +7834,22 @@
                             overflow: "hidden"
                         },
                         n = this.isRTL ? "paddingLeft" : "paddingRight",
                         r = this.getElement();
                     e.style = {
                         overflow: r.style.overflow,
                         [n]: r.style[n]
-                    }, e.scrollBarWidth && (t[n] = `${parseInt($(r,n)||"0",10)+e.scrollBarWidth}px`), r.setAttribute(cc, ""), $(r, t)
+                    }, e.scrollBarWidth && (t[n] = `${parseInt(L(r,n)||"0",10)+e.scrollBarWidth}px`), r.setAttribute(Ec, ""), L(r, t)
                 }
                 reset() {
                     [...this.modals].forEach((e => this.remove(e)))
                 }
                 removeContainerStyle(e) {
                     const t = this.getElement();
-                    t.removeAttribute(cc), Object.assign(t.style, e.style)
+                    t.removeAttribute(Ec), Object.assign(t.style, e.style)
                 }
                 add(e) {
                     let t = this.modals.indexOf(e);
                     return -1 !== t || (t = this.modals.length, this.modals.push(e), this.setModalAttributes(e), 0 !== t || (this.state = {
                         scrollBarWidth: this.getScrollbarWidth(),
                         style: {}
                     }, this.handleContainerOverflow && this.setContainerStyle(this.state))), t
@@ -7718,108 +7857,179 @@
                 remove(e) {
                     const t = this.modals.indexOf(e); - 1 !== t && (this.modals.splice(t, 1), !this.modals.length && this.handleContainerOverflow && this.removeContainerStyle(this.state), this.removeModalAttributes(e))
                 }
                 isTopModal(e) {
                     return !!this.modals.length && this.modals[this.modals.length - 1] === e
                 }
             },
-            dc = (e, t) => G ? null == e ? (t || T()).body : ("function" == typeof e && (e = e()), e && "current" in e && (e = e.current), e && ("nodeType" in e || e.getBoundingClientRect) ? e : null) : null;
+            kc = (e, t) => V ? null == e ? (t || C()).body : ("function" == typeof e && (e = e()), e && "current" in e && (e = e.current), e && ("nodeType" in e || e.getBoundingClientRect) ? e : null) : null;
 
-        function pc(e, t) {
-            const n = To(),
-                [r, a] = (0, i.useState)((() => dc(e, null == n ? void 0 : n.document)));
+        function Pc(e, t) {
+            const n = Bo(),
+                [r, a] = (0, i.useState)((() => kc(e, null == n ? void 0 : n.document)));
             if (!r) {
-                const t = dc(e);
+                const t = kc(e);
                 t && a(t)
             }
             return (0, i.useEffect)((() => {
                 t && r && t(r)
             }), [t, r]), (0, i.useEffect)((() => {
-                const t = dc(e);
+                const t = kc(e);
                 t !== r && a(t)
             }), [e, r]), r
         }
-        const fc = function({
-            children: e,
-            in: t,
-            onExited: n,
-            mountOnEnter: r,
-            unmountOnExit: a
-        }) {
-            const s = (0, i.useRef)(null),
-                o = (0, i.useRef)(t),
-                l = Xe(n);
-            (0, i.useEffect)((() => {
-                t ? o.current = !0 : l(s.current)
-            }), [t, l]);
-            const c = ie(s, e.ref),
-                u = (0, i.cloneElement)(e, {
-                    ref: c
-                });
-            return t ? u : a || !o.current && r ? null : u
-        };
+        const Cc = function({
+                children: e,
+                in: t,
+                onExited: n,
+                mountOnEnter: r,
+                unmountOnExit: a
+            }) {
+                const s = (0, i.useRef)(null),
+                    o = (0, i.useRef)(t),
+                    l = Ye(n);
+                (0, i.useEffect)((() => {
+                    t ? o.current = !0 : l(s.current)
+                }), [t, l]);
+                const c = oe(s, e.ref),
+                    u = (0, i.cloneElement)(e, {
+                        ref: c
+                    });
+                return t ? u : a || !o.current && r ? null : u
+            },
+            Tc = ["onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited", "addEndListener", "children"];
+        const Sc = ["component"],
+            Rc = i.forwardRef(((e, t) => {
+                let {
+                    component: n
+                } = e;
+                const r = function(e) {
+                    let {
+                        onEnter: t,
+                        onEntering: n,
+                        onEntered: r,
+                        onExit: a,
+                        onExiting: s,
+                        onExited: o,
+                        addEndListener: l,
+                        children: c
+                    } = e, u = function(e, t) {
+                        if (null == e) return {};
+                        var n, r, a = {},
+                            s = Object.keys(e);
+                        for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
+                        return a
+                    }(e, Tc);
+                    const d = (0, i.useRef)(null),
+                        p = oe(d, "function" == typeof c ? null : c.ref),
+                        f = e => t => {
+                            e && d.current && e(d.current, t)
+                        },
+                        m = (0, i.useCallback)(f(t), [t]),
+                        g = (0, i.useCallback)(f(n), [n]),
+                        b = (0, i.useCallback)(f(r), [r]),
+                        y = (0, i.useCallback)(f(a), [a]),
+                        h = (0, i.useCallback)(f(s), [s]),
+                        v = (0, i.useCallback)(f(o), [o]),
+                        _ = (0, i.useCallback)(f(l), [l]);
+                    return Object.assign({}, u, {
+                        nodeRef: d
+                    }, t && {
+                        onEnter: m
+                    }, n && {
+                        onEntering: g
+                    }, r && {
+                        onEntered: b
+                    }, a && {
+                        onExit: y
+                    }, s && {
+                        onExiting: h
+                    }, o && {
+                        onExited: v
+                    }, l && {
+                        addEndListener: _
+                    }, {
+                        children: "function" == typeof c ? (e, t) => c(e, Object.assign({}, t, {
+                            ref: p
+                        })) : (0, i.cloneElement)(c, {
+                            ref: p
+                        })
+                    })
+                }(function(e, t) {
+                    if (null == e) return {};
+                    var n, r, a = {},
+                        s = Object.keys(e);
+                    for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
+                    return a
+                }(e, Sc));
+                return (0, _.jsx)(n, Object.assign({
+                    ref: t
+                }, r))
+            }));
 
-        function mc({
+        function Dc({
             children: e,
             in: t,
             onExited: n,
             onEntered: r,
             transition: a
         }) {
             const [s, o] = (0, i.useState)(!t);
             t && s && o(!1);
             const l = function({
                     in: e,
                     onTransition: t
                 }) {
                     const n = (0, i.useRef)(null),
                         r = (0, i.useRef)(!0),
-                        a = Xe(t);
-                    return tt((() => {
+                        a = Ye(t);
+                    return at((() => {
                         if (!n.current) return;
                         let t = !1;
                         return a({
                             in: e,
                             element: n.current,
                             initial: r.current,
                             isStale: () => t
                         }), () => {
                             t = !0
                         }
-                    }), [e, a]), tt((() => (r.current = !1, () => {
+                    }), [e, a]), at((() => (r.current = !1, () => {
                         r.current = !0
                     })), []), n
                 }({
                     in: !!t,
                     onTransition: e => {
                         Promise.resolve(a(e)).then((() => {
                             e.isStale() || (e.in ? null == r || r(e.element, e.initial) : (o(!0), null == n || n(e.element)))
                         }), (t => {
                             throw e.in || o(!0), t
                         }))
                     }
                 }),
-                c = ie(l, e.ref);
+                c = oe(l, e.ref);
             return s && !t ? null : (0, i.cloneElement)(e, {
                 ref: c
             })
         }
 
-        function gc(e, t, n) {
-            return e ? (0, _.jsx)(e, Object.assign({}, n)) : t ? (0, _.jsx)(mc, Object.assign({}, n, {
+        function Lc(e, t, n) {
+            return e ? (0, _.jsx)(Rc, Object.assign({}, n, {
+                component: e
+            })) : t ? (0, _.jsx)(Dc, Object.assign({}, n, {
                 transition: t
-            })) : (0, _.jsx)(fc, Object.assign({}, n))
+            })) : (0, _.jsx)(Cc, Object.assign({}, n))
         }
 
-        function bc(e) {
+        function $c(e) {
             return "Escape" === e.code || 27 === e.keyCode
         }
-        const yc = ["show", "role", "className", "style", "children", "backdrop", "keyboard", "onBackdropClick", "onEscapeKeyDown", "transition", "runTransition", "backdropTransition", "runBackdropTransition", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "renderDialog", "renderBackdrop", "manager", "container", "onShow", "onHide", "onExit", "onExited", "onExiting", "onEnter", "onEntering", "onEntered"];
-        let hc;
-        const vc = (0, i.forwardRef)(((e, t) => {
+        const Ic = ["show", "role", "className", "style", "children", "backdrop", "keyboard", "onBackdropClick", "onEscapeKeyDown", "transition", "runTransition", "backdropTransition", "runBackdropTransition", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "renderDialog", "renderBackdrop", "manager", "container", "onShow", "onHide", "onExit", "onExited", "onExiting", "onEnter", "onEntering", "onEntered"];
+        let Ac;
+        const Fc = (0, i.forwardRef)(((e, t) => {
             let {
                 show: n = !1,
                 role: r = "dialog",
                 className: a,
                 style: s,
                 children: o,
                 backdrop: l = !0,
@@ -7848,22 +8058,23 @@
                 onEntered: R
             } = e, D = function(e, t) {
                 if (null == e) return {};
                 var n, r, a = {},
                     s = Object.keys(e);
                 for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
                 return a
-            }(e, yc);
-            const L = pc(N),
-                $ = function(e) {
-                    const t = To(),
+            }(e, Ic);
+            const L = Bo(),
+                $ = Pc(N),
+                I = function(e) {
+                    const t = Bo(),
                         n = e || function(e) {
-                            return hc || (hc = new uc({
+                            return Ac || (Ac = new jc({
                                 ownerDocument: null == e ? void 0 : e.document
-                            })), hc
+                            })), Ac
                         }(t),
                         r = (0, i.useRef)({
                             dialog: null,
                             backdrop: null
                         });
                     return Object.assign(r.current, {
                         add: () => n.add(r.current),
@@ -7873,222 +8084,223 @@
                             r.current.dialog = e
                         }), []),
                         setBackdropRef: (0, i.useCallback)((e => {
                             r.current.backdrop = e
                         }), [])
                     })
                 }(w),
-                I = Qe(),
-                A = Ze(n),
-                [F, B] = (0, i.useState)(!n),
-                z = (0, i.useRef)(null);
-            (0, i.useImperativeHandle)(t, (() => $), [$]), G && !A && n && (z.current = lc()), n && F && B(!1);
-            const K = Xe((() => {
-                    if ($.add(), Y.current = ee(document, "keydown", q), V.current = ee(document, "focus", (() => setTimeout(W)), !0), E && E(), b) {
-                        const e = lc(document);
-                        $.dialog && e && !Gs($.dialog, e) && (z.current = e, $.dialog.focus())
+                F = tt(),
+                M = nt(n),
+                [B, z] = (0, i.useState)(!n),
+                K = (0, i.useRef)(null);
+            (0, i.useImperativeHandle)(t, (() => I), [I]), V && !M && n && (K.current = Nc(null == L ? void 0 : L.document)), n && B && z(!1);
+            const H = Ye((() => {
+                    if (I.add(), X.current = Z(document, "keydown", G), Y.current = Z(document, "focus", (() => setTimeout(W)), !0), E && E(), b) {
+                        var e, t;
+                        const n = Nc(null != (e = null == (t = I.dialog) ? void 0 : t.ownerDocument) ? e : null == L ? void 0 : L.document);
+                        I.dialog && n && !eo(I.dialog, n) && (K.current = n, I.dialog.focus())
                     }
                 })),
-                H = Xe((() => {
+                U = Ye((() => {
                     var e;
-                    $.remove(), null == Y.current || Y.current(), null == V.current || V.current(), h && (null == (e = z.current) || null == e.focus || e.focus(v), z.current = null)
+                    I.remove(), null == X.current || X.current(), null == Y.current || Y.current(), h && (null == (e = K.current) || null == e.focus || e.focus(v), K.current = null)
                 }));
             (0, i.useEffect)((() => {
-                n && L && K()
-            }), [n, L, K]), (0, i.useEffect)((() => {
-                F && H()
-            }), [F, H]), nr((() => {
-                H()
-            }));
-            const W = Xe((() => {
-                    if (!y || !I() || !$.isTopModal()) return;
-                    const e = lc();
-                    $.dialog && e && !Gs($.dialog, e) && $.dialog.focus()
+                n && $ && H()
+            }), [n, $, H]), (0, i.useEffect)((() => {
+                B && U()
+            }), [B, U]), ur((() => {
+                U()
+            }));
+            const W = Ye((() => {
+                    if (!y || !F() || !I.isTopModal()) return;
+                    const e = Nc(null == L ? void 0 : L.document);
+                    I.dialog && e && !eo(I.dialog, e) && I.dialog.focus()
                 })),
-                U = Xe((e => {
+                q = Ye((e => {
                     e.target === e.currentTarget && (null == u || u(e), !0 === l && j())
                 })),
-                q = Xe((e => {
-                    c && bc(e) && $.isTopModal() && (null == d || d(e), e.defaultPrevented || j())
+                G = Ye((e => {
+                    c && $c(e) && I.isTopModal() && (null == d || d(e), e.defaultPrevented || j())
                 })),
-                V = (0, i.useRef)(),
-                Y = (0, i.useRef)();
-            if (!L) return null;
-            const X = Object.assign({
+                Y = (0, i.useRef)(),
+                X = (0, i.useRef)();
+            if (!$) return null;
+            const J = Object.assign({
                 role: r,
-                ref: $.setDialogRef,
+                ref: I.setDialogRef,
                 "aria-modal": "dialog" === r || void 0
             }, D, {
                 style: s,
                 className: a,
                 tabIndex: -1
             });
-            let J = x ? x(X) : (0, _.jsx)("div", Object.assign({}, X, {
+            let Q = x ? x(J) : (0, _.jsx)("div", Object.assign({}, J, {
                 children: i.cloneElement(o, {
                     role: "document"
                 })
             }));
-            J = gc(p, f, {
+            Q = Lc(p, f, {
                 unmountOnExit: !0,
                 mountOnEnter: !0,
                 appear: !0,
                 in: !!n,
                 onExit: k,
                 onExiting: C,
                 onExited: (...e) => {
-                    B(!0), null == P || P(...e)
+                    z(!0), null == P || P(...e)
                 },
                 onEnter: T,
                 onEntering: S,
                 onEntered: R,
-                children: J
+                children: Q
             });
-            let Q = null;
-            return l && (Q = O({
-                ref: $.setBackdropRef,
-                onClick: U
-            }), Q = gc(m, g, {
+            let ee = null;
+            return l && (ee = O({
+                ref: I.setBackdropRef,
+                onClick: q
+            }), ee = Lc(m, g, {
                 in: !!n,
                 appear: !0,
                 mountOnEnter: !0,
                 unmountOnExit: !0,
-                children: Q
+                children: ee
             })), (0, _.jsx)(_.Fragment, {
-                children: M().createPortal((0, _.jsxs)(_.Fragment, {
-                    children: [Q, J]
-                }), L)
+                children: A().createPortal((0, _.jsxs)(_.Fragment, {
+                    children: [ee, Q]
+                }), $)
             })
         }));
-        vc.displayName = "Modal";
-        const _c = Object.assign(vc, {
-            Manager: uc
+        Fc.displayName = "Modal";
+        const Mc = Object.assign(Fc, {
+            Manager: jc
         });
 
-        function xc(e, t) {
+        function Bc(e, t) {
             return e.classList ? !!t && e.classList.contains(t) : -1 !== (" " + (e.className.baseVal || e.className) + " ").indexOf(" " + t + " ")
         }
 
-        function Oc(e, t) {
+        function zc(e, t) {
             return e.replace(new RegExp("(^|\\s)" + t + "(?:\\s|$)", "g"), "$1").replace(/\s+/g, " ").replace(/^\s*|\s*$/g, "")
         }
-        const wc = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
-            Nc = ".sticky-top",
-            Ec = ".navbar-toggler";
-        class jc extends uc {
+        const Kc = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
+            Hc = ".sticky-top",
+            Uc = ".navbar-toggler";
+        class Wc extends jc {
             adjustAndStore(e, t, n) {
                 const r = t.style[e];
-                t.dataset[e] = r, $(t, {
-                    [e]: `${parseFloat($(t,e))+n}px`
+                t.dataset[e] = r, L(t, {
+                    [e]: `${parseFloat(L(t,e))+n}px`
                 })
             }
             restore(e, t) {
                 const n = t.dataset[e];
-                void 0 !== n && (delete t.dataset[e], $(t, {
+                void 0 !== n && (delete t.dataset[e], L(t, {
                     [e]: n
                 }))
             }
             setContainerStyle(e) {
                 super.setContainerStyle(e);
                 const t = this.getElement();
                 var n, r;
-                if (r = "modal-open", (n = t).classList ? n.classList.add(r) : xc(n, r) || ("string" == typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)), !e.scrollBarWidth) return;
+                if (r = "modal-open", (n = t).classList ? n.classList.add(r) : Bc(n, r) || ("string" == typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)), !e.scrollBarWidth) return;
                 const a = this.isRTL ? "paddingLeft" : "paddingRight",
                     s = this.isRTL ? "marginLeft" : "marginRight";
-                xa(t, wc).forEach((t => this.adjustAndStore(a, t, e.scrollBarWidth))), xa(t, Nc).forEach((t => this.adjustAndStore(s, t, -e.scrollBarWidth))), xa(t, Ec).forEach((t => this.adjustAndStore(s, t, e.scrollBarWidth)))
+                Ca(t, Kc).forEach((t => this.adjustAndStore(a, t, e.scrollBarWidth))), Ca(t, Hc).forEach((t => this.adjustAndStore(s, t, -e.scrollBarWidth))), Ca(t, Uc).forEach((t => this.adjustAndStore(s, t, e.scrollBarWidth)))
             }
             removeContainerStyle(e) {
                 super.removeContainerStyle(e);
                 const t = this.getElement();
                 var n, r;
-                r = "modal-open", (n = t).classList ? n.classList.remove(r) : "string" == typeof n.className ? n.className = Oc(n.className, r) : n.setAttribute("class", Oc(n.className && n.className.baseVal || "", r));
+                r = "modal-open", (n = t).classList ? n.classList.remove(r) : "string" == typeof n.className ? n.className = zc(n.className, r) : n.setAttribute("class", zc(n.className && n.className.baseVal || "", r));
                 const a = this.isRTL ? "paddingLeft" : "paddingRight",
                     s = this.isRTL ? "marginLeft" : "marginRight";
-                xa(t, wc).forEach((e => this.restore(a, e))), xa(t, Nc).forEach((e => this.restore(s, e))), xa(t, Ec).forEach((e => this.restore(s, e)))
+                Ca(t, Kc).forEach((e => this.restore(a, e))), Ca(t, Hc).forEach((e => this.restore(s, e))), Ca(t, Uc).forEach((e => this.restore(s, e)))
             }
         }
-        let kc;
+        let qc;
 
-        function Pc(e) {
-            return kc || (kc = new jc(e)), kc
+        function Vc(e) {
+            return qc || (qc = new Wc(e)), qc
         }
-        const Cc = jc,
-            Tc = i.createContext({
+        const Gc = Wc,
+            Yc = i.createContext({
                 onHide() {}
             }),
-            Sc = i.forwardRef((({
+            Xc = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 contentClassName: n,
                 centered: r,
                 size: a,
                 fullscreen: s,
                 children: o,
                 scrollable: i,
                 ...l
             }, c) => {
-                const u = `${e=j(e,"modal")}-dialog`,
+                const u = `${e=E(e,"modal")}-dialog`,
                     d = "string" == typeof s ? `${e}-fullscreen-${s}` : `${e}-fullscreen`;
                 return (0, _.jsx)("div", {
                     ...l,
                     ref: c,
                     className: b()(u, t, a && `${e}-${a}`, r && `${u}-centered`, i && `${u}-scrollable`, s && d),
                     children: (0, _.jsx)("div", {
                         className: b()(`${e}-content`, n),
                         children: o
                     })
                 })
             }));
-        Sc.displayName = "ModalDialog";
-        var Rc = ["bsPrefix", "className", "style", "dialogClassName", "contentClassName", "children", "dialogAs", "aria-labelledby", "aria-describedby", "aria-label", "show", "animation", "backdrop", "keyboard", "onEscapeKeyDown", "onShow", "onHide", "container", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "onEntered", "onExit", "onExiting", "onEnter", "onEntering", "onExited", "backdropClassName", "zIndex", "manager"];
+        Xc.displayName = "ModalDialog";
+        var Jc = ["bsPrefix", "className", "style", "dialogClassName", "contentClassName", "children", "dialogAs", "aria-labelledby", "aria-describedby", "aria-label", "show", "animation", "backdrop", "keyboard", "onEscapeKeyDown", "onShow", "onHide", "container", "autoFocus", "enforceFocus", "restoreFocus", "restoreFocusOptions", "onEntered", "onExit", "onExiting", "onEnter", "onEntering", "onExited", "backdropClassName", "zIndex", "manager"];
 
-        function Dc(e, t) {
+        function Qc(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Lc(e) {
+        function Zc(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Dc(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Dc(Object(n)).forEach((function(t) {
+                t % 2 ? Qc(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Qc(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var $c = {
+        var eu = {
             show: !1,
             backdrop: !0,
             keyboard: !0,
             autoFocus: !0,
             enforceFocus: !0,
             restoreFocus: !0,
             animation: !0,
-            dialogAs: Sc
+            dialogAs: Xc
         };
 
-        function Ic(t) {
-            return l().createElement(dt, e({}, t, {
+        function tu(t) {
+            return l().createElement(bt, e({}, t, {
                 timeout: null
             }))
         }
 
-        function Ac(t) {
-            return l().createElement(dt, e({}, t, {
+        function nu(t) {
+            return l().createElement(bt, e({}, t, {
                 timeout: null
             }))
         }
-        var Mc = l().forwardRef((function(t, n) {
+        var ru = l().forwardRef((function(t, n) {
             var r = t.bsPrefix,
                 a = t.className,
                 s = t.style,
                 c = t.dialogClassName,
                 u = t.contentClassName,
                 d = t.children,
                 p = t.dialogAs,
@@ -8099,133 +8311,133 @@
                 h = t.animation,
                 v = t.backdrop,
                 _ = t.keyboard,
                 x = t.onEscapeKeyDown,
                 O = t.onShow,
                 w = t.onHide,
                 N = t.container,
-                E = t.autoFocus,
+                j = t.autoFocus,
                 k = t.enforceFocus,
-                P = t.restoreFocus,
+                T = t.restoreFocus,
                 S = t.restoreFocusOptions,
                 R = t.onEntered,
                 D = t.onExit,
                 L = t.onExiting,
                 $ = t.onEnter,
                 I = t.onEntering,
                 A = t.onExited,
-                M = t.backdropClassName,
-                F = t.zIndex,
+                F = t.backdropClassName,
+                M = t.zIndex,
                 B = t.manager,
-                z = o(t, Rc),
-                K = Le((0, i.useState)({}), 2),
+                z = o(t, Jc),
+                K = Se((0, i.useState)({}), 2),
                 H = K[0],
-                W = K[1],
-                U = Le((0, i.useState)(!1), 2),
-                q = U[0],
-                V = U[1],
+                U = K[1],
+                W = Se((0, i.useState)(!1), 2),
+                q = W[0],
+                G = W[1],
                 Y = (0, i.useRef)(!1),
                 X = (0, i.useRef)(!1),
-                J = (0, i.useRef)(null),
-                ee = Le(Je(), 2),
-                ne = ee[0],
-                re = ee[1],
-                ae = ie(n, re),
-                se = Xe(w),
-                oe = C();
-            r = j(r, "modal");
+                Z = (0, i.useRef)(null),
+                te = Se(et(), 2),
+                ne = te[0],
+                re = te[1],
+                ae = oe(n, re),
+                se = Ye(w),
+                ie = P();
+            r = E(r, "modal");
             var le = (0, i.useMemo)((function() {
                 return {
                     onHide: se
                 }
             }), [se]);
 
             function ce() {
-                return B || Pc({
-                    isRTL: oe
+                return B || Vc({
+                    isRTL: ie
                 })
             }
 
             function ue(e) {
-                if (G) {
+                if (V) {
                     var t = ce().getScrollbarWidth() > 0,
-                        n = e.scrollHeight > T(e).documentElement.clientHeight;
-                    W({
-                        paddingRight: t && !n ? ic() : void 0,
-                        paddingLeft: !t && n ? ic() : void 0
+                        n = e.scrollHeight > C(e).documentElement.clientHeight;
+                    U({
+                        paddingRight: t && !n ? wc() : void 0,
+                        paddingLeft: !t && n ? wc() : void 0
                     })
                 }
             }
-            var de = Xe((function() {
+            var de = Ye((function() {
                 ne && ue(ne.dialog)
             }));
-            nr((function() {
+            ur((function() {
                 var e;
-                Z(window, "resize", de), null === (e = J.current) || void 0 === e || e.call(J)
+                Q(window, "resize", de), null === (e = Z.current) || void 0 === e || e.call(Z)
             }));
             var pe = function() {
                     Y.current = !0
                 },
                 fe = function(e) {
                     Y.current && ne && e.target === ne.dialog && (X.current = !0), Y.current = !1
                 },
                 me = function() {
-                    V(!0), J.current = te(ne.dialog, (function() {
-                        V(!1)
+                    G(!0), Z.current = ee(ne.dialog, (function() {
+                        G(!1)
                     }))
                 },
                 ge = function(e) {
                     "static" !== v ? X.current || e.target !== e.currentTarget ? X.current = !1 : null == w || w() : function(e) {
                         e.target === e.currentTarget && me()
                     }(e)
                 },
                 be = (0, i.useCallback)((function(t) {
                     return l().createElement("div", e({}, t, {
-                        className: b()("".concat(r, "-backdrop"), M, !h && "show"),
+                        className: b()("".concat(r, "-backdrop"), F, !h && "show"),
                         style: {
-                            zIndex: F
+                            zIndex: M
                         }
                     }))
-                }), [h, M, r, F]),
-                ye = Lc(Lc({}, s), H);
-            return ye.display = "block", l().createElement(Tc.Provider, {
+                }), [h, F, r, M]),
+                ye = Zc(Zc({}, s), H);
+            return ye.display = "block", l().createElement(Yc.Provider, {
                 value: le
-            }, l().createElement(_c, {
+            }, l().createElement(Mc, {
                 show: y,
                 ref: ae,
                 backdrop: v,
                 container: N,
                 keyboard: !0,
-                autoFocus: E,
+                autoFocus: j,
                 enforceFocus: k,
-                restoreFocus: P,
+                restoreFocus: T,
                 restoreFocusOptions: S,
                 onEscapeKeyDown: function(e) {
                     _ || "static" !== v ? _ && x && x(e) : (e.preventDefault(), me())
                 },
                 onShow: O,
                 onHide: w,
                 onEnter: function(e, t) {
                     e && ue(e), null == $ || $(e, t)
                 },
                 onEntering: function(e, t) {
-                    null == I || I(e, t), Q(window, "resize", de)
+                    null == I || I(e, t), J(window, "resize", de)
                 },
                 onEntered: R,
                 onExit: function(e) {
                     var t;
-                    null === (t = J.current) || void 0 === t || t.call(J), null == D || D(e)
+                    null === (t = Z.current) || void 0 === t || t.call(Z), null == D || D(e)
                 },
                 onExiting: L,
                 onExited: function(e) {
-                    e && (e.style.display = ""), null == A || A(e), Z(window, "resize", de)
+                    e && (e.style.display = ""), null == A || A(e), Q(window, "resize", de)
                 },
                 manager: ce(),
-                transition: h ? Ic : void 0,
-                backdropTransition: h ? Ac : void 0,
+                transition: h ? tu : void 0,
+                backdropTransition: h ? nu : void 0,
                 renderBackdrop: be,
                 renderDialog: function(t) {
                     return l().createElement("div", e({
                         role: "dialog"
                     }, t, {
                         style: ye,
                         className: b()(a, r, q && "".concat(r, "-static")),
@@ -8238,41 +8450,41 @@
                         onMouseDown: pe,
                         className: c,
                         contentClassName: u
                     }), d))
                 }
             }))
         }));
-        Mc.defaultProps = $c;
-        const Fc = Mc;
-        var Bc = ["children", "is_open", "setProps", "className", "class_name", "autoFocus", "autofocus", "enforceFocus", "labelledBy", "labelledby", "modalClassName", "modal_class_name", "contentClassName", "content_class_name", "backdropClassName", "backdrop_class_name", "tag", "loading_state", "fade", "style", "zindex", "zIndex"];
+        ru.defaultProps = eu;
+        const au = ru;
+        var su = ["children", "is_open", "setProps", "className", "class_name", "autoFocus", "autofocus", "enforceFocus", "labelledBy", "labelledby", "modalClassName", "modal_class_name", "contentClassName", "content_class_name", "backdropClassName", "backdrop_class_name", "tag", "loading_state", "fade", "style", "zindex", "zIndex"];
 
-        function zc(e, t) {
+        function ou(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Kc(e) {
+        function iu(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? zc(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : zc(Object(n)).forEach((function(t) {
+                t % 2 ? ou(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ou(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Hc = function(t) {
+        var lu = function(t) {
             var n = t.children,
                 r = t.is_open,
                 a = t.setProps,
                 s = t.className,
                 i = t.class_name,
                 c = t.autoFocus,
                 u = t.autofocus,
@@ -8287,16 +8499,16 @@
                 _ = t.backdrop_class_name,
                 x = t.tag,
                 O = t.loading_state,
                 w = t.fade,
                 N = t.style,
                 E = t.zindex,
                 j = t.zIndex,
-                k = o(t, Bc);
-            return l().createElement(Fc, e({
+                k = o(t, su);
+            return l().createElement(au, e({
                 animation: w,
                 dialogAs: x,
                 dialogClassName: i || s,
                 className: b || g,
                 contentClassName: h || y,
                 backdropClassName: _ || v,
                 autoFocus: u || c,
@@ -8304,23 +8516,23 @@
                 "aria-labelledby": f || p,
                 show: r,
                 onHide: function() {
                     a && a({
                         is_open: !1
                     })
                 },
-                style: E || j ? Kc(Kc({}, N), {}, {
+                style: E || j ? iu(iu({}, N), {}, {
                     zIndex: E || j
                 }) : N,
                 zIndex: E || j
             }, m(["persistence", "persistence_type", "persisted_props"], k), {
                 "data-dash-is-loading": O && O.is_loading || void 0
             }), n)
         };
-        Hc.propTypes = {
+        lu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             is_open: u().bool,
@@ -8342,217 +8554,246 @@
             content_class_name: u().string,
             contentClassName: u().string,
             fade: u().bool,
             fullscreen: u().oneOf([u().bool, u().oneOf(["sm-down", "md-down", "lg-down", "xl-down", "xxl-down"])]),
             zindex: u().oneOfType([u().number, u().string]),
             zIndex: u().oneOfType([u().number, u().string])
         };
-        const Wc = Hc,
-            Uc = ht("modal-body");
-        var qc = ["children", "loading_state", "className", "class_name", "tag"],
-            Vc = function(t) {
+        const cu = lu,
+            uu = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "modal-body"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        uu.displayName = "ModalBody";
+        const du = uu;
+        var pu = ["children", "loading_state", "className", "class_name", "tag"],
+            fu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, qc);
-                return l().createElement(Uc, e({
+                    c = o(t, pu);
+                return l().createElement(du, e({
                     as: i,
                     className: s || a,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], c)), n)
             };
-        Vc.propTypes = {
+        fu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Gc = Vc,
-            Yc = ht("modal-footer");
-        var Xc = ["children", "loading_state", "className", "class_name", "tag"],
-            Jc = function(t) {
+        const mu = fu,
+            gu = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "modal-footer"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        gu.displayName = "ModalFooter";
+        const bu = gu;
+        var yu = ["children", "loading_state", "className", "class_name", "tag"],
+            hu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, Xc);
-                return l().createElement(Yc, e({
+                    c = o(t, yu);
+                return l().createElement(bu, e({
                     as: i,
                     className: s || a,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], c)), n)
             };
-        Jc.propTypes = {
+        hu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Qc = Jc,
-            Zc = i.forwardRef((({
-                closeLabel: e,
+        const vu = hu,
+            _u = i.forwardRef((({
+                closeLabel: e = "Close",
                 closeVariant: t,
-                closeButton: n,
+                closeButton: n = !1,
                 onHide: r,
                 children: a,
                 ...s
             }, o) => {
-                const l = (0, i.useContext)(Tc),
-                    c = Xe((() => {
+                const l = (0, i.useContext)(Yc),
+                    c = Ye((() => {
                         null == l || l.onHide(), null == r || r()
                     }));
                 return (0, _.jsxs)("div", {
                     ref: o,
                     ...s,
-                    children: [a, n && (0, _.jsx)(mt, {
+                    children: [a, n && (0, _.jsx)(vt, {
                         "aria-label": e,
                         variant: t,
                         onClick: c
                     })]
                 })
-            }));
-        Zc.defaultProps = {
-            closeLabel: "Close",
-            closeButton: !1
-        };
-        const eu = Zc,
-            tu = i.forwardRef((({
+            })),
+            xu = _u,
+            Ou = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                ...n
-            }, r) => (e = j(e, "modal-header"), (0, _.jsx)(eu, {
-                ref: r,
-                ...n,
-                className: b()(t, e)
+                closeLabel: n = "Close",
+                closeButton: r = !1,
+                ...a
+            }, s) => (e = E(e, "modal-header"), (0, _.jsx)(xu, {
+                ref: s,
+                ...a,
+                className: b()(t, e),
+                closeLabel: n,
+                closeButton: r
             }))));
-        tu.displayName = "ModalHeader", tu.defaultProps = {
-            closeLabel: "Close",
-            closeButton: !1
-        };
-        const nu = tu;
-        var ru = ["children", "loading_state", "className", "class_name", "tag", "close_button"],
-            au = function(t) {
+        Ou.displayName = "ModalHeader";
+        const wu = Ou;
+        var Nu = ["children", "loading_state", "className", "class_name", "tag", "close_button"],
+            Eu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
                     c = t.close_button,
-                    u = o(t, ru);
-                return l().createElement(nu, e({
+                    u = o(t, Nu);
+                return l().createElement(wu, e({
                     as: i,
                     className: s || a,
                     closeButton: c,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], u)), n)
             };
-        au.defaultProps = {
+        Eu.defaultProps = {
             close_button: !0
-        }, au.propTypes = {
+        }, Eu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             close_button: u().bool,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const su = au,
-            ou = ht("modal-title", {
-                Component: gt("h4")
-            });
-        var iu = ["children", "loading_state", "className", "class_name", "tag"],
-            lu = function(t) {
+        const ju = Eu,
+            ku = Xe("h4"),
+            Pu = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = ku,
+                ...r
+            }, a) => (t = E(t, "modal-title"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Pu.displayName = "ModalTitle";
+        const Cu = Pu;
+        var Tu = ["children", "loading_state", "className", "class_name", "tag"],
+            Su = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.tag,
-                    c = o(t, iu);
-                return l().createElement(ou, e({
+                    c = o(t, Tu);
+                return l().createElement(Cu, e({
                     as: i,
                     className: s || a,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }, m(["setProps"], c)), n)
             };
-        lu.propTypes = {
+        Su.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const cu = lu;
-        var uu = ["children", "loading_state", "className", "class_name", "pills", "justified", "horizontal", "vertical", "navbar_scroll"],
-            du = {
+        const Ru = Su;
+        var Du = ["children", "loading_state", "className", "class_name", "pills", "justified", "horizontal", "vertical", "navbar_scroll"],
+            Lu = {
                 start: "justify-content-start",
                 center: "justify-content-center",
                 end: "justify-content-end",
                 around: "justify-content-around",
                 between: "justify-content-between"
             },
-            pu = {
+            $u = {
                 xs: "flex-xs-column",
                 sm: "flex-sm-column",
                 md: "flex-md-column",
                 lg: "flex-lg-column",
                 xl: "flex-xl-column"
             },
-            fu = function(t) {
+            Iu = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.pills,
                     c = t.justified,
                     u = t.horizontal,
                     d = t.vertical,
                     p = t.navbar_scroll,
-                    f = o(t, uu),
-                    g = u && du[u],
-                    y = !0 === d ? "flex-column" : d && pu[d],
+                    f = o(t, Du),
+                    g = u && Lu[u],
+                    y = !0 === d ? "flex-column" : d && $u[d],
                     h = b()(s || a, g, y);
-                return l().createElement(fi, e({
+                return l().createElement(ki, e({
                     className: h,
                     variant: i ? "pills" : null,
                     justify: c,
                     navbarScroll: p
                 }, m(["setProps"], f), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        fu.propTypes = {
+        Iu.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             pills: u().bool,
@@ -8565,425 +8806,435 @@
             navbar_scroll: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const mu = fu,
-            gu = i.forwardRef((({
+        const Au = Iu,
+            Fu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n,
                 ...r
             }, a) => {
-                e = j(e, "navbar-brand");
+                e = E(e, "navbar-brand");
                 const s = n || (r.href ? "a" : "span");
                 return (0, _.jsx)(s, {
                     ...r,
                     ref: a,
                     className: b()(t, e)
                 })
             }));
-        gu.displayName = "NavbarBrand";
-        const bu = gu,
-            yu = i.forwardRef((({
+        Fu.displayName = "NavbarBrand";
+        const Mu = Fu,
+            Bu = i.forwardRef((({
                 children: e,
                 bsPrefix: t,
                 ...n
             }, r) => {
-                t = j(t, "navbar-collapse");
-                const a = (0, i.useContext)(zo);
-                return (0, _.jsx)(ge, {
+                t = E(t, "navbar-collapse");
+                const a = (0, i.useContext)(ri);
+                return (0, _.jsx)(pe, {
                     in: !(!a || !a.expanded),
                     ...n,
                     children: (0, _.jsx)("div", {
                         ref: r,
                         className: t,
                         children: e
                     })
                 })
             }));
-        yu.displayName = "NavbarCollapse";
-        const hu = yu,
-            vu = i.forwardRef((({
+        Bu.displayName = "NavbarCollapse";
+        const zu = Bu,
+            Ku = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 children: n,
-                label: r,
+                label: r = "Toggle navigation",
                 as: a = "button",
                 onClick: s,
                 ...o
             }, l) => {
-                e = j(e, "navbar-toggler");
+                e = E(e, "navbar-toggler");
                 const {
                     onToggle: c,
                     expanded: u
-                } = (0, i.useContext)(zo) || {}, d = Xe((e => {
+                } = (0, i.useContext)(ri) || {}, d = Ye((e => {
                     s && s(e), c && c()
                 }));
                 return "button" === a && (o.type = "button"), (0, _.jsx)(a, {
                     ...o,
                     ref: l,
                     onClick: d,
                     "aria-label": r,
                     className: b()(t, e, !u && "collapsed"),
                     children: n || (0, _.jsx)("span", {
                         className: `${e}-icon`
                     })
                 })
             }));
-        vu.displayName = "NavbarToggle", vu.defaultProps = {
-            label: "Toggle navigation"
-        };
-        const _u = vu;
-        var xu = new WeakMap,
-            Ou = function(e, t) {
-                if (e && t) {
-                    var n = xu.get(t) || new Map;
-                    xu.set(t, n);
-                    var r = n.get(e);
-                    return r || ((r = t.matchMedia(e)).refCount = 0, n.set(r.media, r)), r
+        Ku.displayName = "NavbarToggle";
+        const Hu = Ku,
+            Uu = new WeakMap,
+            Wu = (e, t) => {
+                if (!e || !t) return;
+                const n = Uu.get(t) || new Map;
+                Uu.set(t, n);
+                let r = n.get(e);
+                return r || (r = t.matchMedia(e), r.refCount = 0, n.set(r.media, r)), r
+            };
+
+        function qu(e, t = ("undefined" == typeof window ? void 0 : window)) {
+            const n = Wu(e, t),
+                [r, a] = (0, i.useState)((() => !!n && n.matches));
+            return at((() => {
+                let n = Wu(e, t);
+                if (!n) return a(!1);
+                let r = Uu.get(t);
+                const s = () => {
+                    a(n.matches)
+                };
+                return n.refCount++, n.addListener(s), s(), () => {
+                    n.removeListener(s), n.refCount--, n.refCount <= 0 && (null == r || r.delete(n.media)), n = void 0
                 }
-            };
-
-        function wu(e, t) {
-            void 0 === t && (t = "undefined" == typeof window ? void 0 : window);
-            var n = Ou(e, t),
-                r = (0, i.useState)((function() {
-                    return !!n && n.matches
-                })),
-                a = r[0],
-                s = r[1];
-            return tt((function() {
-                var n = Ou(e, t);
-                if (!n) return s(!1);
-                var r = xu.get(t),
-                    a = function() {
-                        s(n.matches)
-                    };
-                return n.refCount++, n.addListener(a), a(),
-                    function() {
-                        n.removeListener(a), n.refCount--, n.refCount <= 0 && (null == r || r.delete(n.media)), n = void 0
-                    }
-            }), [e]), a
+            }), [e]), r
         }
-        const Nu = function(e) {
-                var t = Object.keys(e);
+        const Vu = function(e) {
+                const t = Object.keys(e);
 
                 function n(e, t) {
-                    return e === t ? t : e ? e + " and " + t : t
+                    return e === t ? t : e ? `${e} and ${t}` : t
                 }
                 return function(r, a, s) {
-                    var o, l;
-                    return "object" == typeof r ? (o = r, s = a, a = !0) : ((l = {})[r] = a = a || !0, o = l), wu((0, i.useMemo)((function() {
-                        return Object.entries(o).reduce((function(r, a) {
-                            var s, o = a[0],
-                                i = a[1];
-                            return "up" !== i && !0 !== i || (r = n(r, ("number" == typeof(s = e[o]) && (s += "px"), "(min-width: " + s + ")"))), "down" !== i && !0 !== i || (r = n(r, function(n) {
-                                var r = function(e) {
-                                        return t[Math.min(t.indexOf(e) + 1, t.length - 1)]
-                                    }(n),
-                                    a = e[r];
-                                return "(max-width: " + (a = "number" == typeof a ? a - .2 + "px" : "calc(" + a + " - 0.2px)") + ")"
-                            }(o))), r
-                        }), "")
-                    }), [JSON.stringify(o)]), s)
+                    let o;
+                    return "object" == typeof r ? (o = r, s = a, a = !0) : (a = a || !0, o = {
+                        [r]: a
+                    }), qu((0, i.useMemo)((() => Object.entries(o).reduce(((r, [a, s]) => ("up" !== s && !0 !== s || (r = n(r, function(t) {
+                        let n = e[t];
+                        return "number" == typeof n && (n = `${n}px`), `(min-width: ${n})`
+                    }(a))), "down" !== s && !0 !== s || (r = n(r, function(n) {
+                        const r = function(e) {
+                            return t[Math.min(t.indexOf(e) + 1, t.length - 1)]
+                        }(n);
+                        let a = e[r];
+                        return a = "number" == typeof a ? a - .2 + "px" : `calc(${a} - 0.2px)`, `(max-width: ${a})`
+                    }(a))), r)), "")), [JSON.stringify(o)]), s)
                 }
             }({
                 xs: 0,
                 sm: 576,
                 md: 768,
                 lg: 992,
                 xl: 1200,
                 xxl: 1400
             }),
-            Eu = ht("offcanvas-body"),
-            ju = {
-                [K]: "show",
-                [H]: "show"
+            Gu = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "offcanvas-body"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Gu.displayName = "OffcanvasBody";
+        const Yu = Gu,
+            Xu = {
+                [z]: "show",
+                [K]: "show"
             },
-            ku = i.forwardRef((({
+            Ju = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 children: n,
-                ...r
-            }, a) => (e = j(e, "offcanvas"), (0, _.jsx)(ce, {
-                ref: a,
-                addEndListener: re,
-                ...r,
+                in: r = !1,
+                mountOnEnter: a = !1,
+                unmountOnExit: s = !1,
+                appear: o = !1,
+                ...l
+            }, c) => (e = E(e, "offcanvas"), (0, _.jsx)(le, {
+                ref: c,
+                addEndListener: ne,
+                in: r,
+                mountOnEnter: a,
+                unmountOnExit: s,
+                appear: o,
+                ...l,
                 childRef: n.ref,
                 children: (r, a) => i.cloneElement(n, {
                     ...a,
-                    className: b()(t, n.props.className, (r === K || r === W) && `${e}-toggling`, ju[r])
+                    className: b()(t, n.props.className, (r === z || r === H) && `${e}-toggling`, Xu[r])
                 })
             }))));
-        ku.defaultProps = {
-            in: !1,
-            mountOnEnter: !1,
-            unmountOnExit: !1,
-            appear: !1
-        }, ku.displayName = "OffcanvasToggling";
-        const Pu = ku,
-            Cu = i.forwardRef((({
+        Ju.displayName = "OffcanvasToggling";
+        const Qu = Ju,
+            Zu = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                ...n
-            }, r) => (e = j(e, "offcanvas-header"), (0, _.jsx)(eu, {
-                ref: r,
-                ...n,
-                className: b()(t, e)
+                closeLabel: n = "Close",
+                closeButton: r = !1,
+                ...a
+            }, s) => (e = E(e, "offcanvas-header"), (0, _.jsx)(xu, {
+                ref: s,
+                ...a,
+                className: b()(t, e),
+                closeLabel: n,
+                closeButton: r
             }))));
-        Cu.displayName = "OffcanvasHeader", Cu.defaultProps = {
-            closeLabel: "Close",
-            closeButton: !1
-        };
-        const Tu = Cu,
-            Su = ht("offcanvas-title", {
-                Component: gt("h5")
-            });
+        Zu.displayName = "OffcanvasHeader";
+        const ed = Zu,
+            td = Xe("h5"),
+            nd = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = td,
+                ...r
+            }, a) => (t = E(t, "offcanvas-title"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        nd.displayName = "OffcanvasTitle";
+        const rd = nd;
 
-        function Ru(e) {
-            return (0, _.jsx)(Pu, {
+        function ad(e) {
+            return (0, _.jsx)(Qu, {
                 ...e
             })
         }
 
-        function Du(e) {
-            return (0, _.jsx)(dt, {
+        function sd(e) {
+            return (0, _.jsx)(bt, {
                 ...e
             })
         }
-        const Lu = i.forwardRef((({
+        const od = i.forwardRef((({
             bsPrefix: e,
             className: t,
             children: n,
             "aria-labelledby": r,
-            placement: a,
+            placement: a = "start",
             responsive: s,
-            show: o,
-            backdrop: l,
-            keyboard: c,
-            scroll: u,
+            show: o = !1,
+            backdrop: l = !0,
+            keyboard: c = !0,
+            scroll: u = !1,
             onEscapeKeyDown: d,
             onShow: p,
             onHide: f,
             container: m,
-            autoFocus: g,
-            enforceFocus: y,
-            restoreFocus: h,
+            autoFocus: g = !0,
+            enforceFocus: y = !0,
+            restoreFocus: h = !0,
             restoreFocusOptions: v,
             onEntered: x,
             onExit: O,
             onExiting: w,
             onEnter: N,
-            onEntering: E,
+            onEntering: j,
             onExited: k,
             backdropClassName: P,
             manager: C,
-            renderStaticNode: T,
+            renderStaticNode: T = !1,
             ...S
         }, R) => {
             const D = (0, i.useRef)();
-            e = j(e, "offcanvas");
+            e = E(e, "offcanvas");
             const {
                 onToggle: L
-            } = (0, i.useContext)(zo) || {}, [$, I] = (0, i.useState)(!1), A = Nu(s || "xs", "up");
+            } = (0, i.useContext)(ri) || {}, [$, I] = (0, i.useState)(!1), A = Vu(s || "xs", "up");
             (0, i.useEffect)((() => {
                 I(s ? o && !A : o)
             }), [o, s, A]);
-            const M = Xe((() => {
+            const F = Ye((() => {
                     null == L || L(), null == f || f()
                 })),
-                F = (0, i.useMemo)((() => ({
-                    onHide: M
-                })), [M]),
+                M = (0, i.useMemo)((() => ({
+                    onHide: F
+                })), [F]),
                 B = (0, i.useCallback)((t => (0, _.jsx)("div", {
                     ...t,
                     className: b()(`${e}-backdrop`, P)
                 })), [P, e]),
                 z = o => (0, _.jsx)("div", {
                     ...o,
                     ...S,
                     className: b()(t, s ? `${e}-${s}` : e, `${e}-${a}`),
                     "aria-labelledby": r,
                     children: n
                 });
             return (0, _.jsxs)(_.Fragment, {
-                children: [!$ && (s || T) && z({}), (0, _.jsx)(Tc.Provider, {
-                    value: F,
-                    children: (0, _.jsx)(_c, {
+                children: [!$ && (s || T) && z({}), (0, _.jsx)(Yc.Provider, {
+                    value: M,
+                    children: (0, _.jsx)(Mc, {
                         show: $,
                         ref: R,
                         backdrop: l,
                         container: m,
                         keyboard: c,
                         autoFocus: g,
                         enforceFocus: y && !u,
                         restoreFocus: h,
                         restoreFocusOptions: v,
                         onEscapeKeyDown: d,
                         onShow: p,
-                        onHide: M,
+                        onHide: F,
                         onEnter: (e, ...t) => {
                             e && (e.style.visibility = "visible"), null == N || N(e, ...t)
                         },
-                        onEntering: E,
+                        onEntering: j,
                         onEntered: x,
                         onExit: O,
                         onExiting: w,
                         onExited: (e, ...t) => {
                             e && (e.style.visibility = ""), null == k || k(...t)
                         },
-                        manager: C || (u ? (D.current || (D.current = new Cc({
+                        manager: C || (u ? (D.current || (D.current = new Gc({
                             handleContainerOverflow: !1
-                        })), D.current) : Pc()),
-                        transition: Ru,
-                        backdropTransition: Du,
+                        })), D.current) : Vc()),
+                        transition: ad,
+                        backdropTransition: sd,
                         renderBackdrop: B,
                         renderDialog: z
                     })
                 })]
             })
         }));
-        Lu.displayName = "Offcanvas", Lu.defaultProps = {
-            show: !1,
-            backdrop: !0,
-            keyboard: !0,
-            scroll: !1,
-            autoFocus: !0,
-            enforceFocus: !0,
-            restoreFocus: !0,
-            placement: "start",
-            renderStaticNode: !1
-        };
-        const $u = Object.assign(Lu, {
-                Body: Eu,
-                Header: Tu,
-                Title: Su
-            }),
-            Iu = i.forwardRef(((e, t) => {
-                const n = (0, i.useContext)(zo);
-                return (0, _.jsx)($u, {
+        od.displayName = "Offcanvas";
+        const id = Object.assign(od, {
+                Body: Yu,
+                Header: ed,
+                Title: rd
+            }),
+            ld = i.forwardRef(((e, t) => {
+                const n = (0, i.useContext)(ri);
+                return (0, _.jsx)(id, {
                     ref: t,
                     show: !(null == n || !n.expanded),
                     ...e,
                     renderStaticNode: !0
                 })
             }));
-        Iu.displayName = "NavbarOffcanvas";
-        const Au = Iu,
-            Mu = ht("navbar-text", {
-                Component: "span"
-            }),
-            Fu = i.forwardRef(((e, t) => {
+        ld.displayName = "NavbarOffcanvas";
+        const cd = ld,
+            ud = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "span",
+                ...r
+            }, a) => (t = E(t, "navbar-text"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        ud.displayName = "NavbarText";
+        const dd = ud,
+            pd = i.forwardRef(((e, t) => {
                 const {
                     bsPrefix: n,
-                    expand: r,
-                    variant: a,
+                    expand: r = !0,
+                    variant: a = "light",
                     bg: s,
                     fixed: o,
                     sticky: l,
                     className: c,
                     as: u = "nav",
                     expanded: d,
                     onToggle: p,
                     onSelect: f,
-                    collapseOnSelect: m,
+                    collapseOnSelect: m = !1,
                     ...g
                 } = v(e, {
                     expanded: "onToggle"
-                }), y = j(n, "navbar"), h = (0, i.useCallback)(((...e) => {
+                }), y = E(n, "navbar"), h = (0, i.useCallback)(((...e) => {
                     null == f || f(...e), m && d && (null == p || p(!1))
                 }), [f, m, d, p]);
                 void 0 === g.role && "nav" !== u && (g.role = "navigation");
                 let x = `${y}-expand`;
                 "string" == typeof r && (x = `${x}-${r}`);
                 const O = (0, i.useMemo)((() => ({
                     onToggle: () => null == p ? void 0 : p(!d),
                     bsPrefix: y,
                     expanded: !!d,
                     expand: r
                 })), [y, d, r, p]);
-                return (0, _.jsx)(zo.Provider, {
+                return (0, _.jsx)(ri.Provider, {
                     value: O,
-                    children: (0, _.jsx)(_o.Provider, {
+                    children: (0, _.jsx)(To.Provider, {
                         value: h,
                         children: (0, _.jsx)(u, {
                             ref: t,
                             ...g,
                             className: b()(c, y, r && x, a && `${y}-${a}`, s && `bg-${s}`, l && `sticky-${l}`, o && `fixed-${o}`)
                         })
                     })
                 })
             }));
-        Fu.defaultProps = {
-            expand: !0,
-            variant: "light",
-            collapseOnSelect: !1
-        }, Fu.displayName = "Navbar";
-        const Bu = Object.assign(Fu, {
-            Brand: bu,
-            Collapse: hu,
-            Offcanvas: Au,
-            Text: Mu,
-            Toggle: _u
+        pd.displayName = "Navbar";
+        const fd = Object.assign(pd, {
+            Brand: Mu,
+            Collapse: zu,
+            Offcanvas: cd,
+            Text: dd,
+            Toggle: Hu
         });
-        var zu = ["children", "color", "style", "loading_state", "className", "class_name", "light", "dark", "tag"];
+        var md = ["children", "color", "style", "loading_state", "className", "class_name", "light", "dark", "tag"];
 
-        function Ku(e, t) {
+        function gd(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Hu(e) {
+        function bd(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ku(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ku(Object(n)).forEach((function(t) {
+                t % 2 ? gd(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : gd(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Wu = function(t) {
+        var yd = function(t) {
             var n = t.children,
                 r = t.color,
                 a = t.style,
                 s = t.loading_state,
                 i = t.className,
                 c = t.class_name,
                 u = (t.light, t.dark),
                 d = t.tag,
-                p = o(t, zu),
-                f = Et.has(r);
-            return l().createElement(Bu, e({
+                p = o(t, md),
+                f = Ot.has(r);
+            return l().createElement(fd, e({
                 variant: u ? "dark" : "light",
                 as: d,
                 bg: f ? r : null,
-                style: Hu({
+                style: bd({
                     backgroundColor: !f && r
                 }, a),
                 className: c || i
             }, m(["setProps"], p), {
                 "data-dash-is-loading": s && s.is_loading || void 0
             }), n)
         };
-        Wu.defaultProps = {
+        yd.defaultProps = {
             color: "light",
             light: !0,
             expand: "md"
-        }, Wu.propTypes = {
+        }, yd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             light: u().bool,
@@ -8996,68 +9247,72 @@
             expand: u().oneOfType([u().bool, u().string]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Uu = Wu;
-        var qu = ["children", "loading_state", "className", "class_name"],
-            Vu = function(t) {
+        const hd = yd;
+        var vd = ["children", "loading_state", "className", "class_name", "href", "setProps"],
+            _d = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, qu);
-                return l().createElement(bu, e({
+                    i = t.href,
+                    c = t.setProps,
+                    u = o(t, vd),
+                    d = Fe(i, c);
+                return l().createElement(Mu, e({
                     className: s || a
-                }, m(["setProps"], i), {
-                    as: t.href ? Kt : "span",
+                }, u, {
+                    as: d ? Bt : "span",
+                    href: d,
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Vu.propTypes = {
+        _d.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             external_link: u().bool,
             href: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Gu = Vu;
-        var Yu = ["children", "loading_state", "className", "class_name"],
-            Xu = function(t) {
+        const xd = _d;
+        var Od = ["children", "loading_state", "className", "class_name"],
+            wd = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Yu);
-                return l().createElement(_u, e({
+                    i = o(t, Od);
+                return l().createElement(Hu, e({
                     onClick: function() {
                         t.setProps && t.setProps({
                             n_clicks: t.n_clicks + 1,
                             n_clicks_timestamp: Date.now()
                         })
                     },
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Xu.defaultProps = {
+        wd.defaultProps = {
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, Xu.propTypes = {
+        }, wd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             type: u().string,
@@ -9065,91 +9320,93 @@
             n_clicks_timestamp: u().number,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ju = Xu;
-        var Qu = ["children", "brand", "brand_href", "brand_style", "brand_external_link", "links_left", "fluid", "color", "dark", "light", "style", "loading_state", "className", "class_name"];
+        const Nd = wd;
+        var Ed = ["children", "brand", "brand_href", "brand_style", "brand_external_link", "links_left", "fluid", "color", "dark", "light", "style", "loading_state", "className", "class_name", "setProps"];
 
-        function Zu(e, t) {
+        function jd(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function ed(e) {
+        function kd(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Zu(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Zu(Object(n)).forEach((function(t) {
+                t % 2 ? jd(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : jd(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var td = function(t) {
+        var Pd = function(t) {
             var n = t.children,
                 r = t.brand,
                 a = t.brand_href,
                 s = t.brand_style,
                 c = t.brand_external_link,
                 u = t.links_left,
                 d = t.fluid,
                 p = t.color,
                 f = t.dark,
                 g = (t.light, t.style),
                 b = t.loading_state,
                 y = t.className,
                 h = t.class_name,
-                v = o(t, Qu),
-                _ = Et.has(p),
-                x = Le((0, i.useState)(!1), 2),
-                O = x[0],
-                w = x[1];
-            return l().createElement(Bu, e({
+                v = t.setProps,
+                _ = o(t, Ed),
+                x = Fe(a, v),
+                O = Ot.has(p),
+                w = Se((0, i.useState)(!1), 2),
+                N = w[0],
+                E = w[1];
+            return l().createElement(fd, e({
                 variant: f ? "dark" : "light",
-                bg: _ ? p : null,
-                color: _ ? p : null,
-                style: _ ? g : ed({
+                bg: O ? p : null,
+                color: O ? p : null,
+                style: O ? g : kd({
                     backgroundColor: p
                 }, g),
                 className: h || y
-            }, m(["setProps"], v), {
+            }, m(["setProps"], _), {
                 "data-dash-is-loading": b && b.is_loading || void 0
-            }), l().createElement(ba, {
+            }), l().createElement(Na, {
                 fluid: d
-            }, r && l().createElement(Gu, {
-                href: a,
+            }, r && l().createElement(xd, {
+                href: x,
                 style: s,
                 external_link: c
-            }, r), l().createElement(Ju, {
+            }, r), l().createElement(Nd, {
                 onClick: function() {
-                    return w(!O)
+                    return E(!N)
                 }
-            }), l().createElement(Bu.Collapse, {
-                in: O
-            }, l().createElement(mu, {
+            }), l().createElement(fd.Collapse, {
+                in: N
+            }, l().createElement(Au, {
                 className: u ? "me-auto" : "ms-auto"
             }, n))))
         };
-        td.defaultProps = {
+        Pd.defaultProps = {
             fluid: !1,
             color: "light",
             light: !0,
             expand: "md",
             links_left: !1
-        }, td.propTypes = {
+        }, Pd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             brand: u().node,
@@ -9166,90 +9423,91 @@
             expand: u().oneOfType([u().bool, u().string]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const nd = td;
-        var rd = ["children", "loading_state", "className", "class_name"],
-            ad = function(t) {
+        const Cd = Pd;
+        var Td = ["children", "loading_state", "className", "class_name"],
+            Sd = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, rd);
-                return l().createElement(ci, e({
+                    i = o(t, Td);
+                return l().createElement(wi, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        ad.propTypes = {
+        Sd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const sd = ad;
-        var od = n(14),
-            id = ["children", "disabled", "className", "class_name", "active", "loading_state", "setProps", "n_clicks", "href"],
-            ld = function(t) {
-                var n = Le((0, i.useState)(!1), 2),
+        const Rd = Sd;
+        var Dd = n(13),
+            Ld = ["children", "disabled", "className", "class_name", "active", "loading_state", "setProps", "n_clicks", "href"],
+            $d = function(t) {
+                var n = Se((0, i.useState)(!1), 2),
                     r = n[0],
                     a = n[1],
                     s = t.children,
                     c = t.disabled,
                     u = t.className,
                     d = t.class_name,
                     p = t.active,
                     f = t.loading_state,
                     g = t.setProps,
                     y = t.n_clicks,
                     h = t.href,
-                    v = o(t, id),
-                    _ = function(e) {
-                        a(!0 === p || "exact" === p && e === h || "partial" === p && e.startsWith(h))
+                    v = o(t, Ld),
+                    _ = Fe(h, g),
+                    x = function(e) {
+                        a(!0 === p || "exact" === p && e === _ || "partial" === p && e.startsWith(_))
                     };
                 (0, i.useEffect)((function() {
-                    _(window.location.pathname), "string" == typeof p && od.History.onChange((function() {
-                        _(window.location.pathname)
+                    x(window.location.pathname), "string" == typeof p && Dd.History.onChange((function() {
+                        x(window.location.pathname)
                     }))
                 }), [p]);
-                var x = b()(d || u, "nav-link", {
+                var O = b()(d || u, "nav-link", {
                     active: r,
                     disabled: c
                 });
-                return l().createElement(Kt, e({
-                    className: x,
+                return l().createElement(Bt, e({
+                    className: O,
                     disabled: c,
                     preOnClick: function() {
                         !c && g && g({
                             n_clicks: y + 1,
                             n_clicks_timestamp: Date.now()
                         })
                     },
-                    href: h
+                    href: _
                 }, m(["n_clicks_timestamp"], v), {
                     "data-dash-is-loading": f && f.is_loading || void 0
                 }), s)
             };
-        ld.defaultProps = {
+        $d.defaultProps = {
             active: !1,
             disabled: !1,
             n_clicks: 0,
             n_clicks_timestamp: -1
-        }, ld.propTypes = {
+        }, $d.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             href: u().string,
@@ -9261,17 +9519,17 @@
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             target: u().string
         };
-        const cd = ld;
-        var ud = ["is_open", "setProps", "children", "loading_state", "class_name", "className", "backdrop", "backdrop_class_name", "backdropClassName", "labelledby", "labelledBy", "scrollable", "autofocus", "autoFocus", "close_button", "title"],
-            dd = function(t) {
+        const Id = $d;
+        var Ad = ["is_open", "setProps", "children", "loading_state", "class_name", "className", "backdrop", "backdrop_class_name", "backdropClassName", "labelledby", "labelledBy", "scrollable", "autofocus", "autoFocus", "close_button", "title"],
+            Fd = function(t) {
                 var n = t.is_open,
                     r = t.setProps,
                     a = t.children,
                     s = t.loading_state,
                     i = t.class_name,
                     c = t.className,
                     u = t.backdrop,
@@ -9280,41 +9538,41 @@
                     f = t.labelledby,
                     m = t.labelledBy,
                     g = t.scrollable,
                     b = t.autofocus,
                     y = t.autoFocus,
                     h = t.close_button,
                     v = t.title,
-                    _ = o(t, ud),
+                    _ = o(t, Ad),
                     x = function() {
                         r && r({
                             is_open: !n
                         })
                     },
-                    O = v || h ? l().createElement($u.Header, {
+                    O = v || h ? l().createElement(id.Header, {
                         closeButton: h,
                         onHide: "static" === u && h ? x : null
-                    }, l().createElement($u.Title, null, v)) : null;
-                return l().createElement($u, e({
+                    }, l().createElement(id.Title, null, v)) : null;
+                return l().createElement(id, e({
                     autoFocus: b || y,
                     "aria-labelledby": f || m,
                     className: i || c,
                     backdropClassName: d || p,
                     scroll: g,
                     show: n,
                     onHide: "static" !== u ? x : null,
                     backdrop: u || "static" === u,
                     "data-dash-is-loading": s && s.is_loading || void 0
-                }, _), O, l().createElement($u.Body, null, a))
+                }, _), O, l().createElement(id.Body, null, a))
             };
-        dd.defaultProps = {
+        Fd.defaultProps = {
             close_button: !0,
             is_open: !1,
             backdrop: !0
-        }, dd.propTypes = {
+        }, Fd.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             labelledby: u().string,
             labelledBy: u().string,
@@ -9331,175 +9589,175 @@
             close_button: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const pd = dd,
-            fd = i.forwardRef((({
-                active: e,
-                disabled: t,
+        const Md = Fd,
+            Bd = i.forwardRef((({
+                active: e = !1,
+                disabled: t = !1,
                 className: n,
                 style: r,
-                activeLabel: a,
+                activeLabel: a = "(current)",
                 children: s,
-                ...o
-            }, i) => {
-                const l = e || t ? "span" : lt;
+                linkStyle: o,
+                linkClassName: i,
+                as: l = dt,
+                ...c
+            }, u) => {
+                const d = e || t ? "span" : l;
                 return (0, _.jsx)("li", {
-                    ref: i,
+                    ref: u,
                     style: r,
                     className: b()(n, "page-item", {
                         active: e,
                         disabled: t
                     }),
-                    children: (0, _.jsxs)(l, {
-                        className: "page-link",
-                        ...o,
+                    children: (0, _.jsxs)(d, {
+                        className: b()("page-link", i),
+                        style: o,
+                        ...c,
                         children: [s, e && a && (0, _.jsx)("span", {
                             className: "visually-hidden",
                             children: a
                         })]
                     })
                 })
             }));
-        fd.defaultProps = {
-            active: !1,
-            disabled: !1,
-            activeLabel: "(current)"
-        }, fd.displayName = "PageItem";
-        const md = fd;
+        Bd.displayName = "PageItem";
+        const zd = Bd;
 
-        function gd(e, t, n = e) {
+        function Kd(e, t, n = e) {
             const r = i.forwardRef((({
                 children: e,
                 ...r
-            }, a) => (0, _.jsxs)(fd, {
+            }, a) => (0, _.jsxs)(Bd, {
                 ...r,
                 ref: a,
                 children: [(0, _.jsx)("span", {
                     "aria-hidden": "true",
                     children: e || t
                 }), (0, _.jsx)("span", {
                     className: "visually-hidden",
                     children: n
                 })]
             })));
             return r.displayName = e, r
         }
-        const bd = gd("First", "«"),
-            yd = gd("Prev", "‹", "Previous"),
-            hd = gd("Ellipsis", "…", "More"),
-            vd = gd("Next", "›"),
-            _d = gd("Last", "»"),
-            xd = i.forwardRef((({
+        const Hd = Kd("First", "«"),
+            Ud = Kd("Prev", "‹", "Previous"),
+            Wd = Kd("Ellipsis", "…", "More"),
+            qd = Kd("Next", "›"),
+            Vd = Kd("Last", "»"),
+            Gd = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 size: n,
                 ...r
             }, a) => {
-                const s = j(e, "pagination");
+                const s = E(e, "pagination");
                 return (0, _.jsx)("ul", {
                     ref: a,
                     ...r,
                     className: b()(t, s, n && `${s}-${n}`)
                 })
             }));
-        xd.displayName = "Pagination";
-        const Od = Object.assign(xd, {
-            First: bd,
-            Prev: yd,
-            Ellipsis: hd,
-            Item: md,
-            Next: vd,
-            Last: _d
+        Gd.displayName = "Pagination";
+        const Yd = Object.assign(Gd, {
+            First: Hd,
+            Prev: Ud,
+            Ellipsis: Wd,
+            Item: zd,
+            Next: qd,
+            Last: Vd
         });
-        var wd = ["step", "active_page", "min_value", "fully_expanded", "previous_next", "first_last", "setProps", "class_name", "className", "loading_state"],
-            Nd = function(t) {
+        var Xd = ["step", "active_page", "min_value", "fully_expanded", "previous_next", "first_last", "setProps", "class_name", "className", "loading_state"],
+            Jd = function(t) {
                 var n = t.step,
                     r = t.active_page,
                     a = t.min_value,
                     s = t.fully_expanded,
                     i = t.previous_next,
                     c = t.first_last,
                     u = t.setProps,
                     d = t.class_name,
                     p = t.className,
                     f = t.loading_state,
-                    m = o(t, wd),
+                    m = o(t, Xd),
                     g = t.max_value;
                 (g - a) % n != 0 && (g = g + n - (g - a) % n);
                 var b = function(e) {
                         u && u({
                             active_page: e
                         })
                     },
                     y = function(e) {
-                        return l().createElement(Od.Item, {
+                        return l().createElement(Yd.Item, {
                             key: e,
                             active: e === r,
                             onClick: function() {
                                 return b(e)
                             }
                         }, e)
                     },
                     h = [];
-                if (c && h.push(l().createElement(Od.First, {
+                if (c && h.push(l().createElement(Yd.First, {
                         key: "first",
                         disabled: r === a,
                         onClick: function() {
                             return b(a)
                         }
-                    })), i && h.push(l().createElement(Od.Prev, {
+                    })), i && h.push(l().createElement(Yd.Prev, {
                         key: "previous",
                         disabled: r === a,
                         onClick: function() {
                             return b(r - n)
                         }
                     })), s || Math.floor((g - a) / n) + 1 <= 7)
                     for (var v = a; v <= g; v += n) h.push(y(v));
-                else h.push(y(a)), r <= a + 3 * n ? (h.push(y(a + n)), h.push(y(a + 2 * n)), h.push(y(a + 3 * n)), h.push(y(a + 4 * n)), h.push(l().createElement(Od.Ellipsis, {
+                else h.push(y(a)), r <= a + 3 * n ? (h.push(y(a + n)), h.push(y(a + 2 * n)), h.push(y(a + 3 * n)), h.push(y(a + 4 * n)), h.push(l().createElement(Yd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis"
-                }))) : r >= g - 3 * n ? (h.push(l().createElement(Od.Ellipsis, {
+                }))) : r >= g - 3 * n ? (h.push(l().createElement(Yd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis"
-                })), h.push(y(g - 4 * n)), h.push(y(g - 3 * n)), h.push(y(g - 2 * n)), h.push(y(g - n))) : (h.push(l().createElement(Od.Ellipsis, {
+                })), h.push(y(g - 4 * n)), h.push(y(g - 3 * n)), h.push(y(g - 2 * n)), h.push(y(g - n))) : (h.push(l().createElement(Yd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis-1"
-                })), h.push(y(r - n)), h.push(y(r)), h.push(y(r + n)), h.push(l().createElement(Od.Ellipsis, {
+                })), h.push(y(r - n)), h.push(y(r)), h.push(y(r + n)), h.push(l().createElement(Yd.Ellipsis, {
                     disabled: !0,
                     key: "ellipsis-2"
                 }))), h.push(y(g));
-                return i && h.push(l().createElement(Od.Next, {
+                return i && h.push(l().createElement(Yd.Next, {
                     key: "next",
                     disabled: r === g,
                     onClick: function() {
                         return b(r + n)
                     }
-                })), c && h.push(l().createElement(Od.Last, {
+                })), c && h.push(l().createElement(Yd.Last, {
                     key: "last",
                     disabled: r === g,
                     onClick: function() {
                         return b(g)
                     }
-                })), l().createElement(Od, e({
+                })), l().createElement(Yd, e({
                     className: d || p,
                     "data-dash-is-loading": f && f.is_loading || void 0
                 }, m), h)
             };
-        Nd.defaultProps = {
+        Jd.defaultProps = {
             min_value: 1,
             step: 1,
             active_page: 1,
             fully_expanded: !0,
             previous_next: !1,
             first_last: !1
-        }, Nd.propTypes = {
+        }, Jd.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             size: u().oneOf(["sm", "lg"]),
             min_value: u().number,
             max_value: u().number.isRequired,
@@ -9510,117 +9768,117 @@
             first_last: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Ed = Nd;
+        const Qd = Jd;
 
-        function jd({
+        function Zd({
             animation: e,
             bg: t,
             bsPrefix: n,
             size: r,
             ...a
         }) {
-            n = j(n, "placeholder");
+            n = E(n, "placeholder");
             const [{
                 className: s,
                 ...o
-            }] = ra(a);
+            }] = da(a);
             return {
                 ...o,
                 className: b()(s, e ? `${n}-${e}` : n, r && `${n}-${r}`, t && `bg-${t}`)
             }
         }
-        const kd = i.forwardRef(((e, t) => {
-            const n = jd(e);
+        const ep = i.forwardRef(((e, t) => {
+            const n = Zd(e);
             return (0, _.jsx)(nn, {
                 ...n,
                 ref: t,
                 disabled: !0,
                 tabIndex: -1
             })
         }));
-        kd.displayName = "PlaceholderButton";
-        const Pd = kd,
-            Cd = i.forwardRef((({
+        ep.displayName = "PlaceholderButton";
+        const tp = ep,
+            np = i.forwardRef((({
                 as: e = "span",
                 ...t
             }, n) => {
-                const r = jd(t);
+                const r = Zd(t);
                 return (0, _.jsx)(e, {
                     ...r,
                     ref: n
                 })
             }));
-        Cd.displayName = "Placeholder";
-        const Td = Object.assign(Cd, {
-            Button: Pd
+        np.displayName = "Placeholder";
+        const rp = Object.assign(np, {
+            Button: tp
         });
-        var Sd = ["children", "loading_state", "className", "class_name", "color", "button", "style", "delay_hide", "delay_show", "show_initially", "animation"];
+        var ap = ["children", "loading_state", "className", "class_name", "color", "button", "style", "delay_hide", "delay_show", "show_initially", "animation"];
 
-        function Rd(e, t) {
+        function sp(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
-        var Dd = function(t) {
+        var op = function(t) {
             var n = t.children,
                 r = t.loading_state,
                 a = t.className,
                 s = t.class_name,
                 c = t.color,
                 u = t.button,
                 d = t.style,
                 p = t.delay_hide,
                 f = t.delay_show,
                 g = t.show_initially,
                 y = t.animation,
-                h = o(t, Sd),
-                v = Le((0, i.useState)(g), 2),
+                h = o(t, ap),
+                v = Se((0, i.useState)(g), 2),
                 _ = v[0],
                 x = v[1],
                 O = (0, i.useRef)(),
                 w = (0, i.useRef)();
             (0, i.useEffect)((function() {
                 r && (r.is_loading ? (O.current && (O.current = clearTimeout(O.current)), _ || w.current || (w.current = setTimeout((function() {
                     x(!0), w.current = null
                 }), f))) : (w.current && (w.current = clearTimeout(w.current)), _ && !O.current && (O.current = setTimeout((function() {
                     x(!1), O.current = null
                 }), p))))
             }), [p, f, r]);
             var N = b()(s || a, y && "placeholder"),
                 E = function(t) {
                     var n = t.finalStyle;
-                    return u ? l().createElement(Td.Button, e({
+                    return u ? l().createElement(rp.Button, e({
                         variant: c,
                         className: N,
                         style: n,
                         animation: y
-                    }, m(["setProps"], h))) : l().createElement(Td, e({
+                    }, m(["setProps"], h))) : l().createElement(rp, e({
                         bg: c,
                         className: N,
                         style: n,
                         animation: y
                     }, m(["setProps"], h)))
                 };
             if (n) {
                 var j = function(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? Rd(Object(n), !0).forEach((function(t) {
-                            Ge(e, t, n[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Rd(Object(n)).forEach((function(t) {
+                        t % 2 ? sp(Object(n), !0).forEach((function(t) {
+                            Ve(e, t, n[t])
+                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : sp(Object(n)).forEach((function(t) {
                             Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                         }))
                     }
                     return e
                 }({
                     display: "block",
                     margin: "1rem auto"
@@ -9645,20 +9903,20 @@
                     finalStyle: j
                 })))
             }
             return l().createElement(E, {
                 finalStyle: d
             })
         };
-        Dd._dashprivate_isLoadingComponent = !0, Dd.defaultProps = {
+        op._dashprivate_isLoadingComponent = !0, op.defaultProps = {
             delay_hide: 0,
             delay_show: 0,
             show_initially: !0,
             button: !1
-        }, Dd.propTypes = {
+        }, op.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             loading_state: u().shape({
@@ -9676,85 +9934,96 @@
             xs: u().number,
             sm: u().number,
             md: u().number,
             lg: u().number,
             xl: u().number,
             xxl: u().number
         };
-        const Ld = Dd,
-            $d = ht("popover-body");
+        const ip = op,
+            lp = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "popover-body"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        lp.displayName = "PopoverBody";
+        const cp = lp;
 
-        function Id(e, t, n, r, a, s, o) {
+        function up(e, t, n, r, a, s, o) {
             try {
                 var i = e[s](o),
                     l = i.value
             } catch (e) {
                 return void n(e)
             }
             i.done ? t(l) : Promise.resolve(l).then(r, a)
         }
 
-        function Ad(e) {
+        function dp(e) {
             return function() {
                 var t = this,
                     n = arguments;
                 return new Promise((function(r, a) {
                     var s = e.apply(t, n);
 
                     function o(e) {
-                        Id(s, r, a, o, i, "next", e)
+                        up(s, r, a, o, i, "next", e)
                     }
 
                     function i(e) {
-                        Id(s, r, a, o, i, "throw", e)
+                        up(s, r, a, o, i, "throw", e)
                     }
                     o(void 0)
                 }))
             }
         }
-        var Md = n(15),
-            Fd = n.n(Md);
-        const Bd = () => {},
-            zd = i.forwardRef(((e, t) => {
+        var pp = n(14),
+            fp = n.n(pp);
+        const mp = () => {},
+            gp = i.forwardRef(((e, t) => {
                 const {
                     flip: n,
                     offset: r,
                     placement: a,
                     containerPadding: s,
                     popperConfig: o = {},
                     transition: l,
                     runTransition: c
-                } = e, [u, d] = Je(), [p, f] = Je(), m = ie(d, t), g = pc(e.container), b = pc(e.target), [y, h] = (0, i.useState)(!e.show), v = Vs(b, u, no({
+                } = e, [u, d] = et(), [p, f] = et(), m = oe(d, t), g = Pc(e.container), b = Pc(e.target), [y, h] = (0, i.useState)(!e.show), v = Zs(b, u, lo({
                     placement: a,
                     enableEvents: !!e.show,
                     containerPadding: s || 5,
                     flip: n,
                     offset: r,
                     arrowElement: p,
                     popperConfig: o
                 }));
                 e.show && y && h(!1);
                 const _ = e.show || !y;
                 if (function(e, t, {
                         disabled: n,
                         clickTrigger: r
                     } = {}) {
-                        const a = t || Bd;
-                        eo(e, a, {
+                        const a = t || mp;
+                        oo(e, a, {
                             disabled: n,
                             clickTrigger: r
                         });
-                        const s = Xe((e => {
-                            bc(e) && a(e)
+                        const s = Ye((e => {
+                            $c(e) && a(e)
                         }));
                         (0, i.useEffect)((() => {
                             if (n || null == e) return;
-                            const t = T(Qs(e));
+                            const t = C(ao(e));
                             let r = (t.defaultView || window).event;
-                            const a = ee(t, "keyup", (e => {
+                            const a = Z(t, "keyup", (e => {
                                 e !== r ? s(e) : r = void 0
                             }));
                             return () => {
                                 a()
                             }
                         }), [e, n, s])
                     }(u, e.onHide, {
@@ -9776,418 +10045,519 @@
                     placement: a,
                     show: !!e.show,
                     arrowProps: Object.assign({}, v.attributes.arrow, {
                         style: v.styles.arrow,
                         ref: f
                     })
                 });
-                return j = gc(l, c, {
+                return j = Lc(l, c, {
                     in: !!e.show,
                     appear: !0,
                     mountOnEnter: !0,
                     unmountOnExit: !0,
                     children: j,
                     onExit: x,
                     onExiting: O,
                     onExited: (...t) => {
                         h(!0), e.onExited && e.onExited(...t)
                     },
                     onEnter: w,
                     onEntering: N,
                     onEntered: E
-                }), g ? M().createPortal(j, g) : null
+                }), g ? A().createPortal(j, g) : null
             }));
-        zd.displayName = "Overlay";
-        const Kd = zd,
-            Hd = ht("popover-header");
-        class Wd extends i.Component {}
+        gp.displayName = "Overlay";
+        const bp = gp,
+            yp = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "popover-header"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        yp.displayName = "PopoverHeader";
+        const hp = yp;
+
+        function vp(e, t) {
+            let n = e;
+            return "left" === e ? n = t ? "end" : "start" : "right" === e && (n = t ? "start" : "end"), n
+        }
 
-        function Ud(e = "absolute") {
+        function _p(e = "absolute") {
             return {
                 position: e,
                 top: "0",
                 left: "0",
                 opacity: "0",
                 pointerEvents: "none"
             }
         }
-        const qd = i.forwardRef((({
-            bsPrefix: e,
-            placement: t,
-            className: n,
-            style: r,
-            children: a,
-            body: s,
-            arrowProps: o,
-            hasDoneInitialMeasure: i,
-            popper: l,
-            show: c,
-            ...u
-        }, d) => {
-            const p = j(e, "popover"),
-                f = C(),
-                [m] = (null == t ? void 0 : t.split("-")) || [],
-                g = function(e, t) {
-                    let n = e;
-                    return "left" === e ? n = t ? "end" : "start" : "right" === e && (n = t ? "start" : "end"), n
-                }(m, f);
-            let y = r;
-            return c && !i && (y = {
-                ...r,
-                ...Ud(null == l ? void 0 : l.strategy)
-            }), (0, _.jsxs)("div", {
-                ref: d,
-                role: "tooltip",
-                style: y,
-                "x-placement": m,
-                className: b()(n, p, m && `bs-popover-${g}`),
-                ...u,
-                children: [(0, _.jsx)("div", {
-                    className: "popover-arrow",
-                    ...o
-                }), s ? (0, _.jsx)($d, {
-                    children: a
-                }) : a]
-            })
-        }));
-        qd.defaultProps = {
-            placement: "right"
-        };
-        const Vd = Object.assign(qd, {
-                Header: Hd,
-                Body: $d,
+        i.Component;
+        const xp = i.forwardRef((({
+                bsPrefix: e,
+                placement: t = "right",
+                className: n,
+                style: r,
+                children: a,
+                body: s,
+                arrowProps: o,
+                hasDoneInitialMeasure: i,
+                popper: l,
+                show: c,
+                ...u
+            }, d) => {
+                const p = E(e, "popover"),
+                    f = P(),
+                    [m] = (null == t ? void 0 : t.split("-")) || [],
+                    g = vp(m, f);
+                let y = r;
+                return c && !i && (y = {
+                    ...r,
+                    ..._p(null == l ? void 0 : l.strategy)
+                }), (0, _.jsxs)("div", {
+                    ref: d,
+                    role: "tooltip",
+                    style: y,
+                    "x-placement": m,
+                    className: b()(n, p, m && `bs-popover-${g}`),
+                    ...u,
+                    children: [(0, _.jsx)("div", {
+                        className: "popover-arrow",
+                        ...o
+                    }), s ? (0, _.jsx)(cp, {
+                        children: a
+                    }) : a]
+                })
+            })),
+            Op = Object.assign(xp, {
+                Header: hp,
+                Body: cp,
                 POPPER_OFFSET: [0, 8]
             }),
-            Gd = {
-                transition: dt,
-                rootClose: !1,
-                show: !1,
-                placement: "top"
-            },
-            Yd = i.forwardRef((({
+            wp = i.forwardRef((({
+                bsPrefix: e,
+                placement: t = "right",
+                className: n,
+                style: r,
+                children: a,
+                arrowProps: s,
+                hasDoneInitialMeasure: o,
+                popper: i,
+                show: l,
+                ...c
+            }, u) => {
+                e = E(e, "tooltip");
+                const d = P(),
+                    [p] = (null == t ? void 0 : t.split("-")) || [],
+                    f = vp(p, d);
+                let m = r;
+                return l && !o && (m = {
+                    ...r,
+                    ..._p(null == i ? void 0 : i.strategy)
+                }), (0, _.jsxs)("div", {
+                    ref: u,
+                    style: m,
+                    role: "tooltip",
+                    "x-placement": p,
+                    className: b()(n, e, `bs-tooltip-${f}`),
+                    ...c,
+                    children: [(0, _.jsx)("div", {
+                        className: "tooltip-arrow",
+                        ...s
+                    }), (0, _.jsx)("div", {
+                        className: `${e}-inner`,
+                        children: a
+                    })]
+                })
+            }));
+        wp.displayName = "Tooltip";
+        const Np = Object.assign(wp, {
+                TOOLTIP_OFFSET: [0, 6]
+            }),
+            Ep = i.forwardRef((({
                 children: e,
-                transition: t,
+                transition: t = bt,
                 popperConfig: n = {},
-                ...r
-            }, a) => {
-                const s = (0, i.useRef)({}),
-                    [o, l] = (0, i.useState)(null),
-                    [c, u] = function(e) {
+                rootClose: r = !1,
+                placement: a = "top",
+                show: s = !1,
+                ...o
+            }, l) => {
+                const c = (0, i.useRef)({}),
+                    [u, d] = (0, i.useState)(null),
+                    [p, f] = function(e) {
                         const t = (0, i.useRef)(null),
-                            n = j(void 0, "popover"),
-                            r = (0, i.useMemo)((() => ({
+                            n = E(void 0, "popover"),
+                            r = E(void 0, "tooltip"),
+                            a = (0, i.useMemo)((() => ({
                                 name: "offset",
                                 options: {
-                                    offset: () => t.current && xc(t.current, n) ? e || Vd.POPPER_OFFSET : e || [0, 0]
+                                    offset: () => {
+                                        if (e) return e;
+                                        if (t.current) {
+                                            if (Bc(t.current, n)) return Op.POPPER_OFFSET;
+                                            if (Bc(t.current, r)) return Np.TOOLTIP_OFFSET
+                                        }
+                                        return [0, 0]
+                                    }
                                 }
-                            })), [e, n]);
-                        return [t, [r]]
-                    }(r.offset),
-                    d = ie(a, c),
-                    p = !0 === t ? dt : t || void 0,
-                    f = Xe((e => {
-                        l(e), null == n || null == n.onFirstUpdate || n.onFirstUpdate(e)
+                            })), [e, n, r]);
+                        return [t, [a]]
+                    }(o.offset),
+                    m = oe(l, p),
+                    g = !0 === t ? bt : t || void 0,
+                    y = Ye((e => {
+                        d(e), null == n || null == n.onFirstUpdate || n.onFirstUpdate(e)
                     }));
-                return tt((() => {
-                    o && (null == s.current.scheduleUpdate || s.current.scheduleUpdate())
-                }), [o]), (0, i.useEffect)((() => {
-                    r.show || l(null)
-                }), [r.show]), (0, _.jsx)(Kd, {
-                    ...r,
-                    ref: d,
+                return at((() => {
+                    u && o.target && (null == c.current.scheduleUpdate || c.current.scheduleUpdate())
+                }), [u, o.target]), (0, i.useEffect)((() => {
+                    s || d(null)
+                }), [s]), (0, _.jsx)(bp, {
+                    ...o,
+                    ref: m,
                     popperConfig: {
                         ...n,
-                        modifiers: u.concat(n.modifiers || []),
-                        onFirstUpdate: f
+                        modifiers: f.concat(n.modifiers || []),
+                        onFirstUpdate: y
                     },
-                    transition: p,
+                    transition: g,
+                    rootClose: r,
+                    placement: a,
+                    show: s,
                     children: (r, {
                         arrowProps: a,
-                        popper: l,
-                        show: c
+                        popper: s,
+                        show: o
                     }) => {
-                        var u, d;
+                        var l, d;
                         ! function(e, t) {
                             const {
                                 ref: n
                             } = e, {
                                 ref: r
                             } = t;
-                            e.ref = n.__wrapped || (n.__wrapped = e => n(le(e))), t.ref = r.__wrapped || (r.__wrapped = e => r(le(e)))
+                            e.ref = n.__wrapped || (n.__wrapped = e => n(ie(e))), t.ref = r.__wrapped || (r.__wrapped = e => r(ie(e)))
                         }(r, a);
-                        const p = null == l ? void 0 : l.placement,
-                            f = Object.assign(s.current, {
-                                state: null == l ? void 0 : l.state,
-                                scheduleUpdate: null == l ? void 0 : l.update,
+                        const p = null == s ? void 0 : s.placement,
+                            f = Object.assign(c.current, {
+                                state: null == s ? void 0 : s.state,
+                                scheduleUpdate: null == s ? void 0 : s.update,
                                 placement: p,
-                                outOfBoundaries: (null == l || null == (u = l.state) || null == (d = u.modifiersData.hide) ? void 0 : d.isReferenceHidden) || !1,
+                                outOfBoundaries: (null == s || null == (l = s.state) || null == (d = l.modifiersData.hide) ? void 0 : d.isReferenceHidden) || !1,
                                 strategy: n.strategy
                             }),
-                            m = !!o;
+                            m = !!u;
                         return "function" == typeof e ? e({
                             ...r,
                             placement: p,
-                            show: c,
-                            ...!t && c && {
+                            show: o,
+                            ...!t && o && {
                                 className: "show"
                             },
                             popper: f,
                             arrowProps: a,
                             hasDoneInitialMeasure: m
                         }) : i.cloneElement(e, {
                             ...r,
                             placement: p,
                             arrowProps: a,
                             popper: f,
                             hasDoneInitialMeasure: m,
-                            className: b()(e.props.className, !t && c && "show"),
+                            className: b()(e.props.className, !t && o && "show"),
                             style: {
                                 ...e.props.style,
                                 ...r.style
                             }
                         })
                     }
                 })
             }));
-        Yd.displayName = "Overlay", Yd.defaultProps = Gd;
-        const Xd = Yd;
-        var Jd = ["children", "target", "delay", "trigger", "defaultShow", "setProps", "autohide"],
-            Qd = (0, i.createContext)({});
-        const Zd = function(t) {
-            var n, r, a, s, c, u = t.children,
-                d = t.target,
-                p = t.delay,
-                f = t.trigger,
-                m = t.defaultShow,
-                g = t.setProps,
-                b = t.autohide,
-                y = o(t, Jd),
-                h = (!1, n = Le((0, i.useState)(false), 2), r = n[0], a = n[1], s = (0, i.useRef)(r), (0, i.useEffect)((function() {
+        Ep.displayName = "Overlay";
+        const jp = Ep;
+        var kp = ["children", "target", "delay", "trigger", "defaultShow", "setProps", "autohide"],
+            Pp = (0, i.createContext)({});
+        const Cp = function(t) {
+            var n, r, a, s, c = t.children,
+                u = t.target,
+                d = t.delay,
+                p = t.trigger,
+                f = t.defaultShow,
+                m = t.setProps,
+                g = t.autohide,
+                b = o(t, kp),
+                y = (!1, n = Se((0, i.useState)(false), 2), r = n[0], a = n[1], s = (0, i.useRef)(r), (0, i.useEffect)((function() {
                     s.current = r
                 }), [r]), [r, a, s]),
-                v = Le(h, 3),
-                _ = v[0],
-                x = v[1],
-                O = v[2],
+                h = Se(y, 3),
+                v = h[0],
+                _ = h[1],
+                x = h[2],
+                O = (0, i.useRef)(null),
                 w = (0, i.useRef)(null),
                 N = (0, i.useRef)(null),
-                E = (0, i.useRef)(null),
-                j = "string" == typeof f ? f.split(" ") : [],
-                k = "object" !== De(c = d) ? c : "{" + Object.keys(c).sort().map((function(e) {
-                    return JSON.stringify(e) + ":" + ((t = c[e]) && t.wild || JSON.stringify(t));
+                E = (0, i.useRef)(!1);
+            (0, i.useEffect)((function() {
+                return E.current = !0,
+                    function() {
+                        E.current = !1
+                    }
+            }));
+            var j, k = "string" == typeof p ? p.split(" ") : [],
+                P = "object" !== Te(j = u) ? j : "{" + Object.keys(j).sort().map((function(e) {
+                    return JSON.stringify(e) + ":" + ((t = j[e]) && t.wild || JSON.stringify(t));
                     var t
                 })).join(",") + "}",
-                P = Le((0, i.useState)(!1), 2),
-                C = P[0],
-                T = P[1],
-                S = function() {
-                    O.current && (N.current = clearTimeout(N.current), x(!1), g && g({
+                C = Se((0, i.useState)(!1), 2),
+                T = C[0],
+                S = C[1],
+                R = function() {
+                    x.current && (w.current = clearTimeout(w.current), _(!1), m && E.current && m({
                         is_open: !1
                     }))
                 },
-                R = function() {
-                    !O.current && E.current ? (E.current = clearTimeout(E.current), S()) : O.current && (clearTimeout(N.current), N.current = setTimeout(S, p.hide))
-                },
                 D = function() {
-                    O.current || (E.current = clearTimeout(E.current), x(!0), g && g({
+                    !x.current && N.current ? (N.current = clearTimeout(N.current), R()) : x.current && (clearTimeout(w.current), w.current = setTimeout(R, d.hide))
+                },
+                L = function() {
+                    x.current || (N.current = clearTimeout(N.current), _(!0), m && E && m({
                         is_open: !0
                     }))
                 },
-                L = function() {
-                    O.current && N.current ? (N.current = clearTimeout(N.current), D()) : O.current || (clearTimeout(E.current), E.current = setTimeout(D, p.show))
+                $ = function() {
+                    x.current && w.current ? (w.current = clearTimeout(w.current), L()) : x.current || (clearTimeout(N.current), N.current = setTimeout(L, d.show))
                 },
-                $ = function(e) {
+                I = function(e) {
                     var t, n;
-                    t = e.target, (n = w.current) && (t === n || n.contains(t)) && (N.current && (N.current = clearTimeout(N.current)), O.current ? R() : L())
+                    t = e.target, (n = O.current) && (t === n || n.contains(t)) && (w.current && (w.current = clearTimeout(w.current)), x.current ? D() : $())
                 };
             (0, i.useEffect)((function() {
                 setTimeout((function() {
-                    return x(m)
+                    return _(f)
                 }), 50)
-            }), [m]), (0, i.useEffect)((function() {
-                j.indexOf("legacy") > -1 ? T(!0) : T(!1)
-            }), [j]);
-            var I = function(e) {
+            }), [f]), (0, i.useEffect)((function() {
+                k.indexOf("legacy") > -1 ? S(!0) : S(!1)
+            }), [k]);
+            var A = function(e) {
                     return new Promise((function(t) {
                         return setTimeout(t, e)
                     }))
                 },
-                A = function() {
-                    var e = Ad(Fd().mark((function e(t) {
+                F = function() {
+                    var e = dp(fp().mark((function e(t) {
                         var n, r, a = arguments;
-                        return Fd().wrap((function(e) {
+                        return fp().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
                                     if (n = a.length > 1 && void 0 !== a[1] ? a[1] : 0, !(null === (r = document.getElementById(t)) && n < 4)) {
                                         e.next = 6;
                                         break
                                     }
-                                    return e.next = 5, I(100 * Math.pow(2, n));
+                                    return e.next = 5, A(100 * Math.pow(2, n));
                                 case 5:
-                                    return e.abrupt("return", A(t, n + 1));
+                                    return e.abrupt("return", F(t, n + 1));
                                 case 6:
                                     return e.abrupt("return", r);
                                 case 7:
                                 case "end":
                                     return e.stop()
                             }
                         }), e)
                     })));
                     return function(t) {
                         return e.apply(this, arguments)
                     }
                 }();
             return (0, i.useEffect)((function() {
                 var e = function() {
-                    var e = Ad(Fd().mark((function e() {
-                        return Fd().wrap((function(e) {
+                    var e = dp(fp().mark((function e() {
+                        return fp().wrap((function(e) {
                             for (;;) switch (e.prev = e.next) {
                                 case 0:
-                                    return e.next = 2, A(k);
+                                    return e.next = 2, F(P);
                                 case 2:
-                                    w.current = e.sent, (t = w.current) && (j.indexOf("hover") > -1 && (t.addEventListener("mouseover", L, !0), t.addEventListener("mouseout", R, !0)), j.indexOf("focus") > -1 && (t.addEventListener("focusin", D, !0), t.addEventListener("focusout", S, !0)), (j.indexOf("click") > -1 || j.indexOf("legacy") > -1) && document.addEventListener("click", $, !0), t.addEventListener("keydown", (function(e) {
-                                        "Escape" === e.key && S()
+                                    O.current = e.sent, (t = O.current) && (k.indexOf("hover") > -1 && (t.addEventListener("mouseover", $, !0), t.addEventListener("mouseout", D, !0)), k.indexOf("focus") > -1 && (t.addEventListener("focusin", $, !0), t.addEventListener("focusout", D, !0)), (k.indexOf("click") > -1 || k.indexOf("legacy") > -1) && document.addEventListener("click", I, !0), t.addEventListener("keydown", (function(e) {
+                                        "Escape" === e.key && R()
                                     })));
                                 case 4:
                                 case "end":
                                     return e.stop()
                             }
                             var t
                         }), e)
                     })));
                     return function() {
                         return e.apply(this, arguments)
                     }
                 }();
                 e()
-            }), [k]), l().createElement(Qd.Provider, {
+            }), [P]), l().createElement(Pp.Provider, {
                 value: {
                     handleMouseOverTooltipContent: function(e) {
-                        j.indexOf("hover") > -1 && !b && (N.current && (N.current = clearTimeout(N.current)), D())
+                        k.indexOf("hover") > -1 && !g && (w.current && (w.current = clearTimeout(w.current)), L())
                     },
                     handleMouseLeaveTooltipContent: function(e) {
-                        j.indexOf("hover") > -1 && !b && (E.current && (E.current = clearTimeout(E.current)), e.persist(), R())
+                        k.indexOf("hover") > -1 && !g && (N.current && (N.current = clearTimeout(N.current)), e.persist(), D())
                     }
                 }
-            }, l().createElement(Xd, e({
-                show: _,
-                rootClose: C,
+            }, l().createElement(jp, e({
+                show: v,
+                rootClose: T,
                 onHide: function() {
-                    x(!1), g && g({
+                    _(!1), m && E.current && m({
                         is_open: !1
                     })
                 },
-                target: w.current
-            }, y), u))
+                target: O.current
+            }, b), c))
         };
-        var ep = ["placement", "className", "style", "children", "body", "arrowProps", "popper", "show", "hideArrow"],
-            tp = ["bsPrefix", "placement", "className", "style", "children", "arrowProps", "popper", "show"],
-            np = function(e) {
+        var Tp = ["placement", "className", "style", "children", "body", "arrowProps", "popper", "show", "hideArrow"],
+            Sp = ["bsPrefix", "placement", "className", "style", "children", "arrowProps", "popper", "show", "hasDoneInitialMeasure"];
+
+        function Rp(e, t) {
+            var n = Object.keys(e);
+            if (Object.getOwnPropertySymbols) {
+                var r = Object.getOwnPropertySymbols(e);
+                t && (r = r.filter((function(t) {
+                    return Object.getOwnPropertyDescriptor(e, t).enumerable
+                }))), n.push.apply(n, r)
+            }
+            return n
+        }
+
+        function Dp(e) {
+            for (var t = 1; t < arguments.length; t++) {
+                var n = null != arguments[t] ? arguments[t] : {};
+                t % 2 ? Rp(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Rp(Object(n)).forEach((function(t) {
+                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+                }))
+            }
+            return e
+        }
+        var Lp = function(e) {
                 var t = e;
                 return "left" === e ? t = "start" : "right" === e && (t = "end"), t
             },
-            rp = l().forwardRef((function(t, n) {
+            $p = l().forwardRef((function(t, n) {
                 var r = t.placement,
                     a = t.className,
                     s = t.style,
                     c = t.children,
                     u = t.body,
                     d = t.arrowProps,
                     p = (t.popper, t.show, t.hideArrow),
-                    f = o(t, ep),
-                    m = Le((null == r ? void 0 : r.split("-")) || [], 1)[0],
-                    g = np(m),
-                    y = (0, i.useContext)(Qd),
+                    f = o(t, Tp),
+                    m = Se((null == r ? void 0 : r.split("-")) || [], 1)[0],
+                    g = Lp(m),
+                    y = (0, i.useContext)(Pp),
                     h = y.handleMouseOverTooltipContent,
                     v = y.handleMouseLeaveTooltipContent;
                 return l().createElement("div", e({
                     ref: n,
                     role: "tooltip",
                     style: s,
                     "x-placement": m,
                     className: b()(a, "popover", m && "bs-popover-".concat(g)),
                     onMouseOver: h,
                     onMouseLeave: v
                 }, f), !p && l().createElement("div", e({
                     className: "popover-arrow"
-                }, d)), u ? l().createElement($d, null, c) : c)
+                }, d)), u ? l().createElement(cp, null, c) : c)
             })),
-            ap = l().forwardRef((function(t, n) {
+            Ip = l().forwardRef((function(t, n) {
                 t.bsPrefix;
                 var r = t.placement,
                     a = t.className,
                     s = t.style,
                     c = t.children,
                     u = t.arrowProps,
-                    d = (t.popper, t.show, o(t, tp)),
-                    p = Le((null == r ? void 0 : r.split("-")) || [], 1)[0],
-                    f = np(p),
-                    m = (0, i.useContext)(Qd),
-                    g = m.handleMouseOverTooltipContent,
-                    y = m.handleMouseLeaveTooltipContent;
+                    d = t.popper,
+                    p = t.show,
+                    f = t.hasDoneInitialMeasure,
+                    m = o(t, Sp),
+                    g = Se((null == r ? void 0 : r.split("-")) || [], 1)[0],
+                    y = Lp(g),
+                    h = s;
+                p && !f && (Dp(Dp({}, s), {}, {
+                    position: null == d ? void 0 : d.strategy,
+                    top: "0",
+                    left: "0",
+                    opacity: "0",
+                    pointerEvents: "none"
+                }), function(e) {
+                    throw new TypeError('"computedStyle" is read-only')
+                }());
+                var v = (0, i.useContext)(Pp),
+                    _ = v.handleMouseOverTooltipContent,
+                    x = v.handleMouseLeaveTooltipContent;
                 return l().createElement("div", e({
                     ref: n,
-                    style: s,
+                    style: h,
                     role: "tooltip",
-                    "x-placement": p,
-                    className: b()(a, "tooltip", "bs-tooltip-".concat(f)),
-                    onMouseOver: g,
-                    onMouseLeave: y
-                }, d), l().createElement("div", e({
+                    "x-placement": g,
+                    className: b()(a, "tooltip", "bs-tooltip-".concat(y)),
+                    onMouseOver: _,
+                    onMouseLeave: x
+                }, m), l().createElement("div", e({
                     className: "tooltip-arrow"
                 }, u)), l().createElement("div", {
                     className: "tooltip-inner"
                 }, c))
             })),
-            sp = ["children", "is_open", "loading_state", "className", "class_name", "style", "id", "hide_arrow", "offset", "body"],
-            op = function(t) {
+            Ap = ["children", "is_open", "loading_state", "className", "class_name", "style", "id", "hide_arrow", "offset", "body"],
+            Fp = function(t) {
                 var n = t.children,
                     r = t.is_open,
                     a = t.loading_state,
                     s = t.className,
                     i = t.class_name,
                     c = t.style,
                     u = t.id,
                     d = t.hide_arrow,
                     p = t.offset,
                     f = t.body,
-                    g = o(t, sp),
+                    g = o(t, Ap),
                     b = p ? {
                         modifiers: [{
                             name: "offset",
                             options: {
                                 offset: "string" == typeof p ? p.split(",").map((function(e) {
                                     return parseInt(e)
                                 })) : [0, p]
                             }
                         }]
                     } : {};
-                return l().createElement(Zd, e({
+                return l().createElement(Cp, e({
                     "data-dash-is-loading": a && a.is_loading || void 0,
                     defaultShow: r,
                     popperConfig: b
-                }, m(["persistence", "persisted_props", "persistence_type"], g)), l().createElement(rp, {
+                }, m(["persistence", "persisted_props", "persistence_type"], g)), l().createElement($p, {
                     style: c,
                     id: u,
                     className: i || s,
                     hideArrow: d,
                     body: f
                 }, n))
             };
-        op.defaultProps = {
+        Fp.defaultProps = {
             delay: {
                 show: 0,
                 hide: 50
             },
             placement: "right",
             flip: !0,
             autohide: !1,
             persisted_props: ["is_open"],
             persistence_type: "local"
-        }, op.propTypes = {
+        }, Fp.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             placement: u().oneOf(["auto", "auto-start", "auto-end", "top", "top-start", "top-end", "right", "right-start", "right-end", "bottom", "bottom-start", "bottom-end", "left", "left-start", "left-end"]),
@@ -10210,214 +10580,214 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["is_open"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const ip = op;
-        var lp = ["children", "loading_state", "className", "class_name"],
-            cp = function(t) {
+        const Mp = Fp;
+        var Bp = ["children", "loading_state", "className", "class_name"],
+            zp = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, lp);
-                return l().createElement($d, e({
+                    i = o(t, Bp);
+                return l().createElement(cp, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        cp.propTypes = {
+        zp.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const up = cp;
-        var dp = ["children", "loading_state", "className", "class_name"],
-            pp = function(t) {
+        const Kp = zp;
+        var Hp = ["children", "loading_state", "className", "class_name"],
+            Up = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, dp);
-                return l().createElement(Hd, e({
+                    i = o(t, Hp);
+                return l().createElement(hp, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        pp.propTypes = {
+        Up.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             tag: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const fp = pp;
-        var mp = ["min", "now", "max", "label", "visuallyHidden", "striped", "animated", "className", "style", "variant", "barStyle"],
-            gp = ["isChild", "min", "max"],
-            bp = ["now", "label", "visuallyHidden", "striped", "animated", "variant", "className", "children", "barStyle"],
-            yp = ["children", "loading_state", "color", "className", "class_name", "value", "hide_label", "bar"];
+        const Wp = Up;
+        var qp = ["min", "now", "max", "label", "visuallyHidden", "striped", "animated", "className", "style", "variant", "barStyle"],
+            Vp = ["isChild", "min", "max"],
+            Gp = ["now", "label", "visuallyHidden", "striped", "animated", "variant", "className", "children", "barStyle"],
+            Yp = ["children", "loading_state", "color", "className", "class_name", "value", "hide_label", "bar"];
 
-        function hp(e, t) {
+        function Xp(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function vp(e) {
+        function Jp(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? hp(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : hp(Object(n)).forEach((function(t) {
+                t % 2 ? Xp(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Xp(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var _p = l().createContext({}),
-            xp = 1e3;
+        var Qp = l().createContext({}),
+            Zp = 1e3;
 
-        function Op(e, t, n) {
+        function ef(e, t, n) {
             var r = (e - t) / (n - t) * 100;
-            return Math.round(r * xp) / xp
+            return Math.round(r * Zp) / Zp
         }
 
-        function wp(t, n) {
-            var r, a = t.min,
-                s = t.now,
-                i = t.max,
-                c = t.label,
-                u = t.visuallyHidden,
-                d = t.striped,
-                p = t.animated,
-                f = t.className,
-                m = t.style,
-                g = t.variant,
-                y = t.barStyle,
-                h = o(t, mp);
+        function tf(t, n) {
+            var r = t.min,
+                a = t.now,
+                s = t.max,
+                i = t.label,
+                c = t.visuallyHidden,
+                u = t.striped,
+                d = t.animated,
+                p = t.className,
+                f = t.style,
+                m = t.variant,
+                g = t.barStyle,
+                y = o(t, qp);
             return l().createElement("div", e({
                 ref: n
-            }, h, {
+            }, y, {
                 role: "progressbar",
-                className: b()(f, "progress-bar", (r = {}, Ge(r, "bg-".concat(g), g), Ge(r, "progress-bar-animated", p), Ge(r, "progress-bar-striped", p || d), r)),
-                style: vp(vp({
-                    width: "".concat(Op(s, a, i), "%")
-                }, m), y),
-                "aria-valuenow": s,
-                "aria-valuemin": a,
-                "aria-valuemax": i
-            }), u ? l().createElement("span", {
+                className: b()(p, "progress-bar", Ve(Ve(Ve({}, "bg-".concat(m), m), "progress-bar-animated", d), "progress-bar-striped", d || u)),
+                style: Jp(Jp({
+                    width: "".concat(ef(a, r, s), "%")
+                }, f), g),
+                "aria-valuenow": a,
+                "aria-valuemin": r,
+                "aria-valuemax": s
+            }), c ? l().createElement("span", {
                 className: "visually-hidden"
-            }, c) : c)
+            }, i) : i)
         }
-        var Np = l().forwardRef((function(t, n) {
+        var nf = l().forwardRef((function(t, n) {
             var r = t.isChild,
                 a = t.min,
                 s = t.max,
-                c = o(t, gp);
+                c = o(t, Vp);
             if (r) {
-                var u = (0, i.useContext)(_p);
-                return wp(vp(vp({}, c), {}, {
+                var u = (0, i.useContext)(Qp);
+                return tf(Jp(Jp({}, c), {}, {
                     max: s || u.max,
                     min: a || u.min
                 }), n)
             }
             var d = c.now,
                 p = c.label,
                 f = c.visuallyHidden,
                 m = c.striped,
                 g = c.animated,
                 y = c.variant,
                 h = c.className,
                 v = c.children,
                 _ = c.barStyle,
-                x = o(c, bp);
+                x = o(c, Gp);
             return a = void 0 === a ? 0 : a, s = void 0 === s ? 100 : s, l().createElement("div", e({
                 ref: n
             }, x, {
                 className: b()(h, "progress")
-            }), l().createElement(_p.Provider, {
+            }), l().createElement(Qp.Provider, {
                 value: {
                     min: a,
                     max: s
                 }
-            }, v ? cr(v, (function(e) {
+            }, v ? hr(v, (function(e) {
                 return (0, i.cloneElement)(e, {
                     isChild: !0
                 })
-            })) : wp({
+            })) : tf({
                 min: a,
                 now: d,
                 max: s,
                 label: p,
                 visuallyHidden: f,
                 striped: m,
                 animated: g,
                 variant: y,
                 barStyle: _
             }, n)))
         }));
-        Np.defaultProps = {
+        nf.defaultProps = {
             animated: !1,
             isChild: !1,
             visuallyHidden: !1,
             striped: !1
         };
-        var Ep = function(t) {
+        var rf = function(t) {
             var n = t.children,
                 r = t.loading_state,
                 a = t.color,
                 s = t.className,
                 i = t.class_name,
                 c = t.value,
                 u = t.hide_label,
                 d = t.bar,
-                p = o(t, yp),
-                f = Et.has(a);
-            return l().createElement(Np, e({
+                p = o(t, Yp),
+                f = Ot.has(a);
+            return l().createElement(nf, e({
                 className: i || s
             }, m(["setProps"], p), {
                 "data-dash-is-loading": r && r.is_loading || void 0,
                 now: c,
                 isChild: d,
                 variant: f ? a : null,
                 visuallyHidden: u,
                 barStyle: f ? {} : {
                     backgroundColor: a
                 }
             }), n)
         };
-        Ep.defaultProps = {
+        rf.defaultProps = {
             hide_label: !1
-        }, Ep.propTypes = {
+        }, rf.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             bar: u().bool,
@@ -10431,48 +10801,48 @@
             color: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const jp = Ep;
+        const af = rf;
 
-        function kp(e, t) {
+        function sf(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Pp(e) {
+        function of(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? kp(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : kp(Object(n)).forEach((function(t) {
+                t % 2 ? sf(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : sf(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Cp = function(e) {
+        var lf = function(e) {
             var t = e.id,
                 n = e.className,
                 r = e.class_name,
                 a = e.style,
                 s = e.options,
                 o = e.key,
                 i = e.loading_state,
                 c = e.name,
-                u = Me(s).map((function(t) {
+                u = Ie(s).map((function(t) {
                     return function(t) {
                         var n = e.id,
                             r = e.inputClassName,
                             a = e.input_class_name,
                             s = e.inputCheckedStyle,
                             o = e.input_checked_style,
                             i = e.inputStyle,
@@ -10488,15 +10858,15 @@
                             _ = e.labelCheckedStyle,
                             x = e.label_checked_style,
                             O = e.setProps,
                             w = e.inline,
                             N = e.value,
                             E = e.switch,
                             j = t.value === N,
-                            k = j ? Pp(Pp({}, v || h), x || _) : v || h,
+                            k = j ? of(of({}, v || h), x || _) : v || h,
                             P = t.input_id || "_dbcprivate_radioitems_".concat(n, "_input_").concat(t.value);
                         return l().createElement("div", {
                             className: b()("form-check", w && "form-check-inline", E && "form-switch"),
                             key: t.value
                         }, l().createElement("input", {
                             id: P,
                             name: c,
@@ -10524,15 +10894,15 @@
                 id: t,
                 className: r || n,
                 style: a,
                 key: o,
                 "data-dash-is-loading": i && i.is_loading || void 0
             }, u)
         };
-        Cp.propTypes = {
+        lf.propTypes = {
             options: u().oneOfType([u().arrayOf(u().oneOfType([u().string, u().number])), u().object, u().arrayOf(u().exact({
                 label: u().node.isRequired,
                 value: u().oneOfType([u().string, u().number]).isRequired,
                 disabled: u().bool,
                 input_id: u().string,
                 label_id: u().string
             }))]),
@@ -10566,29 +10936,29 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             name: u().string
-        }, Cp.defaultProps = {
+        }, lf.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             options: [],
             persisted_props: ["value"],
             persistence_type: "local"
         };
-        const Tp = Cp;
-        var Sp = function(e) {
+        const cf = lf;
+        var uf = function(e) {
             var t = e.value,
                 n = e.disabled,
                 r = e.className,
                 a = e.class_name,
                 s = e.style,
                 o = e.id,
                 i = e.input_class_name,
@@ -10623,15 +10993,15 @@
             }), l().createElement("label", {
                 id: p,
                 style: f,
                 className: b()(m || g, "form-check-label", "form-label"),
                 htmlFor: o
             }, d))
         };
-        Sp.propTypes = {
+        uf.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             input_style: u().object,
             inputStyle: u().object,
             input_class_name: u().string,
@@ -10650,38 +11020,38 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
-        }, Sp.defaultProps = {
+        }, uf.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             persisted_props: ["value"],
             persistence_type: "local",
             value: !1,
             disabled: !1
         };
-        const Rp = Sp,
-            Dp = i.forwardRef((({
+        const df = uf,
+            pf = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 as: n = "div",
                 ...r
             }, a) => {
-                const s = j(e, "row"),
-                    o = k(),
-                    i = P(),
+                const s = E(e, "row"),
+                    o = j(),
+                    i = k(),
                     l = `${s}-cols`,
                     c = [];
                 return o.forEach((e => {
                     const t = r[e];
                     let n;
                     delete r[e], null != t && "object" == typeof t ? ({
                         cols: n
@@ -10690,104 +11060,104 @@
                     null != n && c.push(`${l}${a}-${n}`)
                 })), (0, _.jsx)(n, {
                     ref: a,
                     ...r,
                     className: b()(t, s, ...c)
                 })
             }));
-        Dp.displayName = "Row";
-        const Lp = Dp;
-        var $p = ["children", "className", "class_name", "align", "justify", "loading_state"],
-            Ip = {
+        pf.displayName = "Row";
+        const ff = pf;
+        var mf = ["children", "className", "class_name", "align", "justify", "loading_state"],
+            gf = {
                 start: "align-items-start",
                 center: "align-items-center",
                 end: "align-items-end",
                 stretch: "align-items-stretch",
                 baseline: "align-items-baseline"
             },
-            Ap = {
+            bf = {
                 start: "justify-content-start",
                 center: "justify-content-center",
                 end: "justify-content-end",
                 around: "justify-content-around",
                 between: "justify-content-between",
                 evenly: "justify-content-evenly"
             },
-            Mp = function(t) {
+            yf = function(t) {
                 var n = t.children,
                     r = t.className,
                     a = t.class_name,
                     s = t.align,
                     i = t.justify,
                     c = t.loading_state,
-                    u = o(t, $p),
-                    d = s && Ip[s],
-                    p = i && Ap[i],
+                    u = o(t, mf),
+                    d = s && gf[s],
+                    p = i && bf[i],
                     f = b()(a || r, d, p);
-                return l().createElement(Lp, e({
+                return l().createElement(ff, e({
                     className: f
                 }, m(["setProps"], u), {
                     "data-dash-is-loading": c && c.is_loading || void 0
                 }), n)
             };
-        Mp.propTypes = {
+        yf.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             align: u().oneOf(["start", "center", "end", "stretch", "baseline"]),
             justify: u().oneOf(["start", "center", "end", "around", "between", "evenly"]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Fp = Mp;
-        var Bp = ["className", "class_name", "html_size", "valid", "invalid", "value"],
-            zp = function(t) {
+        const hf = yf;
+        var vf = ["className", "class_name", "html_size", "valid", "invalid", "value"],
+            _f = function(t) {
                 var n = t.className,
                     r = t.class_name,
                     a = t.html_size,
                     s = t.valid,
                     i = t.invalid,
                     c = t.value,
-                    u = o(t, Bp);
-                return l().createElement(Xi, e({}, m(["setProps", "options", "persistence", "persistence_type", "persisted_props", "loading_state"], u), {
+                    u = o(t, vf);
+                return l().createElement(dl, e({}, m(["setProps", "options", "persistence", "persistence_type", "persisted_props", "loading_state"], u), {
                     isInvalid: i,
                     isValid: s,
                     onChange: function(e) {
                         t.setProps && t.setProps({
                             value: e.target.value
                         })
                     },
                     className: r || n,
                     htmlSize: a,
                     value: c || ""
                 }), l().createElement("option", {
                     value: "",
                     disabled: !0,
                     hidden: !0
-                }, t.placeholder), t.options && Me(t.options).map((function(e) {
+                }, t.placeholder), t.options && Ie(t.options).map((function(e) {
                     return l().createElement("option", {
                         key: e.value,
                         value: e.value,
                         disabled: e.disabled,
                         title: e.title
                     }, e.label)
                 })))
             };
-        zp.defaultProps = {
+        _f.defaultProps = {
             value: "",
             persisted_props: ["value"],
             persistence_type: "local",
             placeholder: ""
-        }, zp.propTypes = {
+        }, _f.propTypes = {
             options: u().oneOfType([u().arrayOf(u().oneOfType([u().string, u().number])), u().object, u().arrayOf(u().exact({
                 label: u().oneOfType([u().string, u().number]).isRequired,
                 value: u().string.isRequired,
                 disabled: u().bool,
                 title: u().string
             }))]),
             value: u().oneOfType([u().string, u().number]),
@@ -10804,112 +11174,112 @@
             size: u().string,
             html_size: u().string,
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             name: u().string
         };
-        const Kp = zp,
-            Hp = i.forwardRef((({
+        const xf = _f,
+            Of = i.forwardRef((({
                 bsPrefix: e,
                 variant: t,
                 animation: n = "border",
                 size: r,
                 as: a = "div",
                 className: s,
                 ...o
             }, i) => {
-                const l = `${e=j(e,"spinner")}-${n}`;
+                const l = `${e=E(e,"spinner")}-${n}`;
                 return (0, _.jsx)(a, {
                     ref: i,
                     ...o,
                     className: b()(s, l, r && `${l}-${r}`, t && `text-${t}`)
                 })
             }));
-        Hp.displayName = "Spinner";
-        const Wp = Hp;
-        var Up = ["children", "color", "loading_state", "spinner_style", "spinnerClassName", "spinner_class_name", "fullscreen", "fullscreenClassName", "fullscreen_class_name", "fullscreen_style", "delay_hide", "delay_show", "show_initially", "type"];
+        Of.displayName = "Spinner";
+        const wf = Of;
+        var Nf = ["children", "color", "loading_state", "spinner_style", "spinnerClassName", "spinner_class_name", "fullscreen", "fullscreenClassName", "fullscreen_class_name", "fullscreen_style", "delay_hide", "delay_show", "show_initially", "type"];
 
-        function qp(e, t) {
+        function Ef(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function Vp(e) {
+        function jf(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? qp(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : qp(Object(n)).forEach((function(t) {
+                t % 2 ? Ef(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ef(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var Gp = function(t) {
+        var kf = function(t) {
             var n = t.children,
                 r = t.color,
                 a = t.loading_state,
                 s = t.spinner_style,
                 c = t.spinnerClassName,
                 u = t.spinner_class_name,
                 d = t.fullscreen,
                 p = t.fullscreenClassName,
                 f = t.fullscreen_class_name,
                 g = t.fullscreen_style,
                 b = t.delay_hide,
                 y = t.delay_show,
                 h = t.show_initially,
                 v = t.type,
-                _ = o(t, Up),
-                x = Le((0, i.useState)(h), 2),
+                _ = o(t, Nf),
+                x = Se((0, i.useState)(h), 2),
                 O = x[0],
                 w = x[1],
                 N = (0, i.useRef)(),
                 E = (0, i.useRef)();
             (0, i.useEffect)((function() {
                 a && (a.is_loading ? (N.current && (N.current = clearTimeout(N.current)), O || E.current || (E.current = setTimeout((function() {
                     w(!0), E.current = null
                 }), y))) : (E.current && (E.current = clearTimeout(E.current)), O && !N.current && (N.current = setTimeout((function() {
                     w(!1), N.current = null
                 }), b))))
             }), [b, y, a]);
-            var j = Et.has(r),
-                k = Vp({
+            var j = Ot.has(r),
+                k = jf({
                     position: "fixed",
                     width: "100vw",
                     height: "100vh",
                     top: 0,
                     left: 0,
                     backgroundColor: "white",
                     display: "flex",
                     justifyContent: "center",
                     alignItems: "center",
                     zIndex: 99,
                     visibility: "visible"
                 }, g),
                 P = function(t) {
                     var n = t.style;
-                    return l().createElement(Wp, e({
+                    return l().createElement(wf, e({
                         variant: j ? r : null,
                         animation: v,
-                        style: Vp({
+                        style: jf({
                             color: !j && r
                         }, n),
                         className: u || c
                     }, m(["setProps"], _)))
                 };
             if (n) {
-                var C = Vp({
+                var C = jf({
                     display: "block",
                     margin: "1rem auto"
                 }, s);
                 return l().createElement("div", {
                     style: O ? {
                         visibility: "hidden",
                         position: "relative"
@@ -10935,20 +11305,20 @@
                 style: k
             }, l().createElement(P, {
                 style: s
             })) : l().createElement(P, {
                 style: s
             })
         };
-        Gp._dashprivate_isLoadingComponent = !0, Gp.defaultProps = {
+        kf._dashprivate_isLoadingComponent = !0, kf.defaultProps = {
             delay_hide: 0,
             delay_show: 0,
             show_initially: !0,
             type: "border"
-        }, Gp.propTypes = {
+        }, kf.propTypes = {
             id: u().string,
             children: u().node,
             fullscreen_style: u().object,
             spinner_style: u().object,
             fullscreen_class_name: u().string,
             fullscreenClassName: u().string,
             spinner_class_name: u().string,
@@ -10957,81 +11327,81 @@
             type: u().string,
             size: u().string,
             fullscreen: u().bool,
             delay_hide: u().number,
             delay_show: u().number,
             show_initially: u().bool
         };
-        const Yp = Gp;
+        const Pf = kf;
 
-        function Xp(e, t = x, n = O) {
+        function Cf(e, t = x, n = "xs") {
             const r = [];
             return Object.entries(e).forEach((([e, a]) => {
                 null != a && ("object" == typeof a ? t.forEach((t => {
                     const s = a[t];
                     if (null != s) {
                         const a = t !== n ? `-${t}` : "";
                         r.push(`${e}${a}-${s}`)
                     }
                 })) : r.push(`${e}-${a}`))
             })), r
         }
-        const Jp = i.forwardRef((({
+        const Tf = i.forwardRef((({
             as: e = "div",
             bsPrefix: t,
             className: n,
             direction: r,
             gap: a,
             ...s
         }, o) => {
-            t = j(t, "horizontal" === r ? "hstack" : "vstack");
-            const i = k(),
-                l = P();
+            t = E(t, "horizontal" === r ? "hstack" : "vstack");
+            const i = j(),
+                l = k();
             return (0, _.jsx)(e, {
                 ...s,
                 ref: o,
-                className: b()(n, t, ...Xp({
+                className: b()(n, t, ...Cf({
                     gap: a
                 }, i, l))
             })
         }));
-        Jp.displayName = "Stack";
-        const Qp = Jp;
-        var Zp = ["children", "loading_state", "className", "class_name"],
-            ef = function(t) {
+        Tf.displayName = "Stack";
+        const Sf = Tf;
+        var Rf = ["children", "loading_state", "className", "class_name"],
+            Df = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
-                    i = o(t, Zp);
-                return l().createElement(Qp, e({
+                    i = o(t, Rf);
+                return l().createElement(Sf, e({
                     className: s || a
                 }, m(["setProps"], i), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        ef.defaultPropTypes = {
+        Df.defaultPropTypes = {
             direction: "vertical"
-        }, ef.propTypes = {
+        }, Df.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             direction: u().oneOf(["vertical", "horizontal"]),
             gap: u().number
         };
-        const tf = ef;
-        var nf = function(e) {
+        const Lf = Df;
+        var $f = function(e) {
             var t = e.value,
                 n = e.disabled,
                 r = e.className,
                 a = e.class_name,
                 s = e.style,
                 o = e.id,
                 i = e.input_class_name,
@@ -11065,15 +11435,15 @@
             }), l().createElement("label", {
                 id: p,
                 style: f,
                 className: b()(m || g, "form-check-label", "form-label"),
                 htmlFor: o
             }, d))
         };
-        nf.propTypes = {
+        $f.propTypes = {
             id: u().string,
             class_name: u().string,
             className: u().string,
             style: u().object,
             input_style: u().object,
             inputStyle: u().object,
             input_class_name: u().string,
@@ -11092,35 +11462,35 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"]),
             setProps: u().func
-        }, nf.defaultProps = {
+        }, $f.defaultProps = {
             inputStyle: {},
             input_style: null,
             inputClassName: "",
             input_class_name: "",
             labelStyle: {},
             label_style: null,
             labelClassName: "",
             label_class_name: "",
             persisted_props: ["value"],
             persistence_type: "local",
             value: !1,
             disabled: !1
         };
-        const rf = nf;
-        var af = function(e) {
+        const If = $f;
+        var Af = function(e) {
             return l().createElement("div", null, e.children)
         };
-        af.defaultProps = {
+        Af.defaultProps = {
             disabled: !1
-        }, af.propTypes = {
+        }, Af.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             tab_style: u().object,
             active_tab_style: u().object,
             label_style: u().object,
             active_label_style: u().object,
@@ -11140,43 +11510,43 @@
             disabled: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const sf = af,
-            of = ["active", "eventKey", "mountOnEnter", "transition", "unmountOnExit", "role", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited"],
-            lf = ["activeKey", "getControlledId", "getControllerId"],
-            cf = ["as"];
+        const Ff = Af,
+            Mf = ["active", "eventKey", "mountOnEnter", "transition", "unmountOnExit", "role", "onEnter", "onEntering", "onEntered", "onExit", "onExiting", "onExited"],
+            Bf = ["activeKey", "getControlledId", "getControllerId"],
+            zf = ["as"];
 
-        function uf(e, t) {
+        function Kf(e, t) {
             if (null == e) return {};
             var n, r, a = {},
                 s = Object.keys(e);
             for (r = 0; r < s.length; r++) n = s[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
             return a
         }
 
-        function df(e) {
+        function Hf(e) {
             let {
                 active: t,
                 eventKey: n,
                 mountOnEnter: r,
                 transition: a,
                 unmountOnExit: s,
                 role: o = "tabpanel",
                 onEnter: l,
                 onEntering: c,
                 onEntered: u,
                 onExit: d,
                 onExiting: p,
                 onExited: f
-            } = e, m = uf(e, of);
-            const g = (0, i.useContext)(Zo);
+            } = e, m = Kf(e, Mf);
+            const g = (0, i.useContext)(pi);
             if (!g) return [Object.assign({}, m, {
                 role: o
             }), {
                 eventKey: n,
                 isActive: t,
                 mountOnEnter: r,
                 transition: a,
@@ -11188,52 +11558,52 @@
                 onExiting: p,
                 onExited: f
             }];
             const {
                 activeKey: b,
                 getControlledId: y,
                 getControllerId: h
-            } = g, v = uf(g, lf), _ = vo(n);
+            } = g, v = Kf(g, Bf), _ = Co(n);
             return [Object.assign({}, m, {
                 role: o,
                 id: y(n),
                 "aria-labelledby": h(n)
             }), {
                 eventKey: n,
-                isActive: null == t && null != _ ? vo(b) === _ : t,
+                isActive: null == t && null != _ ? Co(b) === _ : t,
                 transition: a || v.transition,
                 mountOnEnter: null != r ? r : v.mountOnEnter,
                 unmountOnExit: null != s ? s : v.unmountOnExit,
                 onEnter: l,
                 onEntering: c,
                 onEntered: u,
                 onExit: d,
                 onExiting: p,
                 onExited: f
             }]
         }
-        const pf = i.forwardRef(((e, t) => {
+        const Uf = i.forwardRef(((e, t) => {
             let {
                 as: n = "div"
-            } = e, r = uf(e, cf);
+            } = e, r = Kf(e, zf);
             const [a, {
                 isActive: s,
                 onEnter: o,
                 onEntering: i,
                 onEntered: l,
                 onExit: c,
                 onExiting: u,
                 onExited: d,
                 mountOnEnter: p,
                 unmountOnExit: f,
-                transition: m = fc
-            }] = df(r);
-            return (0, _.jsx)(Zo.Provider, {
+                transition: m = Cc
+            }] = Hf(r);
+            return (0, _.jsx)(pi.Provider, {
                 value: null,
-                children: (0, _.jsx)(_o.Provider, {
+                children: (0, _.jsx)(To.Provider, {
                     value: null,
                     children: (0, _.jsx)(m, {
                         in: s,
                         onEnter: o,
                         onEntering: i,
                         onEntered: l,
                         onExit: c,
@@ -11246,60 +11616,71 @@
                             hidden: !s,
                             "aria-hidden": !s
                         }))
                     })
                 })
             })
         }));
-        pf.displayName = "TabPanel";
-        const ff = e => {
+        Uf.displayName = "TabPanel";
+        const Wf = e => {
             const {
                 id: t,
                 generateChildId: n,
                 onSelect: r,
                 activeKey: a,
                 defaultActiveKey: s,
                 transition: o,
                 mountOnEnter: l,
                 unmountOnExit: c,
                 children: u
-            } = e, [d, p] = Oa(a, s, r), f = fo(t), m = (0, i.useMemo)((() => n || ((e, t) => f ? `${f}-${t}-${e}` : null)), [f, n]), g = (0, i.useMemo)((() => ({
+            } = e, [d, p] = Ta(a, s, r), f = _o(t), m = (0, i.useMemo)((() => n || ((e, t) => f ? `${f}-${t}-${e}` : null)), [f, n]), g = (0, i.useMemo)((() => ({
                 onSelect: p,
                 activeKey: d,
                 transition: o,
                 mountOnEnter: l || !1,
                 unmountOnExit: c || !1,
                 getControlledId: e => m(e, "tabpane"),
                 getControllerId: e => m(e, "tab")
             })), [p, d, o, l, c, m]);
-            return (0, _.jsx)(Zo.Provider, {
+            return (0, _.jsx)(pi.Provider, {
                 value: g,
-                children: (0, _.jsx)(_o.Provider, {
+                children: (0, _.jsx)(To.Provider, {
                     value: p || null,
                     children: u
                 })
             })
         };
-        ff.Panel = pf;
-        const mf = ff;
+        Wf.Panel = Uf;
+        const qf = Wf;
 
-        function gf(e) {
-            return "boolean" == typeof e ? e ? dt : fc : e
+        function Vf(e) {
+            return "boolean" == typeof e ? e ? bt : Cc : e
         }
-        const bf = ({
+        const Gf = ({
             transition: e,
             ...t
-        }) => (0, _.jsx)(mf, {
+        }) => (0, _.jsx)(qf, {
             ...t,
-            transition: gf(e)
+            transition: Vf(e)
         });
-        bf.displayName = "TabContainer";
-        const yf = bf,
-            hf = ht("tab-content"),
-            vf = i.forwardRef((({
+        Gf.displayName = "TabContainer";
+        const Yf = Gf,
+            Xf = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "tab-content"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Xf.displayName = "TabContent";
+        const Jf = Xf,
+            Qf = i.forwardRef((({
                 bsPrefix: e,
                 transition: t,
                 ...n
             }, r) => {
                 const [{
                     className: a,
                     as: s = "div",
@@ -11310,22 +11691,22 @@
                     onEntering: c,
                     onEntered: u,
                     onExit: d,
                     onExiting: p,
                     onExited: f,
                     mountOnEnter: m,
                     unmountOnExit: g,
-                    transition: y = dt
-                }] = df({
+                    transition: y = bt
+                }] = Hf({
                     ...n,
-                    transition: gf(t)
-                }), h = j(e, "tab-pane");
-                return (0, _.jsx)(Zo.Provider, {
+                    transition: Vf(t)
+                }), h = E(e, "tab-pane");
+                return (0, _.jsx)(pi.Provider, {
                     value: null,
-                    children: (0, _.jsx)(_o.Provider, {
+                    children: (0, _.jsx)(To.Provider, {
                         value: null,
                         children: (0, _.jsx)(y, {
                             in: i,
                             onEnter: l,
                             onEntering: c,
                             onEntered: u,
                             onExit: d,
@@ -11338,130 +11719,130 @@
                                 ref: r,
                                 className: b()(a, h, i && "active")
                             })
                         })
                     })
                 })
             }));
-        vf.displayName = "TabPane";
-        const _f = vf,
-            xf = {
+        Qf.displayName = "TabPane";
+        const Zf = Qf,
+            em = {
                 eventKey: u().oneOfType([u().string, u().number]),
                 title: u().node.isRequired,
                 disabled: u().bool,
                 tabClassName: u().string,
                 tabAttrs: u().object
             },
-            Of = () => {
+            tm = () => {
                 throw new Error("ReactBootstrap: The `Tab` component is not meant to be rendered! It's an abstract component that is only valid as a direct Child of the `Tabs` Component. For custom tabs components use TabPane and TabsContainer directly")
             };
-        Of.propTypes = xf;
-        const wf = Object.assign(Of, {
-            Container: yf,
-            Content: hf,
-            Pane: _f
+        tm.propTypes = em;
+        const nm = Object.assign(tm, {
+            Container: Yf,
+            Content: Jf,
+            Pane: Zf
         });
-        var Nf = ["children", "tab_id", "id", "label", "tab_style", "active_tab_style", "label_style", "active_label_style", "tabClassName", "tab_class_name", "activeTabClassName", "active_tab_class_name", "labelClassName", "label_class_name", "activeLabelClassName", "active_label_class_name", "loading_state"];
+        var rm = ["children", "tab_id", "id", "label", "tab_style", "active_tab_style", "label_style", "active_label_style", "tabClassName", "tab_class_name", "activeTabClassName", "active_tab_class_name", "labelClassName", "label_class_name", "activeLabelClassName", "active_label_class_name", "loading_state"];
 
-        function Ef(e, t) {
+        function am(e, t) {
             var n = Object.keys(e);
             if (Object.getOwnPropertySymbols) {
                 var r = Object.getOwnPropertySymbols(e);
                 t && (r = r.filter((function(t) {
                     return Object.getOwnPropertyDescriptor(e, t).enumerable
                 }))), n.push.apply(n, r)
             }
             return n
         }
 
-        function jf(e) {
+        function sm(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = null != arguments[t] ? arguments[t] : {};
-                t % 2 ? Ef(Object(n), !0).forEach((function(t) {
-                    Ge(e, t, n[t])
-                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ef(Object(n)).forEach((function(t) {
+                t % 2 ? am(Object(n), !0).forEach((function(t) {
+                    Ve(e, t, n[t])
+                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : am(Object(n)).forEach((function(t) {
                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                 }))
             }
             return e
         }
-        var kf = function(t) {
+        var om = function(t) {
             var n = t.children,
                 r = t.id,
                 a = t.className,
                 s = t.class_name,
                 c = t.style,
                 u = t.active_tab,
                 d = t.key,
                 p = t.loading_state,
                 f = t.setProps;
-            n = Ie(n), (0, i.useEffect)((function() {
+            n = Le(n), (0, i.useEffect)((function() {
                 f && void 0 === u && f({
-                    active_tab: n && (Ae(n[0]).tab_id || "tab-0")
+                    active_tab: n && ($e(n[0]).tab_id || "tab-0")
                 })
             }), []);
             var g = n && n.map((function(e, t) {
-                    var n = Ae(e),
+                    var n = $e(e),
                         r = n.key || n.tab_id || "tab-" + t,
                         a = u === r;
-                    return l().createElement(fi.Item, {
-                        id: Fe(n.id),
+                    return l().createElement(ki.Item, {
+                        id: Ae(n.id),
                         key: r,
-                        style: a ? jf(jf({}, n.tab_style), n.active_tab_style) : n.tab_style,
+                        style: a ? sm(sm({}, n.tab_style), n.active_tab_style) : n.tab_style,
                         className: b()(n.tab_class_name || n.tabClassName, a && (n.active_tab_class_name || n.activeTabClassName))
-                    }, l().createElement(fi.Link, {
+                    }, l().createElement(ki.Link, {
                         className: b()(n.label_class_name || n.labelClassName, a && (n.active_label_class_name || n.activeLabelClassName), {
                             active: a
                         }),
-                        style: jf(jf(jf({}, !n.disabled && {
+                        style: sm(sm(sm({}, !n.disabled && {
                             cursor: "pointer"
                         }), n.label_style), a && n.active_label_style),
                         disabled: n.disabled,
                         onClick: function() {
                             var e;
                             n.disabled || (e = r, f && u !== e && f({
                                 active_tab: e
                             }))
                         }
                     }, n.label))
                 })),
                 y = n && n.map((function(t, n) {
-                    var r = Ae(t),
+                    var r = $e(t),
                         a = (r.children, r.tab_id),
                         s = (r.id, r.label, r.tab_style, r.active_tab_style, r.label_style, r.active_label_style, r.tabClassName, r.tab_class_name, r.activeTabClassName, r.active_tab_class_name, r.labelClassName, r.label_class_name, r.activeLabelClassName, r.active_label_class_name, r.loading_state),
-                        i = o(r, Nf),
+                        i = o(r, rm),
                         c = a || "tab-" + n;
-                    return l().createElement(wf.Pane, e({
+                    return l().createElement(nm.Pane, e({
                         eventKey: c,
                         key: c
                     }, m(["setProps", "persistence", "persistence_type", "persisted_props"], i), {
                         "data-dash-is-loading": s && s.is_loading || void 0
                     }), t)
                 }));
-            return l().createElement(wf.Container, {
+            return l().createElement(nm.Container, {
                 key: d,
                 activeKey: u,
                 onSelect: function(e) {
                     return f({
                         active_tab: e
                     })
                 },
                 "data-dash-is-loading": p && p.is_loading || void 0
-            }, l().createElement(fi, {
+            }, l().createElement(ki, {
                 id: r,
                 variant: "tabs",
                 as: "ul",
                 className: s || a,
                 style: c
-            }, g), l().createElement(wf.Content, null, y))
+            }, g), l().createElement(nm.Content, null, y))
         };
-        kf.defaultProps = {
+        om.defaultProps = {
             persisted_props: ["active_tab"],
             persistence_type: "local"
-        }, kf.propTypes = {
+        }, om.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             active_tab: u().string,
@@ -11470,28 +11851,28 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["active_tab"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const Pf = kf,
-            Cf = i.forwardRef((({
+        const im = om,
+            lm = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
                 striped: n,
                 bordered: r,
                 borderless: a,
                 hover: s,
                 size: o,
                 variant: i,
                 responsive: l,
                 ...c
             }, u) => {
-                const d = j(e, "table"),
+                const d = E(e, "table"),
                     p = b()(t, d, i && `${d}-${i}`, o && `${d}-${o}`, n && `${d}-${"string"==typeof n?`striped-${n}`:"striped"}`, r && `${d}-bordered`, a && `${d}-borderless`, s && `${d}-hover`),
                     f = (0, _.jsx)("table", {
                         ...c,
                         className: p,
                         ref: u
                     });
                 if (l) {
@@ -11499,32 +11880,32 @@
                     return "string" == typeof l && (e = `${e}-${l}`), (0, _.jsx)("div", {
                         className: e,
                         children: f
                     })
                 }
                 return f
             })),
-            Tf = Cf;
-        var Sf = ["children", "loading_state", "className", "class_name", "color", "dark"],
-            Rf = function(t) {
+            cm = lm;
+        var um = ["children", "loading_state", "className", "class_name", "color", "dark"],
+            dm = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.className,
                     s = t.class_name,
                     i = t.color,
                     c = t.dark,
-                    u = o(t, Sf);
-                return l().createElement(Tf, e({
+                    u = o(t, um);
+                return l().createElement(cm, e({
                     className: s || a,
                     variant: i || (c ? "dark" : void 0)
                 }, m(["setProps"], u), {
                     "data-dash-is-loading": r && r.is_loading || void 0
                 }), n)
             };
-        Rf.propTypes = {
+        dm.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             size: u().string,
@@ -11537,17 +11918,17 @@
             responsive: u().oneOfType([u().bool, u().string]),
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Df = Rf;
-        var Lf = ["value", "n_clicks", "n_blur", "n_submit", "setProps", "className", "class_name", "invalid", "valid", "size", "debounce", "loading_state", "autoFocus", "autofocus", "maxLength", "maxlength", "minLength", "minlength", "readOnly", "readonly", "accessKey", "accesskey", "contentEditable", "contenteditable", "contextMenu", "contextmenu", "spellCheck", "spellcheck", "tabIndex", "tabindex"],
-            $f = function(t) {
+        const pm = dm;
+        var fm = ["value", "n_clicks", "n_blur", "n_submit", "setProps", "className", "class_name", "invalid", "valid", "size", "debounce", "loading_state", "autoFocus", "autofocus", "maxLength", "maxlength", "minLength", "minlength", "readOnly", "readonly", "accessKey", "accesskey", "contentEditable", "contenteditable", "contextMenu", "contextmenu", "spellCheck", "spellcheck", "tabIndex", "tabindex"],
+            mm = function(t) {
                 var n = t.value,
                     r = t.n_clicks,
                     a = t.n_blur,
                     s = t.n_submit,
                     c = t.setProps,
                     u = t.className,
                     d = t.class_name,
@@ -11570,24 +11951,24 @@
                     T = t.contenteditable,
                     S = t.contextMenu,
                     R = t.contextmenu,
                     D = t.spellCheck,
                     L = t.spellcheck,
                     $ = t.tabIndex,
                     I = t.tabindex,
-                    A = o(t, Lf),
-                    M = Le((0, i.useState)(n || ""), 2),
-                    F = M[0],
-                    B = M[1];
+                    A = o(t, fm),
+                    F = Se((0, i.useState)(n || ""), 2),
+                    M = F[0],
+                    B = F[1];
                 (0, i.useEffect)((function() {
-                    n !== F && B(n || "")
+                    n !== M && B(n || "")
                 }), [n]);
                 var z = b()(d || u, p && "is-invalid", f && "is-valid", !!g && "form-control-".concat(g), "form-control");
                 return l().createElement("textarea", e({
-                    value: F,
+                    value: M,
                     className: z,
                     onChange: function(e) {
                         var t = e.target.value;
                         B(t), !y && c && c({
                             value: t
                         })
                     },
@@ -11625,15 +12006,15 @@
                     contextMenu: R || S,
                     spellCheck: L || D,
                     tabIndex: I || $
                 }, m(["n_blur_timestamp", "n_submit_timestamp", "persistence", "persistence_type", "persisted_props"], A), {
                     "data-dash-is-loading": h && h.is_loading || void 0
                 }))
             };
-        $f.propTypes = {
+        mm.propTypes = {
             id: u().string,
             key: u().string,
             value: u().string,
             autofocus: u().string,
             autoFocus: u().string,
             cols: u().oneOfType([u().string, u().number]),
             disabled: u().oneOfType([u().string, u().bool]),
@@ -11682,127 +12063,147 @@
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["value"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
-        }, $f.defaultProps = {
+        }, mm.defaultProps = {
             n_blur: 0,
             n_blur_timestamp: -1,
             n_submit: 0,
             n_submit_timestamp: -1,
             n_clicks: 0,
             n_clicks_timestamp: -1,
             debounce: !1,
             persisted_props: ["value"],
             persistence_type: "local",
             value: ""
         };
-        const If = $f,
-            Af = {
-                [K]: "showing",
-                [W]: "showing show"
+        const gm = mm,
+            bm = {
+                [z]: "showing",
+                [H]: "showing show"
             },
-            Mf = i.forwardRef(((e, t) => (0, _.jsx)(dt, {
+            ym = i.forwardRef(((e, t) => (0, _.jsx)(bt, {
                 ...e,
                 ref: t,
-                transitionClasses: Af
+                transitionClasses: bm
             })));
-        Mf.displayName = "ToastFade";
-        const Ff = Mf,
-            Bf = i.createContext({
+        ym.displayName = "ToastFade";
+        const hm = ym,
+            vm = i.createContext({
                 onClose() {}
             }),
-            zf = i.forwardRef((({
+            _m = i.forwardRef((({
                 bsPrefix: e,
-                closeLabel: t,
+                closeLabel: t = "Close",
                 closeVariant: n,
-                closeButton: r,
+                closeButton: r = !0,
                 className: a,
                 children: s,
                 ...o
             }, l) => {
-                e = j(e, "toast-header");
-                const c = (0, i.useContext)(Bf),
-                    u = Xe((e => {
+                e = E(e, "toast-header");
+                const c = (0, i.useContext)(vm),
+                    u = Ye((e => {
                         null == c || null == c.onClose || c.onClose(e)
                     }));
                 return (0, _.jsxs)("div", {
                     ref: l,
                     ...o,
                     className: b()(e, a),
-                    children: [s, r && (0, _.jsx)(mt, {
+                    children: [s, r && (0, _.jsx)(vt, {
                         "aria-label": t,
                         variant: n,
                         onClick: u,
                         "data-dismiss": "toast"
                     })]
                 })
             }));
-        zf.displayName = "ToastHeader", zf.defaultProps = {
-            closeLabel: "Close",
-            closeButton: !0
-        };
-        const Kf = zf,
-            Hf = ht("toast-body"),
-            Wf = i.forwardRef((({
+        _m.displayName = "ToastHeader";
+        const xm = _m,
+            Om = i.forwardRef((({
+                className: e,
+                bsPrefix: t,
+                as: n = "div",
+                ...r
+            }, a) => (t = E(t, "toast-body"), (0, _.jsx)(n, {
+                ref: a,
+                className: b()(e, t),
+                ...r
+            }))));
+        Om.displayName = "ToastBody";
+        const wm = Om,
+            Nm = i.forwardRef((({
                 bsPrefix: e,
                 className: t,
-                transition: n = Ff,
+                transition: n = hm,
                 show: r = !0,
                 animation: a = !0,
                 delay: s = 5e3,
                 autohide: o = !1,
                 onClose: l,
-                bg: c,
-                ...u
-            }, d) => {
-                e = j(e, "toast");
-                const p = (0, i.useRef)(s),
-                    f = (0, i.useRef)(l);
+                onEntered: c,
+                onExit: u,
+                onExiting: d,
+                onEnter: p,
+                onEntering: f,
+                onExited: m,
+                bg: g,
+                ...y
+            }, h) => {
+                e = E(e, "toast");
+                const v = (0, i.useRef)(s),
+                    x = (0, i.useRef)(l);
                 (0, i.useEffect)((() => {
-                    p.current = s, f.current = l
+                    v.current = s, x.current = l
                 }), [s, l]);
-                const m = sr(),
-                    g = !(!o || !r),
-                    y = (0, i.useCallback)((() => {
-                        g && (null == f.current || f.current())
-                    }), [g]);
+                const O = fr(),
+                    w = !(!o || !r),
+                    N = (0, i.useCallback)((() => {
+                        w && (null == x.current || x.current())
+                    }), [w]);
                 (0, i.useEffect)((() => {
-                    m.set(y, p.current)
-                }), [m, y]);
-                const h = (0, i.useMemo)((() => ({
+                    O.set(N, v.current)
+                }), [O, N]);
+                const j = (0, i.useMemo)((() => ({
                         onClose: l
                     })), [l]),
-                    v = !(!n || !a),
-                    x = (0, _.jsx)("div", {
-                        ...u,
-                        ref: d,
-                        className: b()(e, t, c && `bg-${c}`, !v && (r ? "show" : "hide")),
+                    k = !(!n || !a),
+                    P = (0, _.jsx)("div", {
+                        ...y,
+                        ref: h,
+                        className: b()(e, t, g && `bg-${g}`, !k && (r ? "show" : "hide")),
                         role: "alert",
                         "aria-live": "assertive",
                         "aria-atomic": "true"
                     });
-                return (0, _.jsx)(Bf.Provider, {
-                    value: h,
-                    children: v && n ? (0, _.jsx)(n, {
+                return (0, _.jsx)(vm.Provider, {
+                    value: j,
+                    children: k && n ? (0, _.jsx)(n, {
                         in: r,
+                        onEnter: p,
+                        onEntering: f,
+                        onEntered: c,
+                        onExit: u,
+                        onExiting: d,
+                        onExited: m,
                         unmountOnExit: !0,
-                        children: x
-                    }) : x
+                        children: P
+                    }) : P
                 })
             }));
-        Wf.displayName = "Toast";
-        const Uf = Object.assign(Wf, {
-            Body: Hf,
-            Header: Kf
+        Nm.displayName = "Toast";
+        const Em = Object.assign(Nm, {
+            Body: wm,
+            Header: xm
         });
-        var qf = ["children", "loading_state", "header", "icon", "header_style", "headerClassName", "header_class_name", "body_style", "bodyClassName", "body_class_name", "dismissable", "duration", "n_dismiss", "is_open", "setProps", "className", "class_name", "color"],
-            Vf = function(t) {
+        var jm = ["children", "loading_state", "header", "icon", "header_style", "headerClassName", "header_class_name", "body_style", "bodyClassName", "body_class_name", "dismissable", "duration", "n_dismiss", "is_open", "setProps", "className", "class_name", "color"],
+            km = function(t) {
                 var n = t.children,
                     r = t.loading_state,
                     a = t.header,
                     s = t.icon,
                     c = t.header_style,
                     u = t.headerClassName,
                     d = t.header_class_name,
@@ -11813,35 +12214,35 @@
                     h = t.duration,
                     v = t.n_dismiss,
                     _ = t.is_open,
                     x = t.setProps,
                     O = t.className,
                     w = t.class_name,
                     N = t.color,
-                    E = o(t, qf),
+                    E = o(t, jm),
                     j = function() {
                         x && x({
                             is_open: !1,
                             n_dismiss: v + 1,
                             n_dismiss_timestamp: Date.now()
                         })
                     },
                     k = (0, i.useRef)(null);
                 return (0, i.useEffect)((function() {
                     return h && (_ ? k.current = setTimeout(j, h) : k.current && (clearTimeout(k.current), k.current = null)),
                         function() {
                             return clearTimeout(k.current)
                         }
-                }), [_]), l().createElement(Uf, e({
+                }), [_]), l().createElement(Em, e({
                     show: _,
                     onClose: y && j,
                     className: w || O,
                     bg: N,
                     "data-dash-is-loading": r && r.is_loading || void 0
-                }, m(["n_dismiss_timestamp", "persistence", "persisted_props", "persistence_type", "setProps"], E)), l().createElement(Uf.Header, {
+                }, m(["n_dismiss_timestamp", "persistence", "persisted_props", "persistence_type", "setProps"], E)), l().createElement(Em.Header, {
                     style: c,
                     className: d || u,
                     closeButton: y
                 }, s && l().createElement("svg", {
                     className: "rounded text-".concat(s),
                     width: "20",
                     height: "20",
@@ -11851,27 +12252,27 @@
                     role: "img"
                 }, l().createElement("rect", {
                     fill: "currentColor",
                     width: "100%",
                     height: "100%"
                 })), l().createElement("strong", {
                     className: b()("me-auto", s && "ms-2")
-                }, a)), l().createElement(Uf.Body, {
+                }, a)), l().createElement(Em.Body, {
                     style: p,
                     className: g || f
                 }, n))
             };
-        Vf.defaultProps = {
+        km.defaultProps = {
             is_open: !0,
             n_dismiss: 0,
             n_dismiss_timestamp: -1,
             dismissable: !1,
             persisted_props: ["is_open"],
             persistence_type: "local"
-        }, Vf.propTypes = {
+        }, km.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             header_style: u().object,
             header_class_name: u().string,
@@ -11894,48 +12295,48 @@
                 prop_name: u().string,
                 component_name: u().string
             }),
             persistence: u().oneOfType([u().bool, u().string, u().number]),
             persisted_props: u().arrayOf(u().oneOf(["is_open"])),
             persistence_type: u().oneOf(["local", "session", "memory"])
         };
-        const Gf = Vf;
-        var Yf = ["id", "children", "is_open", "loading_state", "className", "class_name", "style", "fade"],
-            Xf = function(t) {
+        const Pm = km;
+        var Cm = ["id", "children", "is_open", "loading_state", "className", "class_name", "style", "fade"],
+            Tm = function(t) {
                 var n = t.id,
                     r = t.children,
                     a = t.is_open,
                     s = t.loading_state,
                     i = t.className,
                     c = t.class_name,
                     u = t.style,
                     d = t.fade,
-                    p = o(t, Yf);
-                return l().createElement(Zd, e({
+                    p = o(t, Cm);
+                return l().createElement(Cp, e({
                     "data-dash-is-loading": s && s.is_loading || void 0,
                     defaultShow: a
                 }, p, {
                     transition: d
-                }), l().createElement(ap, {
+                }), l().createElement(Ip, {
                     id: n,
                     style: u,
                     className: c || i
                 }, r))
             };
-        Xf.defaultProps = {
+        Tm.defaultProps = {
             delay: {
                 show: 0,
                 hide: 50
             },
             placement: "auto",
             flip: !0,
             autohide: !0,
             fade: !0,
             trigger: "hover focus"
-        }, Xf.propTypes = {
+        }, Tm.propTypes = {
             id: u().string,
             children: u().node,
             style: u().object,
             class_name: u().string,
             className: u().string,
             key: u().string,
             target: u().oneOfType([u().string, u().object]),
@@ -11951,10 +12352,10 @@
             is_open: u().bool,
             loading_state: u().shape({
                 is_loading: u().bool,
                 prop_name: u().string,
                 component_name: u().string
             })
         };
-        const Jf = Xf
+        const Sm = Tm
     })(), window.dash_bootstrap_components = r
 })();
```

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_components/metadata.json` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990530303030303%*

 * *Differences: {"'src/components/breadcrumb/Breadcrumb.js'": "{'description': ''}"}*

```diff
@@ -597,15 +597,15 @@
                 "type": {
                     "name": "string"
                 }
             }
         }
     },
     "src/components/breadcrumb/Breadcrumb.js": {
-        "description": "Use breadcrumbs to create a navigation breadcrumb in your app.",
+        "description": "",
         "displayName": "Breadcrumb",
         "methods": [],
         "props": {
             "className": {
                 "description": "**DEPRECATED** - Use class_name instead.\n\nOften used with CSS to style elements with common properties.",
                 "required": false,
                 "type": {
```

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/_table.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/_table.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components/themes.py` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components/themes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 BOOTSTRAP = (
-    "https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap.min.css"
+    "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
 )
 
-GRID = "https://cdn.jsdelivr.net/npm/bootstrap@5.3.1/dist/css/bootstrap-grid.min.css"  # noqa
+GRID = "https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap-grid.min.css"  # noqa
 
-_BOOTSWATCH_BASE = "https://cdn.jsdelivr.net/npm/bootswatch@5.3.1/dist/"
+_BOOTSWATCH_BASE = "https://cdn.jsdelivr.net/npm/bootswatch@5.3.3/dist/"
 
 CERULEAN = _BOOTSWATCH_BASE + "cerulean/bootstrap.min.css"
 COSMO = _BOOTSWATCH_BASE + "cosmo/bootstrap.min.css"
 CYBORG = _BOOTSWATCH_BASE + "cyborg/bootstrap.min.css"
 DARKLY = _BOOTSWATCH_BASE + "darkly/bootstrap.min.css"
 FLATLY = _BOOTSWATCH_BASE + "flatly/bootstrap.min.css"
 JOURNAL = _BOOTSWATCH_BASE + "journal/bootstrap.min.css"
```

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/PKG-INFO` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-bootstrap-components
-Version: 1.6.0b1
+Version: 1.6.0rc1
 Summary: Bootstrap themed components for use in Plotly Dash
 Home-page: https://dash-bootstrap-components.opensource.faculty.ai/
 Author: Faculty
 Author-email: opensource@faculty.ai
 License: Apache Software License
 Project-URL: Bug Reports, https://github.com/facultyai/dash-bootstrap-components/issues
 Project-URL: Source, https://github.com/facultyai/dash-bootstrap-components/
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.0b1 Summary:
-Bootstrap themed components for use in Plotly Dash Home-page: https://dash-
-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
+Metadata-Version: 2.1 Name: dash-bootstrap-components Version: 1.6.0rc1
+Summary: Bootstrap themed components for use in Plotly Dash Home-page: https://
+dash-bootstrap-components.opensource.faculty.ai/ Author: Faculty Author-email:
 opensource@faculty.ai License: Apache Software License Project-URL: Bug
 Reports, https://github.com/facultyai/dash-bootstrap-components/issues Project-
 URL: Source, https://github.com/facultyai/dash-bootstrap-components/
 Classifier: Framework :: Dash Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `dash-bootstrap-components-1.6.0b1/dash_bootstrap_components.egg-info/SOURCES.txt` & `dash_bootstrap_components-1.6.0rc1/dash_bootstrap_components.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,8 +87,9 @@
 dash_bootstrap_components/_components/metadata.json
 tests/test_alert.py
 tests/test_components_as_props.py
 tests/test_navlink.py
 tests/test_popover.py
 tests/test_positional_args.py
 tests/test_tooltip.py
-tests/test_version.py
+tests/test_version.py
+tests/test_xss_links.py
```

### Comparing `dash-bootstrap-components-1.6.0b1/landing-page.md` & `dash_bootstrap_components-1.6.0rc1/landing-page.md`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/setup.cfg` & `dash_bootstrap_components-1.6.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/setup.py` & `dash_bootstrap_components-1.6.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/tests/test_components_as_props.py` & `dash_bootstrap_components-1.6.0rc1/tests/test_components_as_props.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/tests/test_navlink.py` & `dash_bootstrap_components-1.6.0rc1/tests/test_navlink.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/tests/test_popover.py` & `dash_bootstrap_components-1.6.0rc1/tests/test_popover.py`

 * *Files identical despite different names*

### Comparing `dash-bootstrap-components-1.6.0b1/tests/test_positional_args.py` & `dash_bootstrap_components-1.6.0rc1/tests/test_positional_args.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dash import Dash, html
 from dash_bootstrap_components import Checklist, RadioItems, Select
+from selenium.webdriver.common.by import By
 
 
 def test_dbpa001_checklist(dash_duo):
     """
     Check that the options and value positional arguments are working for
     Checklist.
     """
@@ -27,35 +28,35 @@
     app.layout = html.Div([with_keywords, without_keywords])
 
     dash_duo.start_server(app)
 
     # Check values
     assert [
         a.get_attribute("value")
-        for a in dash_duo.wait_for_element(
-            "#with-keywords"
-        ).find_elements_by_tag_name("input")
+        for a in dash_duo.wait_for_element("#with-keywords").find_elements(
+            by=By.TAG_NAME, value="input"
+        )
     ] == [
         a.get_attribute("value")
-        for a in dash_duo.wait_for_element(
-            "#without-keywords"
-        ).find_elements_by_tag_name("input")
+        for a in dash_duo.wait_for_element("#without-keywords").find_elements(
+            by=By.TAG_NAME, value="input"
+        )
     ]
 
     # Check labels
     assert [
         a.text
-        for a in dash_duo.wait_for_element(
-            "#with-keywords"
-        ).find_elements_by_tag_name("label")
+        for a in dash_duo.wait_for_element("#with-keywords").find_elements(
+            by=By.TAG_NAME, value="label"
+        )
     ] == [
         a.text
-        for a in dash_duo.wait_for_element(
-            "#without-keywords"
-        ).find_elements_by_tag_name("label")
+        for a in dash_duo.wait_for_element("#without-keywords").find_elements(
+            by=By.TAG_NAME, value="label"
+        )
     ]
 
 
 def test_dbpa002_radio_items(dash_duo):
     """
     Check that the options and value positional arguments are working for
     RadioItems.
@@ -80,35 +81,35 @@
     app.layout = html.Div([with_keywords, without_keywords])
 
     dash_duo.start_server(app)
 
     # Check values
     assert [
         a.get_attribute("value")
-        for a in dash_duo.wait_for_element(
-            "#with-keywords"
-        ).find_elements_by_tag_name("input")
+        for a in dash_duo.wait_for_element("#with-keywords").find_elements(
+            by=By.TAG_NAME, value="input"
+        )
     ] == [
         a.get_attribute("value")
-        for a in dash_duo.wait_for_element(
-            "#without-keywords"
-        ).find_elements_by_tag_name("input")
+        for a in dash_duo.wait_for_element("#without-keywords").find_elements(
+            by=By.TAG_NAME, value="input"
+        )
     ]
 
     # Check labels
     assert [
         a.text
-        for a in dash_duo.wait_for_element(
-            "#with-keywords"
-        ).find_elements_by_tag_name("label")
+        for a in dash_duo.wait_for_element("#with-keywords").find_elements(
+            by=By.TAG_NAME, value="label"
+        )
     ] == [
         a.text
-        for a in dash_duo.wait_for_element(
-            "#without-keywords"
-        ).find_elements_by_tag_name("label")
+        for a in dash_duo.wait_for_element("#without-keywords").find_elements(
+            by=By.TAG_NAME, value="label"
+        )
     ]
 
 
 def test_dbpa003_select(dash_duo):
     """
     Check that the options and value positional arguments are working for
     Select.
@@ -133,29 +134,29 @@
     app.layout = html.Div([with_keywords, without_keywords])
 
     dash_duo.start_server(app)
 
     # Check values
     assert [
         a.get_attribute("value")
-        for a in dash_duo.wait_for_element(
-            "#with-keywords"
-        ).find_elements_by_tag_name("option")
+        for a in dash_duo.wait_for_element("#with-keywords").find_elements(
+            by=By.TAG_NAME, value="option"
+        )
     ] == [
         a.get_attribute("value")
-        for a in dash_duo.wait_for_element(
-            "#without-keywords"
-        ).find_elements_by_tag_name("option")
+        for a in dash_duo.wait_for_element("#without-keywords").find_elements(
+            by=By.TAG_NAME, value="option"
+        )
     ]
 
     # Check labels
     assert [
         a.text
-        for a in dash_duo.wait_for_element(
-            "#with-keywords"
-        ).find_elements_by_tag_name("option")
+        for a in dash_duo.wait_for_element("#with-keywords").find_elements(
+            by=By.TAG_NAME, value="option"
+        )
     ] == [
         a.text
-        for a in dash_duo.wait_for_element(
-            "#without-keywords"
-        ).find_elements_by_tag_name("option")
+        for a in dash_duo.wait_for_element("#without-keywords").find_elements(
+            by=By.TAG_NAME, value="option"
+        )
     ]
```

### Comparing `dash-bootstrap-components-1.6.0b1/tests/test_tooltip.py` & `dash_bootstrap_components-1.6.0rc1/tests/test_tooltip.py`

 * *Files identical despite different names*

