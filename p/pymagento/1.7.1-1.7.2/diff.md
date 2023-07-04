# Comparing `tmp/pymagento-1.7.1.tar.gz` & `tmp/pymagento-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymagento-1.7.1.tar", max compression
+gzip compressed data, was "pymagento-1.7.2.tar", max compression
```

## Comparing `pymagento-1.7.1.tar` & `pymagento-1.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-06 16:19:28.936593 pymagento-1.7.1/LICENSE
--rw-r--r--   0        0        0      908 2023-06-06 16:19:28.936593 pymagento-1.7.1/README.md
--rw-r--r--   0        0        0     1189 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/__init__.py
--rw-r--r--   0        0        0     4773 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/attributes.py
--rw-r--r--   0        0        0     3849 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/batches.py
--rw-r--r--   0        0        0    35824 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/client.py
--rw-r--r--   0        0        0     1768 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/exceptions.py
--rw-r--r--   0        0        0      963 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/order_helpers.py
--rw-r--r--   0        0        0        0 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/py.typed
--rw-r--r--   0        0        0     3374 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/queries.py
--rw-r--r--   0        0        0      357 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/types.py
--rw-r--r--   0        0        0       22 2023-06-06 16:19:28.936593 pymagento-1.7.1/magento/version.py
--rw-r--r--   0        0        0     1219 2023-06-06 16:19:28.936593 pymagento-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-04 08:43:16.110479 pymagento-1.7.2/LICENSE
+-rw-r--r--   0        0        0      908 2023-07-04 08:43:16.110479 pymagento-1.7.2/README.md
+-rw-r--r--   0        0        0     1189 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/__init__.py
+-rw-r--r--   0        0        0     4773 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/attributes.py
+-rw-r--r--   0        0        0     3849 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/batches.py
+-rw-r--r--   0        0        0    36798 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/client.py
+-rw-r--r--   0        0        0     1768 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/exceptions.py
+-rw-r--r--   0        0        0      963 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/order_helpers.py
+-rw-r--r--   0        0        0        0 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/py.typed
+-rw-r--r--   0        0        0     3374 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/queries.py
+-rw-r--r--   0        0        0      357 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/types.py
+-rw-r--r--   0        0        0       22 2023-07-04 08:43:16.110479 pymagento-1.7.2/magento/version.py
+-rw-r--r--   0        0        0     1219 2023-07-04 08:43:16.110479 pymagento-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1727 1970-01-01 00:00:00.000000 pymagento-1.7.2/PKG-INFO
```

### Comparing `pymagento-1.7.1/LICENSE` & `pymagento-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/README.md` & `pymagento-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/magento/__init__.py` & `pymagento-1.7.2/magento/__init__.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/magento/attributes.py` & `pymagento-1.7.2/magento/attributes.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/magento/batches.py` & `pymagento-1.7.2/magento/batches.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/magento/client.py` & `pymagento-1.7.2/magento/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from magento.types import Product, SourceItem, Sku, Category, MediaEntry, MagentoEntity, Order, PathId
 from magento.version import __version__
 from magento.exceptions import MagentoException, MagentoAssertionError
 
 from magento.queries import Query, make_search_query, make_field_value_query
 
 __all__ = (
-    'Magento',
+    "Magento",
 )
 
-USER_AGENT = f'Bixoto/PyMagento {__version__} +git.io/JDp0h'
+USER_AGENT = f"Bixoto/PyMagento {__version__} +git.io/JDp0h"
 
 DEFAULT_ATTRIBUTE_DICT = {
     "apply_to": [],
     "backend_type": "int",
     "custom_attributes": [],
     "entity_type_id": "4",
     "extension_attributes": {},
@@ -59,15 +59,15 @@
 def raise_for_response(response: requests.Response):
     """
     Equivalent of requests.Response#raise_for_status with some Magento specifics.
     """
     if response.ok:
         return
 
-    if response.text and response.text[0] == '{':
+    if response.text and response.text[0] == "{":
         try:
             body = response.json()
         except (ValueError, JSONDecodeError):
             pass
         else:
             if isinstance(body, dict) and "message" in body:
                 raise MagentoException(body["message"], parameters=body.get("parameters"),
@@ -123,26 +123,26 @@
         if base_url is None:
             raise RuntimeError("Missing API base URL")
 
         super().__init__(base_url=base_url, user_agent=user_agent, read_only=read_only, **kwargs)
 
         self.scope = scope
         self.logger = logger
-        self.headers['Authorization'] = f"Bearer {token}"
+        self.headers["Authorization"] = f"Bearer {token}"
 
     # Attributes
     # ==========
 
     def save_attribute(self, attribute: MagentoEntity, *, with_defaults=True, throw=True, **kwargs) -> MagentoEntity:
         if with_defaults:
             base = DEFAULT_ATTRIBUTE_DICT.copy()
             base.update(attribute)
             attribute = base
 
-        return self.post_api('/V1/products/attributes', json={"attribute": attribute}, throw=throw, **kwargs).json()
+        return self.post_api("/V1/products/attributes", json={"attribute": attribute}, throw=throw, **kwargs).json()
 
     def delete_attribute(self, attribute_code: str, **kwargs):
         return self.delete_api(f"/V1/products/attributes/{escape_path(attribute_code)}", **kwargs)
 
     # Attribute Sets
     # ==============
 
@@ -181,15 +181,15 @@
     # Bulk Operations
     # ===============
 
     def get_bulk_status(self, bulk_uuid: str) -> MagentoEntity:
         """
         Get the status of an async/bulk operation.
         """
-        return self.get_api(f'/V1/bulk/{escape_path(bulk_uuid)}/status', throw=True).json()
+        return self.get_api(f"/V1/bulk/{escape_path(bulk_uuid)}/status", throw=True).json()
 
     # Carts
     # =====
 
     def get_carts(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
         """Get all carts (generator)."""
         return self.get_paginated("/V1/carts/search", query=query, limit=limit)
@@ -200,15 +200,15 @@
     def get_categories(self, query: Query = None) -> Iterable[Category]:
         """
         Yield all categories.
 
         :param query:
         :return:
         """
-        return self.get_paginated('/V1/categories/list', query=query)
+        return self.get_paginated("/V1/categories/list", query=query)
 
     def get_category(self, category_id: PathId) -> Optional[Category]:
         """
         Return a category given its id.
 
         :param category_id:
         :return:
@@ -231,22 +231,22 @@
         """
         Update a category.
 
         :param category_id:
         :param category_data: (partial) category data to update
         :return: updated category
         """
-        return cast(Category, self.put_api(f'/V1/categories/{category_id}',
+        return cast(Category, self.put_api(f"/V1/categories/{category_id}",
                                            json={"category": category_data}, throw=True).json())
 
     def create_category(self, category: Category, throw=False):
         """
         Create a new category.
         """
-        return self.post_api('/V1/categories', json={"category": category}, throw=throw)
+        return self.post_api("/V1/categories", json={"category": category}, throw=throw)
 
     # CMS
     # ===
 
     def get_cms_pages(self, *, query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
         """Get all CMS pages (generator)."""
         return self.get_paginated("/V1/cmsPage/search", query=query, limit=limit)
@@ -360,36 +360,36 @@
 
         return self.get_paginated("/V1/orders/items", query=query, **kwargs)
 
     def get_order(self, order_id: str, throw=True) -> Optional[Order]:
         """
         Get an order given its (entity) id.
         """
-        return self.get_api(f'/V1/orders/{order_id}', throw=throw).json()
+        return self.get_api(f"/V1/orders/{order_id}", throw=throw).json()
 
     def get_order_by_increment_id(self, increment_id: str) -> Optional[Order]:
         """
         Get an order given its increment id. Return ``None`` if the order doesn’t exist.
 
         :param increment_id:
         :return:
         """
         query = make_field_value_query("increment_id", increment_id)
         for order in self.get_orders(query=query, limit=1):
             return order
         return None
 
     def hold_order(self, order_id: str, **kwargs):
-        return self.post_api(f'/V1/orders/{order_id}/hold', **kwargs)
+        return self.post_api(f"/V1/orders/{order_id}/hold", **kwargs)
 
     def unhold_order(self, order_id: str, **kwargs):
-        return self.post_api(f'/V1/orders/{order_id}/unhold', **kwargs)
+        return self.post_api(f"/V1/orders/{order_id}/unhold", **kwargs)
 
     def save_order(self, order: Order):
-        return self.post_api(f'/V1/orders', json={"entity": order})
+        return self.post_api(f"/V1/orders", json={"entity": order})
 
     def set_order_status(self, order: Order, status: str, *, external_order_id: Optional[str] = None):
         payload = {
             "entity_id": order["entity_id"],
             "status": status,
             "increment_id": order["increment_id"],  # we need to repeat increment_id, otherwise it is regenerated
         }
@@ -437,15 +437,15 @@
     def get_special_prices(self, skus: Sequence[Sku]) -> List[MagentoEntity]:
         """
         Get special prices for a sequence of SKUs.
 
         :param skus:
         :return:
         """
-        return self.post_api('/V1/products/special-price-information',
+        return self.post_api("/V1/products/special-price-information",
                              json={"skus": skus}, throw=True, bypass_read_only=True).json()
 
     def save_special_prices(self, special_prices: Sequence[MagentoEntity]):
         """
         Save a sequence of special prices.
 
         Example:
@@ -454,24 +454,24 @@
             >>> special_price = {"store_id": 0, "sku": "W1033", "price": 2.99, \
                                  "price_from": price_from, "price_to": price_to}
             >>> self.save_special_prices([special_price])
 
         :param special_prices: Special prices to save.
         :return:
         """
-        return self.post_api('/V1/products/special-price', json={"prices": special_prices})
+        return self.post_api("/V1/products/special-price", json={"prices": special_prices})
 
     def delete_special_prices(self, special_prices: Sequence[MagentoEntity]):
         """
         Delete a sequence of special prices.
 
         :param special_prices:
         :return:
         """
-        return self.post_api('/V1/products/special-price-delete', json={"prices": special_prices})
+        return self.post_api("/V1/products/special-price-delete", json={"prices": special_prices})
 
     def delete_special_prices_by_sku(self, skus: Sequence[Sku]):
         """
         Equivalent of `delete_special_prices(get_special_prices(skus))`.
 
         :param skus:
         :return:
@@ -491,24 +491,24 @@
         :param retry:
         :return:
         """
         return cast(Iterator[Product], self.get_paginated("/V1/products/", limit=limit, query=query, retry=retry))
 
     def get_products_types(self) -> Sequence[MagentoEntity]:
         """Get available product types."""
-        return self.get_json_api('/V1/product/types')
+        return self.get_json_api("/V1/product/types")
 
     def get_product(self, sku: Sku) -> Optional[Product]:
         """
         Get a single product. Return ``None`` if it doesn’t exist.
 
         :param sku: SKU of the product
         :return:
         """
-        return self.get_json_api(f'/V1/products/{escape_path(sku)}')
+        return self.get_json_api(f"/V1/products/{escape_path(sku)}")
 
     def get_product_by_id(self, product_id: int) -> Optional[Product]:
         """
         Get a product given its id. Return ``None`` if the product doesn’t exist.
 
         :param product_id: ID of the product
         :return:
@@ -542,46 +542,46 @@
     def get_product_medias(self, sku: Sku) -> Sequence[MediaEntry]:
         """
         Get the list of gallery entries associated with the given product.
 
         :param sku: SKU of the product.
         :return:
         """
-        return self.get_json_api(f'/V1/products/{escape_path(sku)}/media')
+        return self.get_json_api(f"/V1/products/{escape_path(sku)}/media")
 
     def get_product_media(self, sku: Sku, entry_id: PathId) -> MediaEntry:
         """
         Return a gallery entry.
 
         :param sku: SKU of the product.
         :param entry_id:
         :return:
         """
-        return self.get_json_api(f'/V1/products/{escape_path(sku)}/media/{entry_id}')
+        return self.get_json_api(f"/V1/products/{escape_path(sku)}/media/{entry_id}")
 
     def save_product_media(self, sku: Sku, media_entry: MediaEntry):
-        return self.post_api(f'/V1/products/{escape_path(sku)}/media', json={"entry": media_entry}, throw=True).json()
+        return self.post_api(f"/V1/products/{escape_path(sku)}/media", json={"entry": media_entry}, throw=True).json()
 
     def delete_product_media(self, sku: Sku, media_id: PathId, throw=False):
-        return self.delete_api(f'/V1/products/{escape_path(sku)}/media/{media_id}', throw=throw)
+        return self.delete_api(f"/V1/products/{escape_path(sku)}/media/{media_id}", throw=throw)
 
     def save_product(self, product, *, save_options: Optional[bool] = None) -> Product:
         """
         Save a product.
 
         :param product: (partial) product to save.
         :param save_options: set the `saveOptions` attribute.
         :return:
         """
         payload: JSONDict = {"product": product}
         if save_options is not None:
             payload["saveOptions"] = save_options
 
         # throw=False so the log is printed before we raise
-        resp = self.post_api('/V1/products', json=payload, throw=False)
+        resp = self.post_api("/V1/products", json=payload, throw=False)
         if self.logger:
             self.logger.debug("Save product response: %s", resp.text)
         raise_for_response(resp)
         return cast(Product, resp.json())
 
     def update_product(self, sku: Sku, product: Product, *, save_options: Optional[bool] = None) -> Product:
         """
@@ -599,28 +599,28 @@
         :param save_options: set the `saveOptions` attribute.
         :return: updated product
         """
         payload: JSONDict = {"product": product}
         if save_options is not None:
             payload["saveOptions"] = save_options
 
-        return cast(Product, self.put_api(f'/V1/products/{escape_path(sku)}', json=payload, throw=True).json())
+        return cast(Product, self.put_api(f"/V1/products/{escape_path(sku)}", json=payload, throw=True).json())
 
     def delete_product(self, sku: Sku, skip_missing=False, throw=True, **kwargs) -> bool:
         """
         Delete a product given its SKU.
 
         :param sku:
-        :param skip_missing: if true, don't raise if the product is missing, and return False.
+        :param skip_missing: if true, don’t raise if the product is missing, and return False.
         :param throw: throw on error response
         :param kwargs: keyword arguments passed to all underlying methods.
         :return: a boolean indicating success.
         """
         try:
-            response = self.delete_api(f'/V1/products/{escape_path(sku)}', throw=throw, **kwargs)
+            response = self.delete_api(f"/V1/products/{escape_path(sku)}", throw=throw, **kwargs)
         except (HTTPError, MagentoException) as e:
             if skip_missing and e.response is not None and e.response.status_code == 404:
                 return False
             raise
 
         # "Will returned True if deleted"
         # https://magento.redoc.ly/2.3.6-admin/tag/productssku#operation/catalogProductRepositoryV1DeleteByIdDelete
@@ -631,29 +631,29 @@
         Update multiple products using the async bulk API.
 
         Example:
             >>> Magento().async_update_products([{"sku": "SK123", "name": "Abc"}), {"sku": "SK4", "name": "Def"}])
 
         See https://devdocs.magento.com/guides/v2.4/rest/bulk-endpoints.html
 
-        :param product_updates: sequence of product data dicts. They MUST contain an 'sku' key.
+        :param product_updates: sequence of product data dicts. They MUST contain an `sku` key.
         :return:
         """
         payload = [{"product": product_update} for product_update in product_updates]
-        return self.put_api('/V1/products/bySku', json=payload, throw=True, async_bulk=True).json()
+        return self.put_api("/V1/products/bySku", json=payload, throw=True, async_bulk=True).json()
 
     def set_product_stock_item(self, sku: Sku, quantity: int, is_in_stock=1):
         """
         :param sku:
         :param quantity:
         :param is_in_stock:
         :return: requests.Response
         """
         payload = {"stockItem": {"qty": quantity, "is_in_stock": is_in_stock}}
-        return self.put_api(f'/V1/products/{escape_path(sku)}/stockItems/1', json=payload, throw=True)
+        return self.put_api(f"/V1/products/{escape_path(sku)}/stockItems/1", json=payload, throw=True)
 
     def get_product_stock_status(self, sku: Sku) -> MagentoEntity:
         """Get stock status for an SKU."""
         return self.get_api(f"/V1/stockStatuses/{escape_path(sku)}", throw=True).json()
 
     def get_product_stock_item(self, sku: Sku) -> MagentoEntity:
         """Get the stock item for an SKU."""
@@ -663,15 +663,15 @@
         """
         Link two products, one as the parent of the other.
 
         :param parent_sku: SKU of the parent product
         :param child_sku: SKU of the child product
         :return: `requests.Response` object
         """
-        return self.post_api(f'/V1/configurable-products/{escape_path(parent_sku)}/child',
+        return self.post_api(f"/V1/configurable-products/{escape_path(parent_sku)}/child",
                              json={"childSku": child_sku}, **kwargs)
 
     def unlink_child_product(self, parent_sku: Sku, child_sku: Sku, **kwargs) -> requests.Response:
         """
         Opposite of link_child_product().
 
         :param parent_sku: SKU of the parent product
@@ -686,42 +686,42 @@
         Save a configurable product option.
 
         :param sku: SKU of the product
         :param option: option to save
         :param throw:
         :return: `requests.Response` object
         """
-        return self.post_api(f'/V1/configurable-products/{escape_path(sku)}/options',
+        return self.post_api(f"/V1/configurable-products/{escape_path(sku)}/options",
                              json={"option": option}, throw=throw)
 
     # Products Attribute Options
     # --------------------------
 
     def get_products_attribute_options(self, attribute_code: str) -> Sequence[Dict[str, str]]:
         """
         Get all options for a products attribute.
 
         :param attribute_code:
         :return: sequence of option dicts.
         """
-        response = self.get_api(f'/V1/products/attributes/{escape_path(attribute_code)}/options', throw=True)
+        response = self.get_api(f"/V1/products/attributes/{escape_path(attribute_code)}/options", throw=True)
         return cast(Sequence[Dict[str, str]], response.json())
 
     def add_products_attribute_option(self, attribute_code: str, option: Dict[str, str]) -> str:
         """
         Add an option to a products attribute.
 
+        https://magento.redoc.ly/2.3.6-admin/#operation/catalogProductAttributeOptionManagementV1AddPost
+
         :param attribute_code:
-        :param option: dict with label/value keys (mandatory).
-          See https://magento.redoc.ly/2.3.6-admin/#operation/catalogProductAttributeOptionManagementV1AddPost
-          for the optional keys.
+        :param option: dict with label/value keys (mandatory)
         :return: new id
         """
         payload = {"option": option}
-        response = self.post_api(f'/V1/products/attributes/{escape_path(attribute_code)}/options',
+        response = self.post_api(f"/V1/products/attributes/{escape_path(attribute_code)}/options",
                                  json=payload, throw=True)
         ret = cast(str, response.json())
 
         if ret.startswith("id_"):
             ret = ret[3:]
 
         return ret
@@ -730,15 +730,15 @@
         """
         Remove an option to a products attribute.
 
         :param attribute_code:
         :param option_id:
         :return: boolean
         """
-        response = self.delete_api(f'/V1/products/attributes/{escape_path(attribute_code)}/options/{option_id}',
+        response = self.delete_api(f"/V1/products/attributes/{escape_path(attribute_code)}/options/{option_id}",
                                    throw=True)
         return cast(bool, response.json())
 
     # Aliases
     # -------
 
     def get_manufacturers(self):
@@ -761,26 +761,53 @@
         """Return shipments."""
         return self.get_paginated("/V1/shipments", **kwargs)
 
     def ship_order(self, order_id: PathId, payload: MagentoEntity):
         """
         Ship an order.
         """
-        return self.post_api(f'/V1/order/{order_id}/ship', json=payload)
+        return self.post_api(f"/V1/order/{order_id}/ship", json=payload)
 
     def get_order_shipments(self, order_id: Union[int, str]):
         """Get shipments for the given order id."""
         return self.get_shipments(query=make_field_value_query("order_id", order_id))
 
     # Stock
     # =====
 
     def get_stock_source_links(self, query: Query = None) -> Iterable[MagentoEntity]:
         return self.get_paginated("/V1/inventory/stock-source-links", query=query)
 
+    # Sources
+    # =======
+
+    def get_sources(self, query: Query = None) -> Iterable[MagentoEntity]:
+        """
+        Get all sources.
+
+        https://adobe-commerce.redoc.ly/2.4.6-admin/tag/inventorysources#operation/GetV1InventorySources
+        """
+        return self.get_paginated("/V1/inventory/sources", query=query)
+
+    def get_source(self, source_code: str) -> Optional[MagentoEntity]:
+        """
+        Get a single source, or `None` if it doesn’t exist.
+
+        https://adobe-commerce.redoc.ly/2.4.6-admin/tag/inventorysourcessourceCode#operation/GetV1InventorySourcesSourceCode
+        """
+        return self.get_json_api(f"/V1/inventory/sources/{escape_path(source_code)}")
+
+    def save_source(self, source: MagentoEntity):
+        """
+        Save a source.
+
+        https://adobe-commerce.redoc.ly/2.4.6-admin/tag/inventorysources/#operation/PostV1InventorySources
+        """
+        return self.post_api("/V1/inventory/sources", json={"source": source}, throw=True).json()
+
     # Source Items
     # ============
 
     def get_source_items(self, source_code: Optional[str] = None, sku: Optional[str] = None,
                          *,
                          skus: Optional[Iterable[str]] = None,
                          query: Query = None, limit=-1) -> Iterable[MagentoEntity]:
@@ -811,31 +838,31 @@
         """
         Save a sequence of source-items. Return None if the sequence is empty.
 
         :param source_items:
         :return:
         """
         if not source_items:
-            return
-        return self.post_api('/V1/inventory/source-items', json={"sourceItems": source_items}, throw=True).json()
+            return None
+        return self.post_api("/V1/inventory/source-items", json={"sourceItems": source_items}, throw=True).json()
 
     def delete_source_items(self, source_items: Iterable[SourceItem], throw=True, **kwargs):
         """
         Delete a sequence of source-items. Only the SKU and the source_code are used.
         Note: Magento returns an error if this is called with empty source_items.
 
         :param source_items:
         :param throw:
         :param kwargs: keyword arguments passed to the underlying POST call.
         :return: requests.Response object
         """
         payload = {
             "sourceItems": [{"sku": s["sku"], "source_code": s["source_code"]} for s in source_items],
         }
-        return self.post_api('/V1/inventory/source-items-delete', json=payload, throw=throw, **kwargs)
+        return self.post_api("/V1/inventory/source-items-delete", json=payload, throw=throw, **kwargs)
 
     def delete_default_source_items(self):
         """
         Delete all source items that have a source_code=default.
 
         :return: requests.Response object if there are default source items, None otherwise.
         """
@@ -887,15 +914,15 @@
         :return:
         """
         assert path.startswith("/V1/")
 
         full_path = f"/rest/{self.scope}"
 
         if async_bulk:
-            full_path += '/async/bulk'
+            full_path += "/async/bulk"
 
         full_path += path
 
         if self.logger:
             self.logger.debug("%s %s", method, full_path)
         r = super().request_api(method, full_path, *args, throw=False, **kwargs)
         while not r.ok and retry > 0:
@@ -937,23 +964,23 @@
         count = 0
 
         while True:
             page_query = query.copy()
             page_query["searchCriteria[currentPage]"] = current_page
 
             res = self.get_api(path, page_query, throw=True, retry=retry).json()
-            items = res.get('items', [])
+            items = res.get("items", [])
             if not items:
                 break
 
             total_count = res["total_count"]
 
             for item in items:
                 if self.logger and count and count % 1000 == 0:
-                    self.logger.debug(f'loaded {count} items')
+                    self.logger.debug(f"loaded {count} items")
                 yield item
                 count += 1
                 if count >= total_count:
                     return
 
                 if is_limited and count >= limit:
                     return
```

### Comparing `pymagento-1.7.1/magento/exceptions.py` & `pymagento-1.7.2/magento/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/magento/order_helpers.py` & `pymagento-1.7.2/magento/order_helpers.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/magento/queries.py` & `pymagento-1.7.2/magento/queries.py`

 * *Files identical despite different names*

### Comparing `pymagento-1.7.1/pyproject.toml` & `pymagento-1.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymagento"
-version = "1.7.1"
+version = "1.7.2"
 description = "Python client for the Magento 2 API"
 authors = ["Bixoto <tech@bixoto.com>"]
 license = "MIT"
 homepage = "https://github.com/Bixoto/PyMagento"
 include = ["magento/py.typed"]
 readme = "README.md"
 packages = [
```

### Comparing `pymagento-1.7.1/PKG-INFO` & `pymagento-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymagento
-Version: 1.7.1
+Version: 1.7.2
 Summary: Python client for the Magento 2 API
 Home-page: https://github.com/Bixoto/PyMagento
 License: MIT
 Author: Bixoto
 Author-email: tech@bixoto.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

