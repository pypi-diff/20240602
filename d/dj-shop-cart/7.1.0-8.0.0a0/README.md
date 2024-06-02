# Comparing `tmp/dj_shop_cart-7.1.0.tar.gz` & `tmp/dj_shop_cart-8.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_shop_cart-7.1.0.tar", max compression
+gzip compressed data, was "dj_shop_cart-8.0.0a0.tar", max compression
```

## Comparing `dj_shop_cart-7.1.0.tar` & `dj_shop_cart-8.0.0a0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1079 2024-06-01 09:50:11.672798 dj_shop_cart-7.1.0/LICENSE
--rw-r--r--   0        0        0     3728 2024-06-01 09:50:11.673798 dj_shop_cart-7.1.0/README.md
--rw-r--r--   0        0        0        0 2022-03-08 07:27:09.000000 dj_shop_cart-7.1.0/dj_shop_cart/__init__.py
--rw-r--r--   0        0        0      190 2022-06-29 18:59:31.000000 dj_shop_cart-7.1.0/dj_shop_cart/apps.py
--rw-r--r--   0        0        0    10358 2024-06-01 10:40:32.489171 dj_shop_cart-7.1.0/dj_shop_cart/cart.py
--rw-r--r--   0        0        0     1236 2022-06-23 07:20:53.000000 dj_shop_cart-7.1.0/dj_shop_cart/conf.py
--rw-r--r--   0        0        0      212 2022-03-19 11:48:30.000000 dj_shop_cart-7.1.0/dj_shop_cart/context_processors.py
--rw-r--r--   0        0        0     1264 2022-03-03 15:36:44.000000 dj_shop_cart-7.1.0/dj_shop_cart/migrations/0001_initial.py
--rw-r--r--   0        0        0      351 2023-02-27 16:50:20.854935 dj_shop_cart-7.1.0/dj_shop_cart/migrations/0002_rename_items_cart_data.py
--rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.1.0/dj_shop_cart/migrations/__init__.py
--rw-r--r--   0        0        0      455 2023-02-27 16:49:22.862157 dj_shop_cart-7.1.0/dj_shop_cart/models.py
--rw-r--r--   0        0        0      435 2023-08-08 08:20:31.233795 dj_shop_cart-7.1.0/dj_shop_cart/protocols.py
--rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-7.1.0/dj_shop_cart/py.typed
--rw-r--r--   0        0        0     2419 2023-02-27 17:39:56.532528 dj_shop_cart-7.1.0/dj_shop_cart/storages.py
--rw-r--r--   0        0        0      202 2022-03-19 18:55:22.000000 dj_shop_cart-7.1.0/dj_shop_cart/utils.py
--rw-r--r--   0        0        0     1720 2024-06-01 10:41:26.954157 dj_shop_cart-7.1.0/pyproject.toml
--rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 dj_shop_cart-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-06-01 09:50:11.672798 dj_shop_cart-8.0.0a0/LICENSE
+-rw-r--r--   0        0        0     3692 2024-06-02 11:48:06.454400 dj_shop_cart-8.0.0a0/README.md
+-rw-r--r--   0        0        0        0 2022-03-08 07:27:09.000000 dj_shop_cart-8.0.0a0/dj_shop_cart/__init__.py
+-rw-r--r--   0        0        0      190 2022-06-29 18:59:31.000000 dj_shop_cart-8.0.0a0/dj_shop_cart/apps.py
+-rw-r--r--   0        0        0     9580 2024-06-02 15:02:49.335466 dj_shop_cart-8.0.0a0/dj_shop_cart/cart.py
+-rw-r--r--   0        0        0     1905 2024-06-02 14:50:43.410738 dj_shop_cart-8.0.0a0/dj_shop_cart/conf.py
+-rw-r--r--   0        0        0      181 2024-06-02 12:33:14.103059 dj_shop_cart-8.0.0a0/dj_shop_cart/context_processors.py
+-rw-r--r--   0        0        0     1264 2022-03-03 15:36:44.000000 dj_shop_cart-8.0.0a0/dj_shop_cart/migrations/0001_initial.py
+-rw-r--r--   0        0        0      387 2024-06-02 11:40:51.595479 dj_shop_cart-8.0.0a0/dj_shop_cart/migrations/0002_rename_items_cart_data.py
+-rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-8.0.0a0/dj_shop_cart/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2023-02-27 16:49:22.862157 dj_shop_cart-8.0.0a0/dj_shop_cart/models.py
+-rw-r--r--   0        0        0     1018 2024-06-02 11:40:51.595479 dj_shop_cart-8.0.0a0/dj_shop_cart/modifiers.py
+-rw-r--r--   0        0        0      435 2024-06-01 21:07:19.104774 dj_shop_cart-8.0.0a0/dj_shop_cart/protocols.py
+-rw-r--r--   0        0        0        0 2022-03-02 10:59:44.000000 dj_shop_cart-8.0.0a0/dj_shop_cart/py.typed
+-rw-r--r--   0        0        0     2419 2024-06-01 17:01:15.260938 dj_shop_cart-8.0.0a0/dj_shop_cart/storages.py
+-rw-r--r--   0        0        0      382 2024-06-02 11:40:51.595479 dj_shop_cart-8.0.0a0/dj_shop_cart/utils.py
+-rw-r--r--   0        0        0     1722 2024-06-02 15:04:05.180338 dj_shop_cart-8.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4817 1970-01-01 00:00:00.000000 dj_shop_cart-8.0.0a0/PKG-INFO
```

### Comparing `dj_shop_cart-7.1.0/LICENSE` & `dj_shop_cart-8.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.1.0/README.md` & `dj_shop_cart-8.0.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,23 +63,21 @@
         but be sure to update the corresponding setting (see Configuration). Even if you change the name the
         function signature should match this one.
         """
 
 
 # views.py
 
-from dj_shop_cart.cart import get_cart_class
+from dj_shop_cart.cart import Cart
 from django.http import HttpRequest
 from django.views.decorators.http import require_POST
 from django.shortcuts import get_object_or_404
 
 from .models import Product
 
-Cart = get_cart_class()
-
 
 @require_POST
 def add_product(request: HttpRequest, product_id:int):
     product = get_object_or_404(Product.objects.all(), pk=product_id)
     quantity = int(request.POST.get("quantity"))
     cart = Cart.new(request)
     cart.add(product, quantity=quantity)
@@ -124,8 +122,7 @@
 ```sh
 pytest
 ```
 
 ## Feedback
 
 If you have any feedback, please reach out to me at tobidegnon@proton.me.
-
```

### Comparing `dj_shop_cart-7.1.0/dj_shop_cart/cart.py` & `dj_shop_cart-8.0.0a0/dj_shop_cart/cart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 from __future__ import annotations
 
 import contextlib
 import itertools
-from typing import Iterator, Type, TypeVar, Union, cast
+from collections.abc import Iterator
+from functools import cached_property
+from typing import TypeVar, cast
 from uuid import uuid4
 
 from attrs import Factory, asdict, define, field
-from django.core.exceptions import ImproperlyConfigured, ObjectDoesNotExist
+from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.http import HttpRequest
 
 from .conf import conf
-from .protocols import Storage, Numeric
-from .utils import get_module
+from .modifiers import cart_modifiers_pool
+from .protocols import Numeric, Storage
+from .utils import import_class
 
-__all__ = ("Cart", "CartItem", "get_cart_class")
+__all__ = ("Cart", "CartItem", "get_cart_class", "get_cart")
 
-ProductModel = TypeVar("ProductModel", bound=models.Model)
-Variant = Union[str, int, dict, set]
+DjangoModel = TypeVar("DjangoModel", bound=models.Model)
 DEFAULT_CART_PREFIX = "default"
 
 
 @define(kw_only=True)
 class CartItem:
     id: str = field(factory=uuid4, converter=str)
     quantity: int = field(eq=False, converter=int)
-    variant: Variant | None = field(default=None)
+    variant: str | None = field(default=None)
     product_pk: str = field(converter=str)
     product_model_path: str
     metadata: dict = field(factory=dict, eq=False)
 
-    @property
-    def product(self) -> ProductModel:
-        model = cast(Type[ProductModel], get_module(self.product_model_path))
+    @cached_property
+    def product(self) -> DjangoModel:
+        model = cast(type[DjangoModel], import_class(self.product_model_path))
+        if func := getattr(model, "get_cart_object", None):
+            # this is a hack to allow to use a product that is not a django
+            # model instance / instance not already save in db
+            return func(self)  # noqa
         return model.objects.get(pk=self.product_pk)
 
     @property
     def subtotal(self) -> Numeric:
         return self.price * self.quantity
 
     @property
     def price(self) -> Numeric:
         return getattr(self.product, conf.CART_PRODUCT_GET_PRICE_METHOD)(self)
 
     @classmethod
     def from_product(
         cls,
-        product: ProductModel,
+        product: DjangoModel,
         quantity: int,
-        variant: Variant | None = None,
+        variant: str | None = None,
         metadata: dict | None = None,
     ) -> CartItem:
         metadata = metadata or {}
         return cls(
             quantity=quantity,
             variant=variant,
             product_pk=product.pk,
@@ -74,14 +80,18 @@
     def __iter__(self) -> Iterator[CartItem]:
         yield from self._items
 
     def __contains__(self, item: CartItem) -> bool:
         return item in self
 
     @property
+    def items(self) -> list[CartItem]:
+        return self._items
+
+    @property
     def total(self) -> Numeric:
         return sum(item.subtotal for item in self)
 
     @property
     def is_empty(self) -> bool:
         return self.unique_count == 0
 
@@ -96,15 +106,15 @@
     def unique_count(self) -> int:
         """
         The number of unique items in the cart, regardless of the quantity.
         """
         return len(self._items)
 
     @property
-    def products(self) -> list[ProductModel]:
+    def products(self) -> list[DjangoModel]:
         """
         The list of associated products.
         """
         return [item.product for item in self]
 
     def find(self, **criteria) -> list[CartItem]:
         """
@@ -123,18 +133,18 @@
         try:
             return self.find(**criteria)[0]
         except IndexError:
             return None
 
     def add(
         self,
-        product: ProductModel,
+        product: DjangoModel,
         *,
         quantity: int = 1,
-        variant: Variant | None = None,
+        variant: str | None = None,
         override_quantity: bool = False,
         metadata: dict | None = None,
     ) -> CartItem:
         """
         Add a new item to the cart
 
         :param product: An instance of a database product
@@ -153,33 +163,26 @@
         if not item:
             item = CartItem.from_product(
                 product, quantity=0, variant=variant, metadata=metadata
             )
             self._items.append(item)
         if metadata:
             item.metadata.update(metadata)
-        self.before_add(item=item, quantity=quantity)
+
+        for modifier in cart_modifiers_pool.get_modifiers():
+            modifier.before_add(cart=self, item=item, quantity=quantity)
+
         if override_quantity:
             item.quantity = quantity
         else:
             item.quantity += quantity
-        self.after_add(item=item)
-        self.save()
-        return item
 
-    def increase(self, item_id: str, quantity: int = 1) -> CartItem | None:
-        assert (
-            quantity >= 1
-        ), f"Item quantity must be greater than or equal to 1: {quantity}"
-        item = self.find_one(id=item_id)
-        self.before_add(item=item, quantity=quantity)
-        if not item:
-            return None
-        item.quantity += quantity
-        self.after_add(item=item)
+        for modifier in cart_modifiers_pool.get_modifiers():
+            modifier.after_add(cart=self, item=item)
+
         self.save()
         return item
 
     def remove(
         self,
         item_id: str,
         *,
@@ -191,22 +194,28 @@
         :param item_id: The cart item id
         :param quantity: The quantity of the product to remove from the cart
         :return: The removed item with an updated quantity or None
         """
         item = self.find_one(id=item_id)
         if not item:
             return None
-        self.before_remove(item=item, quantity=quantity)
+
+        for modifier in cart_modifiers_pool.get_modifiers():
+            modifier.before_remove(cart=self, item=item, quantity=quantity)
+
         if quantity:
             item.quantity -= int(quantity)
         else:
             item.quantity = 0
         if item.quantity <= 0:
             self._items.pop(self._items.index(item))
-        self.after_remove(item=item)
+
+        for modifier in cart_modifiers_pool.get_modifiers():
+            modifier.after_remove(cart=self, item=item)
+
         self.save()
         return item
 
     def save(self) -> None:
         items = []
         for item in self._items:
             try:
@@ -216,52 +225,23 @@
                 continue
             items.append(asdict(item))
         # load storage old data to avoid overwriting
         data = self.storage.load()
         data[self.prefix] = {"items": items, "metadata": self.metadata}
         self.storage.save(data)
 
-    def empty(self, clear_metadata: bool = True) -> None:
-        """Delete all items in the cart, and optionally clear the metadata."""
-        self._items = []
-        self._metadata = {}
-        data = self.storage.load()
-        with contextlib.suppress(KeyError):
-            data.pop(self.prefix)
-        if clear_metadata:
-            self._metadata.clear()
-        self.storage.save(data)
-
     def variants_group_by_product(self) -> dict[str, list[CartItem]]:
         """
         Return a dictionary with the products ids as keys and a list of variant as values.
         """
         return {
             key: list(items)
             for key, items in itertools.groupby(self, lambda item: item.product_pk)
         }
 
-    def before_add(self, item: CartItem, quantity: int) -> None:
-        """This is meant to be overridden by subclasses to add some logic that is run
-        before an item is added to the cart."""
-
-    def after_add(self, item: CartItem) -> None:
-        """This is meant to be overridden by subclasses to add some logic that is run
-        after an item is added to the cart."""
-
-    def before_remove(
-        self, item: CartItem | None = None, quantity: int | None = None
-    ) -> None:
-        """This is meant to be overridden by subclasses to add some logic that is run
-        before an item is removed from the cart."""
-
-    def after_remove(self, item: CartItem | None = None) -> None:
-        """This is meant to be overridden by subclasses to add some logic that is run after
-        an item is removed from the cart."""
-
     @property
     def metadata(self) -> dict:
         return self._metadata
 
     def update_metadata(self, metadata: dict) -> None:
         self._metadata.update(metadata)
         self.save()
@@ -270,18 +250,32 @@
         if keys:
             for key in keys:
                 self._metadata.pop(key, None)
         else:
             self._metadata = {}
         self.save()
 
+    def empty(self, clear_metadata: bool = True) -> None:
+        """Delete all items in the cart, and optionally clear the metadata."""
+        self._items = []
+        self._metadata = {}
+        data = self.storage.load()
+        with contextlib.suppress(KeyError):
+            data.pop(self.prefix)
+        if clear_metadata:
+            self._metadata.clear()
+        self.storage.save(data)
+
+    def empty_all(self) -> None:
+        """Empty all carts for the current user"""
+        self.storage.clear()
+
     @classmethod
-    def new(cls, request: HttpRequest, prefix: str = DEFAULT_CART_PREFIX) -> Cart:
+    def new(cls, storage: Storage, prefix: str = DEFAULT_CART_PREFIX) -> Cart:
         """Appropriately create a new cart instance. This builder load existing cart if needed."""
-        storage = get_module(conf.CART_STORAGE_BACKEND)(request)
         instance = cls(storage=storage, prefix=prefix)
         try:
             data = storage.load().get(prefix, {})
         except AttributeError:
             data = {}
 
         metadata = data.get("metadata", {})
@@ -293,24 +287,18 @@
             except ObjectDoesNotExist:
                 # If the product associated with the item is no longer in the database, we skip it
                 continue
             instance._items.append(item)
         instance._metadata = metadata
         return instance
 
-    @classmethod
-    def empty_all(cls, request: HttpRequest) -> None:
-        """Empty all carts, prefixed or not."""
-        storage = get_module(conf.CART_STORAGE_BACKEND)(request)
-        storage.clear()
+
+def get_cart(request: HttpRequest, prefix: str = DEFAULT_CART_PREFIX) -> Cart:
+    storage = conf.CART_STORAGE_BACKEND(request)
+    return Cart.new(storage=storage, prefix=prefix)
 
 
 def get_cart_class() -> type[Cart]:
     """
     Returns the correct cart manager class
     """
-    klass = get_module(conf.CART_CLASS)
-    if not issubclass(klass, Cart):
-        raise ImproperlyConfigured(
-            "The `CART_CLASS` settings must be a subclass of the `Cart` class."
-        )
-    return klass
+    return Cart
```

### Comparing `dj_shop_cart-7.1.0/dj_shop_cart/migrations/0001_initial.py` & `dj_shop_cart-8.0.0a0/dj_shop_cart/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.1.0/dj_shop_cart/storages.py` & `dj_shop_cart-8.0.0a0/dj_shop_cart/storages.py`

 * *Files identical despite different names*

### Comparing `dj_shop_cart-7.1.0/pyproject.toml` & `dj_shop_cart-8.0.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dj-shop-cart"
-version = "7.1.0"
+version = "8.0.0a0"
 description = "Simple django cart manager for your django projects."
 authors = ["Tobi DEGNON <tobidegnon@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tobi-De/dj-shop-cart"
 homepage = "https://tobi-de.github.io/dj-shop-cart/"
 keywords = ["django", "python", "cart", "shop", "ecommerce"]
```

### Comparing `dj_shop_cart-7.1.0/PKG-INFO` & `dj_shop_cart-8.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-shop-cart
-Version: 7.1.0
+Version: 8.0.0a0
 Summary: Simple django cart manager for your django projects.
 Home-page: https://tobi-de.github.io/dj-shop-cart/
 License: MIT
 Keywords: django,python,cart,shop,ecommerce
 Author: Tobi DEGNON
 Author-email: tobidegnon@protonmail.com
 Requires-Python: >=3.10,<4.0
@@ -92,23 +92,21 @@
         but be sure to update the corresponding setting (see Configuration). Even if you change the name the
         function signature should match this one.
         """
 
 
 # views.py
 
-from dj_shop_cart.cart import get_cart_class
+from dj_shop_cart.cart import Cart
 from django.http import HttpRequest
 from django.views.decorators.http import require_POST
 from django.shortcuts import get_object_or_404
 
 from .models import Product
 
-Cart = get_cart_class()
-
 
 @require_POST
 def add_product(request: HttpRequest, product_id:int):
     product = get_object_or_404(Product.objects.all(), pk=product_id)
     quantity = int(request.POST.get("quantity"))
     cart = Cart.new(request)
     cart.add(product, quantity=quantity)
@@ -154,8 +152,7 @@
 pytest
 ```
 
 ## Feedback
 
 If you have any feedback, please reach out to me at tobidegnon@proton.me.
 
-
```

