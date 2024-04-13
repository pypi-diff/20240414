# Comparing `tmp/airbyte_source_shopify-2.0.5.dev202404121134.tar.gz` & `tmp/airbyte_source_shopify-2.0.5.dev202404132146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404121134.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404132146.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.5.dev202404121134.tar` & `airbyte_source_shopify-2.0.5.dev202404132146.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4519 2024-04-12 11:31:33.566932 airbyte_source_shopify-2.0.5.dev202404121134/README.md
--rw-r--r--   0        0        0      812 2024-04-12 11:34:26.886386 airbyte_source_shopify-2.0.5.dev202404121134/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/run.py
--rw-r--r--   0        0        0    16103 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     1272 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     1009 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1109 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0      928 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0      610 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     1170 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     1488 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     1217 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      485 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0     5313 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0      736 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0      909 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    13381 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     5226 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    14757 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     1027 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0      536 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     1329 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0      911 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    17520 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0      728 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0    80187 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     1104 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     3891 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0      907 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     2336 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0     7060 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     1675 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     4059 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0      985 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0      951 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     3750 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    15723 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    55609 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     3629 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-04-12 11:31:33.570932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/spec.json
--rw-r--r--   0        0        0    37655 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11968 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/transform.py
--rw-r--r--   0        0        0    14320 2024-04-12 11:31:33.578932 airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/utils.py
--rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404121134/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/README.md
+-rw-r--r--   0        0        0      812 2024-04-13 21:46:21.619674 airbyte_source_shopify-2.0.5.dev202404132146/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/run.py
+-rw-r--r--   0        0        0    16103 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     1272 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     1009 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     1109 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0      928 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0      610 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     1170 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     1488 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     1217 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      485 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0     5313 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0      736 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0      909 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    13381 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     5226 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    14757 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     1027 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0      536 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     1329 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0      911 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    17520 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0      728 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0    80187 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     1104 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     3891 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0      907 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     2336 2024-04-13 21:43:58.456150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0     7060 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     1675 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     4059 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0      985 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0      951 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     3750 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/scopes.py
+-rw-r--r--   0        0        0     1734 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    18577 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    56188 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     3629 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-04-13 21:43:58.460150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/spec.json
+-rw-r--r--   0        0        0    37186 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11968 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/transform.py
+-rw-r--r--   0        0        0    14320 2024-04-13 21:43:58.468150 airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/utils.py
+-rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404132146/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/README.md` & `airbyte_source_shopify-2.0.5.dev202404132146/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/pyproject.toml` & `airbyte_source_shopify-2.0.5.dev202404132146/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.5.dev202404121134"
+version = "2.0.5.dev202404132146"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/__init__.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/auth.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/scopes.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 import logging
 from dataclasses import dataclass, field
 from enum import Enum
 from time import sleep, time
 from typing import Any, Final, Iterable, List, Mapping, Optional, Union
 
+import pendulum as pdm
 import requests
 from airbyte_cdk import AirbyteLogger
 from requests.exceptions import JSONDecodeError
 from source_shopify.utils import ApiTypeEnum
 from source_shopify.utils import ShopifyRateLimiter as limiter
 
 from .exceptions import AirbyteTracedException, ShopifyBulkExceptions
 from .query import ShopifyBulkTemplates
 from .tools import END_OF_FILE, BulkTools
 
 
 class ShopifyBulkStatus(Enum):
     CREATED = "CREATED"
     CANCELED = "CANCELED"
+    CANCELING = "CANCELING"
     COMPLETED = "COMPLETED"
     RUNNING = "RUNNING"
     FAILED = "FAILED"
     TIMEOUT = "TIMEOUT"
     ACCESS_DENIED = "ACCESS_DENIED"
 
 
@@ -50,47 +52,52 @@
     # sleep time per creation attempt
     concurrent_interval_sec: Final[int] = 30
     # max attempts for job creation
     concurrent_max_retry: Final[int] = 19
     # Each job ideally should be executed within the specified time (in sec),
     # to maximize the performance for multi-connection syncs and control the bulk job size within +- 7 mins (420 sec),
     # Ideally the source will balance on it's own rate, based on the time taken to return the data for the slice.
-    job_elapsed_time_threshold_sec: Final[float] = 420.0
+    job_max_elapsed_time_sec: Final[float] = 420.0
     # 0.1 ~= P2H, default value, lower boundary for slice size
     job_size_min: Final[float] = 0.1
     # P365D, upper boundary for slice size
     job_size_max: Final[float] = 365.0
     # running job logger constrain
-    log_running_job_msg_frequency: Final[int] = 3
+    log_job_state_msg_frequency: Final[int] = 3
     # attempt limit indicator
     concurrent_max_attempt_reached: bool = field(init=False, default=False)
     # attempt counter
     concurrent_attempt: int = field(init=False, default=0)
-    # currents: job_id, job_state
+    # currents: job_id, job_state, job_created_at, job_self_canceled
     job_id: Optional[str] = field(init=False, default=None)
+    job_created_at: Optional[str] = field(init=False, default=None)
+    job_self_canceled: bool = field(init=False, default=False)
     job_state: ShopifyBulkStatus = field(init=False, default=None)
     # 2 sec is set as default value to cover the case with the empty-fast-completed jobs
     job_last_elapsed_time: float = field(init=False, default=2.0)
     # dynamically adjusted slice interval
     job_size: float = field(init=False, default=0.0)
     # expand slice factor
     job_size_expand_factor: int = field(init=False, default=2)
     # reduce slice factor
     job_size_reduce_factor: int = field(init=False, default=2)
+    # whether or not the slicer should revert the previous start value
+    job_should_revert_slice: bool = field(init=False, default=False)
     # running job log counter
-    log_running_job_msg_count: int = field(init=False, default=0)
+    log_job_state_msg_count: int = field(init=False, default=0)
 
     @property
     def tools(self) -> BulkTools:
         return BulkTools()
 
     @property
     def job_state_to_fn_map(self) -> Mapping[str, Any]:
         return {
             ShopifyBulkStatus.CREATED.value: self.on_created_job,
+            ShopifyBulkStatus.CANCELING.value: self.on_canceling_job,
             ShopifyBulkStatus.CANCELED.value: self.on_canceled_job,
             ShopifyBulkStatus.COMPLETED.value: self.on_completed_job,
             ShopifyBulkStatus.RUNNING.value: self.on_running_job,
             ShopifyBulkStatus.TIMEOUT.value: self.on_timeout_job,
             ShopifyBulkStatus.FAILED.value: self.on_failed_job,
             ShopifyBulkStatus.ACCESS_DENIED.value: self.on_access_denied_job,
         }
@@ -111,54 +118,99 @@
     def job_size_adjusted_reduce_factor(self) -> float:
         """
         The Job Size reduce factor is 2, by default.
         """
 
         return self.job_size_reduce_factor
 
+    @property
+    def job_elapsed_time_in_state(self) -> int:
+        """
+        Returns the elapsed time taken while Job is in certain status/state.
+        """
+        return (pdm.now() - pdm.parse(self.job_created_at)).in_seconds() if self.job_created_at else 0
+
+    @property
+    def is_long_running_job(self) -> bool:
+        if self.job_elapsed_time_in_state:
+            if self.job_elapsed_time_in_state > self.job_max_elapsed_time_sec:
+                # set the slicer to revert mode
+                self.job_should_revert_slice = True
+                return True
+        else:
+            # reset slicer to normal mode
+            self.job_should_revert_slice = False
+            return False
+
+    def expand_job_size(self) -> None:
+        self.job_size += self.job_size_adjusted_expand_factor
+
+    def reduce_job_size(self) -> None:
+        self.job_size /= self.job_size_adjusted_reduce_factor
+
     def __adjust_job_size(self, job_current_elapsed_time: float) -> None:
-        if job_current_elapsed_time > self.job_elapsed_time_threshold_sec:
-            self.job_size /= self.job_size_adjusted_reduce_factor
-        elif job_current_elapsed_time < 1 or job_current_elapsed_time < self.job_last_elapsed_time:
-            self.job_size += self.job_size_adjusted_expand_factor
-        elif job_current_elapsed_time > self.job_last_elapsed_time < self.job_elapsed_time_threshold_sec:
+        if not self.job_should_revert_slice:
+            if job_current_elapsed_time > self.job_max_elapsed_time_sec:
+                self.reduce_job_size()
+            elif job_current_elapsed_time < 1 or job_current_elapsed_time < self.job_last_elapsed_time:
+                self.expand_job_size()
+            elif job_current_elapsed_time > self.job_last_elapsed_time < self.job_max_elapsed_time_sec:
+                pass
+
+            # set the last job time
+            self.job_last_elapsed_time = job_current_elapsed_time
+            # check the job size slice interval are acceptable
+            self.job_size = max(self.job_size_min, min(self.job_size, self.job_size_max))
+        else:
             pass
 
-        # set the last job time
-        self.job_last_elapsed_time = job_current_elapsed_time
-        # check the job size slice interval are acceptable
-        self.job_size = max(self.job_size_min, min(self.job_size, self.job_size_max))
-
     def __reset_state(self) -> None:
-        # set current job state to default value
-        self.job_state, self.job_id = None, None
+        # set current job state to default values
+        self.job_state, self.job_id, self.job_self_canceled = None, None, False
         # set the running job message counter to default
-        self.log_running_job_msg_count = 0
+        self.log_job_state_msg_count = 0
 
     def job_completed(self) -> bool:
         return self.job_state == ShopifyBulkStatus.COMPLETED.value
 
-    def log_running_job_state(self) -> None:
+    def job_canceled(self) -> bool:
+        return self.job_state == ShopifyBulkStatus.CANCELED.value
+
+    def job_cancel(self) -> requests.Response:
+        # re-use of `self._session(*, **)` to make BULK Job cancel request
+        cancel_args = self.job_get_request_args(ShopifyBulkTemplates.cancel)
+        with self.session as cancel_job:
+            canceled_response = cancel_job.request(**cancel_args)
+            # mark the job was self-canceled
+            self.job_self_canceled = True
+            return self.job_healthcheck(canceled_response)
+
+    def log_job_state_with_count(self) -> None:
         """
-        Print the `RUNNING` Job info message every 3 request, to minimize the noise in the logs.
+        Print the status/state Job info message every N request, to minimize the noise in the logs.
         """
-        if self.log_running_job_msg_count < self.log_running_job_msg_frequency:
-            self.log_running_job_msg_count += 1
+        if self.log_job_state_msg_count < self.log_job_state_msg_frequency:
+            self.log_job_state_msg_count += 1
         else:
-            self.log_state()
-            self.log_running_job_msg_count = 0
-
-    def log_state(self) -> None:
-        self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` is {self.job_state}.")
+            message = f"Elapsed time: {self.job_elapsed_time_in_state} sec"
+            self.log_state(message)
+            self.log_job_state_msg_count = 0
+
+    def log_state(self, message: Optional[str] = None) -> None:
+        pattern = f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` is {self.job_state}."
+        if message:
+            self.logger.info(f"{pattern}. {message}.")
+        else:
+            self.logger.info(pattern)
 
-    def job_get_state_args(self) -> Mapping[str, Any]:
+    def job_get_request_args(self, template: ShopifyBulkTemplates) -> Mapping[str, Any]:
         return {
             "method": "POST",
             "url": self.base_url,
-            "data": ShopifyBulkTemplates.status(self.job_id),
+            "data": template(self.job_id),
             "headers": {"Content-Type": "application/graphql"},
         }
 
     def job_get_result(self, response: Optional[requests.Response] = None) -> Optional[str]:
         job_result_url = response.json().get("data", {}).get("node", {}).get("url") if response else None
         if job_result_url:
             # save to local file using chunks to avoid OOM
@@ -171,30 +223,42 @@
                     # add `<end_of_file>` line to the bottom  of the saved data for easy parsing
                     file.write(END_OF_FILE.encode())
             return filename
 
     def job_update_state(self, response: Optional[requests.Response] = None) -> None:
         if response:
             self.job_state = response.json().get("data", {}).get("node", {}).get("status")
-            if self.job_state == ShopifyBulkStatus.RUNNING.value:
-                self.log_running_job_state()
+            if self.job_state in [ShopifyBulkStatus.RUNNING.value, ShopifyBulkStatus.CANCELING.value]:
+                self.log_job_state_with_count()
             else:
                 self.log_state()
 
     def on_created_job(self, **kwargs) -> None:
         pass
 
-    def on_canceled_job(self, response: requests.Response) -> AirbyteTracedException:
-        raise ShopifyBulkExceptions.BulkJobCanceled(
-            f"The BULK Job: `{self.job_id}` exited with {self.job_state}, details: {response.text}",
-        )
+    def on_canceled_job(self, response: requests.Response) -> None:
+        if not self.job_self_canceled:
+            raise ShopifyBulkExceptions.BulkJobCanceled(
+                f"The BULK Job: `{self.job_id}` exited with {self.job_state}, details: {response.text}",
+            )
+        else:
+            pass
 
-    def on_running_job(self, **kwargs) -> None:
+    def on_canceling_job(self, **kwargs) -> None:
         sleep(self.job_check_interval_sec)
 
+    def on_running_job(self, **kwargs) -> None:
+        if self.is_long_running_job:
+            self.logger.info(
+                f"Stream: `{self.stream_name}` the BULK Job: {self.job_id} runs longer than expected. The job will be canceled and retried with the smaller Slice Size."
+            )
+            self.job_cancel()
+        else:
+            sleep(self.job_check_interval_sec)
+
     def on_completed_job(self, **kwargs) -> None:
         pass
 
     def on_failed_job(self, response: requests.Response) -> AirbyteTracedException:
         raise ShopifyBulkExceptions.BulkJobFailed(
             f"The BULK Job: `{self.job_id}` exited with {self.job_state}, details: {response.text}",
         )
@@ -218,15 +282,15 @@
         except (Exception, JSONDecodeError) as e:
             raise ShopifyBulkExceptions.BulkJobBadResponse(
                 f"Couldn't check the `response` for `errors`, status: {response.status_code}, response: `{response.text}`. Trace: {repr(e)}."
             )
 
     def job_track_running(self) -> Union[AirbyteTracedException, requests.Response]:
         # format Job state check args
-        status_args = self.job_get_state_args()
+        status_args = self.job_get_request_args(ShopifyBulkTemplates.status)
         # re-use of `self._session(*, **)` to make BULK Job status checks
         with self.session as track_running_job:
             response = track_running_job.request(**status_args)
         # errors check
         errors = self.job_check_for_errors(response)
         if not errors:
             self.job_update_state(response)
@@ -235,14 +299,16 @@
         else:
             # execute ERRORS scenario
             self.on_job_with_errors(errors)
 
     def job_check_state(self) -> Optional[str]:
         while not self.job_completed():
             response = self.job_track_running()
+            if self.job_canceled():
+                return None
         # return `job_result_url` when status is `COMPLETED`
         return self.job_get_result(response)
 
     def has_running_concurrent_job(self, errors: Optional[Iterable[Mapping[str, Any]]] = None) -> bool:
         """
         When concurent BULK Job is already running for the same SHOP we receive:
         Error example:
@@ -281,14 +347,15 @@
         return self.job_healthcheck(self.job_retry_request(request))
 
     def job_get_id(self, response: requests.Response) -> Optional[str]:
         response_data = response.json()
         bulk_response = response_data.get("data", {}).get("bulkOperationRunQuery", {}).get("bulkOperation", {})
         if bulk_response and bulk_response.get("status") == ShopifyBulkStatus.CREATED.value:
             job_id = bulk_response.get("id")
+            self.job_created_at = bulk_response.get("createdAt")
             self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{job_id}` is {ShopifyBulkStatus.CREATED.value}")
             return job_id
         else:
             return None
 
     def job_retry_on_concurrency(self, request: requests.PreparedRequest) -> Union[AirbyteTracedException, Optional[requests.Response]]:
         if self.has_reached_max_concurrency_attempt():
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,35 +21,55 @@
         return Template(
             """query {
                     node(id: "$job_id") {
                         ... on BulkOperation {
                             id
                             status
                             errorCode
+                            createdAt
                             objectCount
                             fileSize
                             url
                             partialDataUrl
                         }
                     }
                 }"""
         ).substitute(job_id=bulk_job_id)
 
     @staticmethod
+    def cancel(bulk_job_id: str) -> str:
+        return Template(
+            """mutation {
+                bulkOperationCancel(id: "$job_id") {
+                    bulkOperation {
+                        id
+                        status
+                        createdAt
+                    }
+                    userErrors {
+                        field
+                        message
+                    }
+                }
+            }"""
+        ).substitute(job_id=bulk_job_id)
+
+    @staticmethod
     def prepare(query: str) -> str:
         bulk_template = Template(
             '''mutation {
                 bulkOperationRunQuery(
                     query: """
                     $query
                     """
                 ) {
                     bulkOperation {
                         id
                         status
+                        createdAt
                     }
                     userErrors {
                         field
                         message
                     }
                 }
             }'''
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/source.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/spec.json` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/streams/base_streams.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 
 class IncrementalShopifyStream(ShopifyStream, ABC):
     # Setting the check point interval to the limit of the records output
     state_checkpoint_interval = 250
     # guarantee for the NestedSubstreams to emit the STATE
     # when we have the abnormal STATE distance between Parent and Substream
-    at_least_one_record_output = False
+    filter_by_state_checkpoint = False
 
     # Setting the default cursor field for all streams
     cursor_field = "updated_at"
     deleted_cursor_field = "deleted_at"
 
     @property
     def default_state_comparison_value(self) -> Union[int, str]:
@@ -209,70 +209,52 @@
         # If there is a next page token then we should only send pagination-related parameters.
         if not next_page_token:
             params["order"] = f"{self.order_field} asc"
             if stream_state:
                 params[self.filter_field] = stream_state.get(self.cursor_field)
         return params
 
-    def should_emit_at_least_one_record(self, processed_records: int) -> bool:
-        return self.at_least_one_record_output and processed_records >= self.state_checkpoint_interval
-
-    def emit_duplicated_record_message(
-        self,
-        record_pk: Union[str, int],
-        state_value: Optional[Any] = None,
-        record_value: Optional[Any] = None,
-    ) -> None:
-        state_message = f"The STATE value `{state_value}` is bigger than the record observed `{record_value}`"
-        duplicated_record_message = f"Emitting duplicated record with PK: `{record_pk}` as a checkpoint"
-        self.logger.info(f"Stream `{self.name}`. {state_message}. {duplicated_record_message}.")
+    def should_checkpoint(self, index: int) -> bool:
+        return self.filter_by_state_checkpoint and index >= self.state_checkpoint_interval
 
     # Parse the `stream_slice` with respect to `stream_state` for `Incremental refresh`
     # cases where we slice the stream, the endpoints for those classes don't accept any other filtering,
     # but they provide us with the updated_at field in most cases, so we used that as incremental filtering during the order slicing.
     def filter_records_newer_than_state(
-        self, stream_state: Optional[Mapping[str, Any]] = None, records_slice: Optional[Iterable[Mapping]] = None
+        self,
+        stream_state: Optional[Mapping[str, Any]] = None,
+        records_slice: Optional[Iterable[Mapping]] = None,
     ) -> Iterable:
         # Getting records >= state
-        processed_records = 0
-        emitted_records = 0
         if stream_state:
             state_value = stream_state.get(self.cursor_field, self.default_state_comparison_value)
-            for record in records_slice:
-                processed_records += 1
+            for index, record in enumerate(records_slice, 1):
                 if self.cursor_field in record:
                     record_value = record.get(self.cursor_field, self.default_state_comparison_value)
                     if record_value:
                         if record_value >= state_value:
                             yield record
-                            emitted_records += 1
                         else:
-                            if self.should_emit_at_least_one_record(processed_records):
-                                self.emit_duplicated_record_message(
-                                    record_pk=record.get(self.primary_key),
-                                    state_value=state_value,
-                                    record_value=record_value,
+                            if self.should_checkpoint(index):
+                                self.logger.info(
+                                    f"Stream `{self.name}`. Checkpointing: {{PK: '{record.get(self.primary_key)}', cursor: '{record_value}'}}."
                                 )
                                 yield record
-                                emitted_records += 1
                     else:
                         # old entities could have cursor field in place, but set to null
                         self.logger.warning(
                             f"Stream `{self.name}`, Record ID: `{record.get(self.primary_key)}` cursor value is: {record_value}, record is emitted without state comparison"
                         )
                         yield record
-                        emitted_records += 1
                 else:
                     # old entities could miss the cursor field
                     self.logger.warning(
                         f"Stream `{self.name}`, Record ID: `{record.get(self.primary_key)}` missing cursor field: {self.cursor_field}, record is emitted without state comparison"
                     )
                     yield record
-                    emitted_records += 1
-            self.logger.info(f"Stream `{self.name}`. Emitted Records / Processed Records: {emitted_records}/{processed_records}.")
         else:
             yield from records_slice
 
 
 class IncrementalShopifySubstream(IncrementalShopifyStream):
     """
     IncrementalShopifySubstream - provides slicing functionality for streams using parts of data from parent stream.
@@ -451,15 +433,15 @@
 
     ::  @ nested_entity - the name of the nested entity inside of parent stream, helps to reduce the number of
           API Calls, if present, see `OrderRefunds` or `Fulfillments` streams for more info.
     """
 
     # Setting the check point interval to the limit of the records output
     state_checkpoint_interval = 50
-    at_least_one_record_output = True
+    filter_by_state_checkpoint = True
     data_field = None
     parent_stream_class: Union[ShopifyStream, IncrementalShopifyStream] = None
     mutation_map: Mapping[str, Any] = None
     nested_entity = None
 
     @property
     def availability_strategy(self) -> None:
@@ -752,21 +734,33 @@
     def get_state_value(self, stream_state: Mapping[str, Any] = None) -> Optional[Union[str, int]]:
         if stream_state:
             return self.get_stream_state_value(stream_state)
         else:
             # for majority of cases we fallback to start_date, otherwise.
             return self.config.get("start_date")
 
+    def job_size_reduce_next_slice(self) -> None:
+        # revert the flag
+        self.job_manager.job_should_revert_slice = False
+        # re-adjust Job Size
+        self.job_manager.reduce_job_size()
+
     @stream_state_cache.cache_stream_state
     def stream_slices(self, stream_state: Optional[Mapping[str, Any]] = None, **kwargs) -> Iterable[Optional[Mapping[str, Any]]]:
         if self.filter_field:
             state = self.get_state_value(stream_state)
             start = pdm.parse(state)
             end = pdm.now()
             while start < end:
+                # When the Job is CANCELED intentionally,
+                # we will revert the slice start for the period, and retry with the smaller job size
+                if self.job_manager.is_long_running_job:
+                    start = start.subtract(days=self.slice_interval_in_days)
+                    self.job_size_reduce_next_slice()
+
                 slice_end = start.add(days=self.slice_interval_in_days)
                 # check end period is less than now() or now() is applied otherwise.
                 slice_end = slice_end if slice_end < end else end
                 # making pre-defined sliced query to pass it directly
                 prepared_query = self.query.get(self.filter_field, start.to_rfc3339_string(), slice_end.to_rfc3339_string())
                 self.logger.info(
                     f"Stream: `{self.name}` requesting BULK Job for period: {start} -- {slice_end}. Slice size: `P{round(self.slice_interval_in_days, 1)}D`."
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/transform.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/source_shopify/utils.py` & `airbyte_source_shopify-2.0.5.dev202404132146/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404121134/PKG-INFO` & `airbyte_source_shopify-2.0.5.dev202404132146/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.5.dev202404121134
+Version: 2.0.5.dev202404132146
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

