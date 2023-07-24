# Comparing `tmp/pydantic_xml-2.0.0a1.tar.gz` & `tmp/pydantic_xml-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-2.0.0a1.tar", max compression
+gzip compressed data, was "pydantic_xml-2.0.0a2.tar", max compression
```

## Comparing `pydantic_xml-2.0.0a1.tar` & `pydantic_xml-2.0.0a2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1211 2023-07-15 07:13:13.144047 pydantic_xml-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     3335 2023-07-15 07:13:13.144047 pydantic_xml-2.0.0a1/README.rst
--rw-r--r--   0        0        0      453 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    13335 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      374 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      712 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/errors.py
--rw-r--r--   0        0        0    12182 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/py.typed
--rw-r--r--   0        0        0       36 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0       99 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     3270 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     3174 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     5289 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0    11102 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     5271 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     1428 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/typed_mapping.py
--rw-r--r--   0        0        0     4915 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     2543 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     9374 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0      322 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1876 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4833 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     3335 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/README.rst
+-rw-r--r--   0        0        0      453 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    13335 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      374 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      712 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    12352 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       36 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     3386 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     3290 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     5492 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0    11466 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     5561 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     1428 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/typed_mapping.py
+-rw-r--r--   0        0        0     5135 2023-07-24 18:53:31.756739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2659 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     9774 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0      322 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1883 2023-07-24 18:53:31.760739 pydantic_xml-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4823 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0a2/PKG-INFO
```

### Comparing `pydantic_xml-2.0.0a1/LICENSE` & `pydantic_xml-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/README.rst` & `pydantic_xml-2.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/element/element.py` & `pydantic_xml-2.0.0a2/pydantic_xml/element/element.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/element/native/lxml.py` & `pydantic_xml-2.0.0a2/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/element/native/std.py` & `pydantic_xml-2.0.0a2/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/errors.py` & `pydantic_xml-2.0.0a2/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/model.py` & `pydantic_xml-2.0.0a2/pydantic_xml/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,42 +298,43 @@
     def model_rebuild(cls, **kwargs: Any) -> None:
         super().model_rebuild(**kwargs)
 
         if cls.__xml_serializer__ is None and cls.__pydantic_complete__:
             cls.__build_serializer__()
 
     @classmethod
-    def from_xml_tree(cls: Type[ModelT], root: etree.Element) -> ModelT:
+    def from_xml_tree(cls: Type[ModelT], root: etree.Element, context: Optional[Dict[str, Any]] = None) -> ModelT:
         """
         Deserializes an xml element tree to an object of `cls` type.
 
         :param root: xml element to deserialize the object from
         :return: deserialized object
         """
 
         assert cls.__xml_serializer__ is not None, f"model {cls.__name__} is partially initialized"
 
         if root.tag == cls.__xml_serializer__.element_name:
-            obj = typing.cast(ModelT, cls.__xml_serializer__.deserialize(XmlElement.from_native(root)))
+            obj = typing.cast(ModelT, cls.__xml_serializer__.deserialize(XmlElement.from_native(root), context=context))
             return obj
         else:
             raise errors.ParsingError(
                 f"root element not found (actual: {root.tag}, expected: {cls.__xml_serializer__.element_name})",
             )
 
     @classmethod
-    def from_xml(cls: Type[ModelT], source: Union[str, bytes]) -> ModelT:
+    def from_xml(cls: Type[ModelT], source: Union[str, bytes], context: Optional[Dict[str, Any]] = None) -> ModelT:
         """
         Deserializes an xml string to an object of `cls` type.
 
         :param source: xml string
+        :param context: pydantic validation context
         :return: deserialized object
         """
 
-        return cls.from_xml_tree(etree.fromstring(source))
+        return cls.from_xml_tree(etree.fromstring(source), context=context)
 
     def to_xml_tree(self, *, skip_empty: bool = False) -> etree.Element:
         """
         Serializes the object to an xml tree.
 
         :param skip_empty: skip empty elements (elements without sub-elements, attributes and text, Nones)
         :return: object xml representation
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 from pydantic_core import core_schema as pcs
 
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.serializer import TYPE_FAMILY, SchemaTypeFamily, Serializer
 from pydantic_xml.typedefs import EntityLocation
@@ -35,23 +35,28 @@
             raise errors.SerializationError("value length is incorrect")
 
         for serializer, val, enc in zip(self._inner_serializers, value, encoded):
             serializer.serialize(element, val, enc, skip_empty=skip_empty)
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[List[Any]]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[List[Any]]:
         if self._computed:
             return None
 
         if element is None:
             return None
 
         return [
-            serializer.deserialize(element)
+            serializer.deserialize(element, context=context)
             for serializer in self._inner_serializers
         ]
 
 
 def from_core_schema(schema: pcs.TuplePositionalSchema, ctx: Serializer.Context) -> Serializer:
     for item_schema in schema['items_schema']:
         item_schema, ctx = Serializer.preprocess_schema(item_schema, ctx)
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic_core import core_schema as pcs
 
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.serializer import TYPE_FAMILY, SchemaTypeFamily, Serializer
 from pydantic_xml.typedefs import EntityLocation
@@ -40,23 +40,28 @@
             if skip_empty and val is None:
                 continue
 
             self._inner_serializer.serialize(element, val, enc, skip_empty=skip_empty)
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[List[Any]]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[List[Any]]:
         if self._computed:
             return None
 
         if element is None:
             return None
 
         result = []
-        while (value := self._inner_serializer.deserialize(element)) is not None:
+        while (value := self._inner_serializer.deserialize(element, context=context)) is not None:
             result.append(value)
 
         return result or None
 
 
 def from_core_schema(schema: HomogeneousCollectionTypeSchema, ctx: Serializer.Context) -> Serializer:
     items_schema = schema['items_schema']
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,20 @@
         element.set_attributes({
             QName(tag=attr, ns=ns).uri: str(enc)
             for attr, enc in encoded.items()
         })
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[Dict[str, str]]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[Dict[str, str]]:
         if self._computed:
             return None
 
         if element is None or (attributes := element.pop_attributes()) is None:
             return None
 
         return {
@@ -101,20 +106,25 @@
         super().serialize(sub_element, value, encoded, skip_empty=skip_empty)
         if skip_empty and sub_element.is_empty():
             return None
         else:
             element.append_element(sub_element)
             return sub_element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[Dict[str, str]]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[Dict[str, str]]:
         if self._computed:
             return None
 
         if element and (sub_element := element.pop_element(self._element_name, self._search_mode)) is not None:
-            return super().deserialize(sub_element)
+            return super().deserialize(sub_element, context=context)
         else:
             return None
 
 
 def from_core_schema(schema: pcs.DictSchema, ctx: Serializer.Context) -> Serializer:
     key_schema = schema['keys_schema']
     key_schema, key_ctx = Serializer.preprocess_schema(key_schema, ctx)
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,25 +123,30 @@
             return None
 
         for field_name, field_serializer in self._field_serializers.items():
             field_serializer.serialize(element, getattr(value, field_name), encoded[field_name], skip_empty=skip_empty)
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional['pxml.BaseXmlModel']:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional['pxml.BaseXmlModel']:
         if element is None:
             return None
 
         result = {
             self._fields_validation_aliases.get(field_name, field_name): field_value
             for field_name, field_serializer in self._field_serializers.items()
-            if (field_value := field_serializer.deserialize(element)) is not None
+            if (field_value := field_serializer.deserialize(element, context=context)) is not None
         }
 
-        return self._model.model_validate(result, strict=False)
+        return self._model.model_validate(result, strict=False, context=context)
 
 
 class RootModelSerializer(BaseModelSerializer):
     @classmethod
     def from_core_schema(cls, schema: pcs.ModelSchema, ctx: Serializer.Context) -> 'RootModelSerializer':
         model_cls = schema['cls']
         root_schema = schema['schema']
@@ -204,21 +209,26 @@
         if value is None:
             return None
 
         self._root_serializer.serialize(element, getattr(value, 'root'), encoded, skip_empty=skip_empty)
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional['pxml.BaseXmlModel']:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional['pxml.BaseXmlModel']:
         if element is None:
             return None
 
-        result = self._root_serializer.deserialize(element)
+        result = self._root_serializer.deserialize(element, context=context)
 
-        return self._model.model_validate(result, strict=False)
+        return self._model.model_validate(result, strict=False, context=context)
 
 
 class ModelProxySerializer(BaseModelSerializer):
     @classmethod
     def from_core_schema(cls, schema: pcs.ModelSchema, ctx: Serializer.Context) -> 'ModelProxySerializer':
         model_cls = schema['cls']
         assert issubclass(model_cls, pxml.BaseXmlModel), "unexpected model type"
@@ -275,23 +285,28 @@
         self._model.__xml_serializer__.serialize(sub_element, value, encoded, skip_empty=skip_empty)
         if skip_empty and sub_element.is_empty():
             return None
         else:
             element.append_element(sub_element)
             return sub_element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional['pxml.BaseXmlModel']:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional['pxml.BaseXmlModel']:
         assert self._model.__xml_serializer__ is not None, f"model {self._model.__name__} is partially initialized"
 
         if self._computed:
             return None
 
         if element is not None and \
                 (sub_element := element.pop_element(self._element_name, self._search_mode)) is not None:
-            return self._model.__xml_serializer__.deserialize(sub_element)
+            return self._model.__xml_serializer__.deserialize(sub_element, context=context)
         else:
             return None
 
 
 def from_core_schema(schema: pcs.ModelSchema, ctx: Serializer.Context) -> Serializer:
     is_root_model = schema['root_model']
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/primitive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from pydantic_core import core_schema as pcs
 
 from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.serializer import SearchMode, Serializer
 from pydantic_xml.typedefs import EntityLocation, NsMap
@@ -42,15 +42,20 @@
     ) -> Optional[XmlElementWriter]:
         if value is None and skip_empty:
             return element
 
         element.set_text(str(encoded))
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[str]:
         if self._computed:
             return None
 
         if element is None:
             return None
 
         return element.pop_text() or None
@@ -80,15 +85,19 @@
         if value is None and skip_empty:
             return element
 
         element.set_attribute(self._attr_name, str(encoded))
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *, context: Optional[Dict[str, Any]],
+    ) -> Optional[str]:
         if self._computed:
             return None
 
         if element is None:
             return None
 
         return element.pop_attrib(self._attr_name)
@@ -125,21 +134,26 @@
         super().serialize(sub_element, value, encoded, skip_empty=skip_empty)
         if skip_empty and sub_element.is_empty():
             return None
         else:
             element.append_element(sub_element)
             return sub_element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[str]:
         if self._computed:
             return None
 
         if element is not None and \
                 (sub_element := element.pop_element(self._element_name, self._search_mode)) is not None:
-            return super().deserialize(sub_element)
+            return super().deserialize(sub_element, context=context)
         else:
             return None
 
 
 def from_core_schema(schema: PrimitiveTypeSchema, ctx: Serializer.Context) -> Serializer:
     if ctx.entity_location is EntityLocation.ELEMENT:
         return ElementSerializer.from_core_schema(schema, ctx)
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/typed_mapping.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/typed_mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/union.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,19 +31,24 @@
         self._inner_serializer = inner_serializer
 
     def serialize(
             self, element: XmlElementWriter, value: Any, encoded: Any, *, skip_empty: bool = False,
     ) -> Optional[XmlElementWriter]:
         return self._inner_serializer.serialize(element, value, encoded, skip_empty=skip_empty)
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[str]:
         if self._computed:
             return None
 
-        return self._inner_serializer.deserialize(element)
+        return self._inner_serializer.deserialize(element, context=context)
 
 
 class ModelSerializer(Serializer):
     @classmethod
     def from_core_schema(cls, schema: pcs.UnionSchema, ctx: Serializer.Context) -> 'ModelSerializer':
         computed = ctx.field_computed
         inner_serializers: List[ModelProxySerializer] = []
@@ -71,27 +76,32 @@
     ) -> Optional[XmlElementWriter]:
         for serializer in self._inner_serializers:
             if serializer.model is type(value):
                 return serializer.serialize(element, value, encoded, skip_empty=skip_empty)
 
         return None
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional['pxml.BaseXmlModel']:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional['pxml.BaseXmlModel']:
         if self._computed:
             return None
 
         if element is None:
             return None
 
         last_error: Optional[Exception] = None
         result: Any = None
         for serializer in self._inner_serializers:
             snapshot = element.create_snapshot()
             try:
-                if (result := serializer.deserialize(snapshot)) is None:
+                if (result := serializer.deserialize(snapshot, context=context)) is None:
                     continue
                 else:
                     element.apply_snapshot(snapshot)
                     return result
             except pd.ValidationError as e:
                 last_error = e
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/factories/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Sized
+from typing import Any, Dict, Optional, Sized
 
 from pydantic_core import core_schema as pcs
 
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
 from pydantic_xml.serializers.serializer import SearchMode, Serializer
 from pydantic_xml.typedefs import NsMap
 from pydantic_xml.utils import QName, merge_nsmaps
@@ -51,20 +51,25 @@
         for part in self._path:
             element = element.find_element_or_create(part, self._search_mode, nsmap=self._nsmap)
 
         self._inner_serializer.serialize(element, value, encoded, skip_empty=skip_empty)
 
         return element
 
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[Any]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[Any]:
         if self._computed:
             return None
 
         if element is not None and \
                 (sub_element := element.find_sub_element(self._path, self._search_mode)) is not None:
-            return self._inner_serializer.deserialize(sub_element)
+            return self._inner_serializer.deserialize(sub_element, context=context)
         else:
             return None
 
 
 def from_core_schema(schema: pcs.CoreSchema, ctx: Serializer.Context) -> Serializer:
     return ElementPathSerializer.from_core_schema(schema, ctx)
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/serializers/serializer.py` & `pydantic_xml-2.0.0a2/pydantic_xml/serializers/serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     HOMOGENEOUS_COLLECTION = 3
     HETEROGENEOUS_COLLECTION = 4
     MAPPING = 5
     TYPED_MAPPING = 6
     UNION = 7
     DEFINITIONS = 8
     DEFINITION_REF = 9
+    JSON_OR_PYTHON = 10
 
 
 TYPE_FAMILY = {
     'none':             SchemaTypeFamily.PRIMITIVE,
     'bool':             SchemaTypeFamily.PRIMITIVE,
     'int':              SchemaTypeFamily.PRIMITIVE,
     'float':            SchemaTypeFamily.PRIMITIVE,
@@ -65,14 +66,16 @@
     'function-wrap':    SchemaTypeFamily.META,
     'function-plain':   SchemaTypeFamily.META,
     'default':          SchemaTypeFamily.META,
     'nullable':         SchemaTypeFamily.META,
 
     'definitions':      SchemaTypeFamily.DEFINITIONS,
     'definition-ref':   SchemaTypeFamily.DEFINITION_REF,
+
+    'json-or-python':   SchemaTypeFamily.JSON_OR_PYTHON,
 }
 
 
 class XmlEntityInfoP(typing.Protocol):
     location: Optional[EntityLocation]
     path: Optional[str]
     ns: Optional[str]
@@ -167,14 +170,18 @@
                 ctx = ctx.replace(has_default=True)
             elif schema_type == 'nullable':
                 ctx = ctx.replace(optional=True)
 
             inner_schema = schema['schema']
             return cls.preprocess_schema(inner_schema, ctx)
 
+        elif type_family is SchemaTypeFamily.JSON_OR_PYTHON:
+            inner_schema = schema['python_schema']
+            return cls.preprocess_schema(inner_schema, ctx)
+
         elif type_family is SchemaTypeFamily.DEFINITIONS:
             schema = typing.cast(pcs.DefinitionsSchema, schema)
             definitions = {
                 definition['ref']: definition
                 for definition in schema['definitions']
             }
             ctx = ctx.replace(definitions=ChainMap(definitions, ctx.definitions))
@@ -243,14 +250,20 @@
         :param value: original value
         :param encoded: encoded value (encoded by pydantic)
         :param skip_empty: skip empty element
         :return: created sub-element or original one if sub-element has not been created
         """
 
     @abc.abstractmethod
-    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[Any]:
+    def deserialize(
+            self,
+            element: Optional[XmlElementReader],
+            *,
+            context: Optional[Dict[str, Any]],
+    ) -> Optional[Any]:
         """
         Deserializes a value from the xml element.
 
         :param element: xml element the value is deserialized from
+        :param context: pydantic validation context
         :return: deserialized value
         """
```

### Comparing `pydantic_xml-2.0.0a1/pydantic_xml/utils.py` & `pydantic_xml-2.0.0a2/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-2.0.0a1/pyproject.toml` & `pydantic_xml-2.0.0a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "2.0.0a1"
+version = "2.0.0a2"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
@@ -21,30 +21,30 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-lxml = {version = "^4.9.0", optional = true}
-pydantic = "2.0"
+python = ">=3.8"
+lxml = {version = ">=4.9.0", optional = true}
+pydantic = ">=2.0.0"
 
 furo = {version = "^2022.12.7", optional = true}
 Sphinx = {version = "^5.3.0", optional = true}
 sphinx-copybutton = {version = "^0.5.1", optional = true}
 sphinx_design = {version = "^0.3.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 
 [tool.poetry.extras]
 lxml = ['lxml']
 docs = ['Sphinx', 'toml', 'sphinx_design', 'furo', 'sphinx-copybutton']
 
 [tool.poetry.dev-dependencies]
-lxml-stubs = "^0.4.0"
+lxml-stubs = ">=0.4.0"
 mypy = "^1.4.1"
 pre-commit = "~3.2.0"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 xmldiff = "2.5"
 
 [build-system]
```

### Comparing `pydantic_xml-2.0.0a1/PKG-INFO` & `pydantic_xml-2.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: License :: Public Domain
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Provides-Extra: lxml
 Requires-Dist: Sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
-Requires-Dist: lxml (>=4.9.0,<5.0.0) ; extra == "lxml"
-Requires-Dist: pydantic (==2.0)
+Requires-Dist: lxml (>=4.9.0) ; extra == "lxml"
+Requires-Dist: pydantic (>=2.0.0)
 Requires-Dist: sphinx-copybutton (>=0.5.1,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) ; extra == "docs"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "docs"
 Project-URL: Documentation, https://github.com/dapper91/pydantic-xml
 Project-URL: Repository, https://github.com/dapper91/pydantic-xml
 Description-Content-Type: text/x-rst
```

