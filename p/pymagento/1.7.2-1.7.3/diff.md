# Comparing `tmp/pymagento-1.7.2.tar.gz` & `tmp/pymagento-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.7.2.tar", max compression
+gzip compressed data, was "pymagento-1.7.3.tar", max compression
```

## Comparing `pymagento-1.7.2.tar` & `pymagento-1.7.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-07-04 08:43:16.110479 pymagento-1.7.2/LICENSE
--rw-r--r--   0        0        0      908 2023-07-04 08:43:16.110479 pymagento-1.7.2/README.md
--rw-r--r--   0        0        0     1189 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/__init__.py
--rw-r--r--   0        0        0     4773 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/batches.py
--rw-r--r--   0        0        0    36798 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/client.py
--rw-r--r--   0        0        0     1768 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/queries.py
--rw-r--r--   0        0        0      357 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/types.py
--rw-r--r--   0        0        0       22 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/version.py
--rw-r--r--   0        0        0     1219 2023-07-04 08:43:16.110479 pymagento-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-10 08:43:14.596912 pymagento-1.7.3/LICENSE
+-rw-r--r--   0        0        0      908 2023-07-10 08:43:14.596912 pymagento-1.7.3/README.md
+-rw-r--r--   0        0        0     1189 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/batches.py
+-rw-r--r--   0        0        0    37320 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/types.py
+-rw-r--r--   0        0        0       22 2023-07-10 08:43:14.596912 pymagento-1.7.3/magento/version.py
+-rw-r--r--   0        0        0     1219 2023-07-10 08:43:14.596912 pymagento-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.3/PKG-INFO
```

### Comparing `pymagento-1.7.2/LICENSE` & `pymagento-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/README.md` & `pymagento-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/magento/__init__.py` & `pymagento-1.7.3/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/magento/attributes.py` & `pymagento-1.7.3/magento/attributes.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/magento/batches.py` & `pymagento-1.7.3/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/magento/client.py` & `pymagento-1.7.3/magento/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 class Magento(APISession):
     """
     Client for the Magento API.
     """
     # default batch size for paginated requests
     # Note increasing it doesn’t create a significant time improvement.
-    # For example, in one test on Bixoto production in 2021, getting 2k products using a page size of 1k took 28s.
+    # For example, in one test on Bixoto in 2021, getting 2k products using a page size of 1k took 28s.
     # The same query with a page size of 2k still took 26s.
     PAGE_SIZE = 1000
 
     # default is 4 hours for admin tokens (the ones we use)
     TOKEN_LIFETIME = timedelta(hours=3)
 
     def __init__(self,
@@ -142,17 +142,17 @@
 
     def delete_attribute(self, attribute_code: str, **kwargs):
         return self.delete_api(f"/V1/products/attributes/{escape_path(attribute_code)}", **kwargs)
 
     # Attribute Sets
     # ==============
 
-    def get_attribute_sets(self, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
+    def get_attribute_sets(self, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all attribute sets (generator)."""
-        return self.get_paginated("/V1/eav/attribute-sets/list", limit=limit, **kwargs)
+        return self.get_paginated("/V1/eav/attribute-sets/list", query=query, limit=limit, **kwargs)
 
     def get_attribute_set_attributes(self, attribute_set_id: int, **kwargs):
         """Get all attributes for the given attribute set id."""
         return self.get_json_api(f"/V1/products/attribute-sets/{attribute_set_id}/attributes", **kwargs)
 
     def assign_attribute_set_attribute(self, attribute_set_id: int, attribute_group_id: int, attribute_code: str,
                                        sort_order: int = 0, **kwargs):
@@ -186,29 +186,26 @@
         Get the status of an async/bulk operation.
         """
         return self.get_api(f"/V1/bulk/{escape_path(bulk_uuid)}/status", throw=True).json()
 
     # Carts
     # =====
 
-    def get_carts(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_carts(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all carts (generator)."""
-        return self.get_paginated("/V1/carts/search", query=query, limit=limit)
+        return self.get_paginated("/V1/carts/search", query=query, limit=limit, **kwargs)
 
     # Categories
     # ==========
 
-    def get_categories(self, query: Query = None) -> Iterable[Category]:
+    def get_categories(self, query: Query = None, limit=-1, **kwargs) -> Iterable[Category]:
         """
         Yield all categories.
-
-        :param query:
-        :return:
         """
-        return self.get_paginated("/V1/categories/list", query=query)
+        return self.get_paginated("/V1/categories/list", query=query, limit=limit, **kwargs)
 
     def get_category(self, category_id: PathId) -> Optional[Category]:
         """
         Return a category given its id.
 
         :param category_id:
         :return:
@@ -243,43 +240,43 @@
         Create a new category.
         """
         return self.post_api("/V1/categories", json={"category": category}, throw=throw)
 
     # CMS
     # ===
 
-    def get_cms_pages(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_cms_pages(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all CMS pages (generator)."""
-        return self.get_paginated("/V1/cmsPage/search", query=query, limit=limit)
+        return self.get_paginated("/V1/cmsPage/search", query=query, limit=limit, **kwargs)
 
-    def get_cms_blocks(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_cms_blocks(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all CMS blocks (generator)."""
-        return self.get_paginated("/V1/cmsBlock/search", query=query, limit=limit)
+        return self.get_paginated("/V1/cmsBlock/search", query=query, limit=limit, **kwargs)
 
     # Coupons
     # =======
 
-    def get_coupons(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_coupons(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all coupons (generator)."""
-        return self.get_paginated("/V1/coupons/search", query=query, limit=limit)
+        return self.get_paginated("/V1/coupons/search", query=query, limit=limit, **kwargs)
 
     # Customers
     # =========
 
-    def get_customers(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_customers(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all customers (generator)."""
-        return self.get_paginated("/V1/customers/search", query=query, limit=limit)
+        return self.get_paginated("/V1/customers/search", query=query, limit=limit, **kwargs)
 
     def get_customer(self, customer_id: int) -> dict:
         """Return a single customer."""
         return self.get_api(f"/V1/customers/{customer_id}", throw=True).json()
 
-    def get_customer_groups(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_customer_groups(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all customer groups (generator)."""
-        return self.get_paginated("/V1/customerGroups/search", query=query, limit=limit)
+        return self.get_paginated("/V1/customerGroups/search", query=query, limit=limit, **kwargs)
 
     # Invoices
     # ========
 
     def create_order_invoice(self, order_id: PathId, payload: Optional[dict] = None, notify=True):
         """
         Create an invoice for an order.
@@ -305,17 +302,17 @@
 
     def get_invoice_by_increment_id(self, increment_id: str) -> Optional[MagentoEntity]:
         query = make_field_value_query("increment_id", increment_id)
         for invoice in self.get_invoices(query=query, limit=1):
             return invoice
         return None
 
-    def get_invoices(self, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_invoices(self, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all invoices (generator)."""
-        return self.get_paginated("/V1/invoices", query=query, limit=limit)
+        return self.get_paginated("/V1/invoices", query=query, limit=limit, **kwargs)
 
     def get_order_invoices(self, order_id: Union[int, str]):
         """Get invoices for the given order id."""
         return self.get_invoices(query=make_field_value_query("order_id", order_id))
 
     # Orders
     # ======
@@ -336,33 +333,34 @@
         :param query: optional query.
         :param retry: max retries count
         :return: generator of orders
         """
         if status:
             query = make_field_value_query("status", status, condition_type=status_condition_type)
 
-        return self.get_paginated("/V1/orders", limit=limit, query=query, retry=retry)
+        return self.get_paginated("/V1/orders", query=query, limit=limit, retry=retry)
 
     def get_last_orders(self, limit=10) -> List[Order]:
         """Return a list of the last orders (default: 10)."""
         query = make_search_query([], sort_orders=[("increment_id", "DESC")])
         return list(self.get_orders(query=query, limit=limit))
 
-    def get_orders_items(self, *, sku: Optional[str] = None, query: Query = None, **kwargs):
+    def get_orders_items(self, *, sku: Optional[str] = None, query: Query = None, limit=-1, **kwargs):
         """
         Return orders items.
 
         :param sku: filter orders items on SKU. This is a shortcut for ``query=make_field_value_query("sku", sku)``.
         :param query: optional query. This take precedence over ``sku``.
+        :param limit:
         :return:
         """
         if query is None and sku is not None:
             query = make_field_value_query("sku", sku)
 
-        return self.get_paginated("/V1/orders/items", query=query, **kwargs)
+        return self.get_paginated("/V1/orders/items", query=query, limit=limit, **kwargs)
 
     def get_order(self, order_id: str, throw=True) -> Optional[Order]:
         """
         Get an order given its (entity) id.
         """
         return self.get_api(f"/V1/orders/{order_id}", throw=throw).json()
 
@@ -397,17 +395,17 @@
             payload["ext_order_id"] = external_order_id
 
         return self.save_order(payload)
 
     # Credit Memos
     # ============
 
-    def get_credit_memos(self, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_credit_memos(self, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all credit memos (generator)."""
-        return self.get_paginated("/V1/creditmemos", query=query, limit=limit)
+        return self.get_paginated("/V1/creditmemos", query=query, limit=limit, **kwargs)
 
     # Prices
     # ======
 
     # Base Prices
     # -----------
 
@@ -487,15 +485,15 @@
         Return a generator of all products.
 
         :param limit: -1 for unlimited.
         :param query:
         :param retry:
         :return:
         """
-        return cast(Iterator[Product], self.get_paginated("/V1/products/", limit=limit, query=query, retry=retry))
+        return cast(Iterator[Product], self.get_paginated("/V1/products/", query=query, limit=limit, retry=retry))
 
     def get_products_types(self) -> Sequence[MagentoEntity]:
         """Get available product types."""
         return self.get_json_api("/V1/product/types")
 
     def get_product(self, sku: Sku) -> Optional[Product]:
         """
@@ -746,51 +744,51 @@
         Shortcut for `.get_products_attribute_options("manufacturer")`.
         """
         return self.get_products_attribute_options("manufacturer")
 
     # Sales Rules
     # ===========
 
-    def get_sales_rules(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_sales_rules(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all sales rules (generator)."""
-        return self.get_paginated("/V1/salesRules/search", query=query, limit=limit)
+        return self.get_paginated("/V1/salesRules/search", query=query, limit=limit, **kwargs)
 
     # Shipments
     # =========
 
-    def get_shipments(self, **kwargs) -> Iterable[MagentoEntity]:
+    def get_shipments(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Return shipments."""
-        return self.get_paginated("/V1/shipments", **kwargs)
+        return self.get_paginated("/V1/shipments", query=query, limit=limit, **kwargs)
 
     def ship_order(self, order_id: PathId, payload: MagentoEntity):
         """
         Ship an order.
         """
         return self.post_api(f"/V1/order/{order_id}/ship", json=payload)
 
     def get_order_shipments(self, order_id: Union[int, str]):
         """Get shipments for the given order id."""
         return self.get_shipments(query=make_field_value_query("order_id", order_id))
 
     # Stock
     # =====
 
-    def get_stock_source_links(self, query: Query = None) -> Iterable[MagentoEntity]:
-        return self.get_paginated("/V1/inventory/stock-source-links", query=query)
+    def get_stock_source_links(self, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
+        return self.get_paginated("/V1/inventory/stock-source-links", query=query, limit=limit, **kwargs)
 
     # Sources
     # =======
 
-    def get_sources(self, query: Query = None) -> Iterable[MagentoEntity]:
+    def get_sources(self, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """
         Get all sources.
 
         https://adobe-commerce.redoc.ly/2.4.6-admin/tag/inventorysources#operation/GetV1InventorySources
         """
-        return self.get_paginated("/V1/inventory/sources", query=query)
+        return self.get_paginated("/V1/inventory/sources", query=query, limit=limit, **kwargs)
 
     def get_source(self, source_code: str) -> Optional[MagentoEntity]:
         """
         Get a single source, or `None` if it doesn’t exist.
 
         https://adobe-commerce.redoc.ly/2.4.6-admin/tag/inventorysourcessourceCode#operation/GetV1InventorySourcesSourceCode
         """
@@ -806,15 +804,16 @@
 
     # Source Items
     # ============
 
     def get_source_items(self, source_code: Optional[str] = None, sku: Optional[str] = None,
                          *,
                          skus: Optional[Iterable[str]] = None,
-                         query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+                         query: Query = None, limit=-1,
+                         **kwargs) -> Iterable[MagentoEntity]:
         """
         Return a generator of all source items.
 
         :param source_code: optional source_code to filter on. This takes precedence over the query parameter.
         :param sku: optional SKU to filter on. This takes precedence over the query and the skus parameter.
         :param skus: optional SKUs list to filter on. This takes precedence of the query parameter.
         :param query: optional query.
@@ -828,15 +827,15 @@
             if sku:
                 filter_groups.append([("sku", sku, "eq")])
             elif skus:
                 filter_groups.append([("sku", ",".join(skus), "in")])
 
             query = make_search_query(filter_groups)
 
-        return self.get_paginated("/V1/inventory/source-items", limit=limit, query=query)
+        return self.get_paginated("/V1/inventory/source-items", query=query, limit=limit, **kwargs)
 
     def save_source_items(self, source_items: Sequence[SourceItem]):
         """
         Save a sequence of source-items. Return None if the sequence is empty.
 
         :param source_items:
         :return:
@@ -872,32 +871,32 @@
 
         if source_items:
             return self.delete_source_items(source_items)
 
     # Taxes
     # =====
 
-    def get_tax_classes(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_tax_classes(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all tax classes (generator)."""
-        return self.get_paginated("/V1/taxClasses/search", query=query, limit=limit)
+        return self.get_paginated("/V1/taxClasses/search", query=query, limit=limit, **kwargs)
 
-    def get_tax_rates(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_tax_rates(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all tax rates (generator)."""
-        return self.get_paginated("/V1/taxRates/search", query=query, limit=limit)
+        return self.get_paginated("/V1/taxRates/search", query=query, limit=limit, **kwargs)
 
-    def get_tax_rules(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_tax_rules(self, *, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all tax rules (generator)."""
-        return self.get_paginated("/V1/taxRules/search", query=query, limit=limit)
+        return self.get_paginated("/V1/taxRules/search", query=query, limit=limit, **kwargs)
 
     # Modules
     # =======
 
-    def get_modules(self, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
+    def get_modules(self, query: Query = None, limit=-1, **kwargs) -> Iterable[MagentoEntity]:
         """Get all enabled modules (generator)."""
-        return self.get_paginated("/V1/modules", query=query, limit=limit)
+        return self.get_paginated("/V1/modules", query=query, limit=limit, **kwargs)
 
     # Internals
     # =========
 
     def request_api(self, method: str, path: str, *args, async_bulk=False, throw=False, retry=0, **kwargs):
         """
         Equivalent of .request() that prefixes the path with the base API URL.
```

### Comparing `pymagento-1.7.2/magento/exceptions.py` & `pymagento-1.7.3/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/magento/order_helpers.py` & `pymagento-1.7.3/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/magento/queries.py` & `pymagento-1.7.3/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.2/pyproject.toml` & `pymagento-1.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.7.2"
+version = "1.7.3"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.7.2/PKG-INFO` & `pymagento-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.7.2
+Version: 1.7.3
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

