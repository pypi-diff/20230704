# Comparing `tmp/pyfactories-1.0.0.tar.gz` & `tmp/pyfactories-2.0.0.tar.gz`

## Comparing `pyfactories-1.0.0.tar` & `pyfactories-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/exceptions.py
--rw-r--r--   0        0        0    28558 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/factory.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/fields.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/protocols.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/py.typed
--rw-r--r--   0        0        0     7271 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/collection.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/date.py
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/decimal.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/float.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/integer.py
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/constraints/strings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/extensions/__init__.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/extensions/beanie_odm.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/extensions/odmantic_odm.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/extensions/ormar_orm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/plugins/__init__.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/plugins/pytest_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/value_generators/__init__.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/value_generators/complex_types.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/value_generators/constrained_number.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/value_generators/primitives.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyfactories/value_generators/regex.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfactories-1.0.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyfactories-1.0.0/LICENSE
--rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 pyfactories-1.0.0/README.md
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pyfactories-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7636 2020-02-02 00:00:00.000000 pyfactories-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/exceptions.py
+-rw-r--r--   0        0        0    28567 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/factory.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/fields.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/protocols.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/py.typed
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/__init__.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/collection.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/date.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/decimal.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/float.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/integer.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/constraints/strings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/extensions/__init__.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/extensions/beanie_odm.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/extensions/odmantic_odm.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/extensions/ormar_orm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/plugins/__init__.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/plugins/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/value_generators/__init__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/value_generators/complex_types.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/value_generators/constrained_number.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/value_generators/primitives.py
+-rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyfactories/value_generators/regex.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pyfactories-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyfactories-2.0.0/LICENSE
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 pyfactories-2.0.0/README.md
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pyfactories-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 pyfactories-2.0.0/PKG-INFO
```

### Comparing `pyfactories-1.0.0/pyfactories/__init__.py` & `pyfactories-2.0.0/pyfactories/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.0"
+__version__ = "2.0.0"
 
 from .exceptions import ConfigurationError
 from .extensions import (
     BeanieDocumentFactory,
     BeaniePersistenceHandler,
     OdmanticModelFactory,
     OrmarModelFactory,
```

### Comparing `pyfactories-1.0.0/pyfactories/factory.py` & `pyfactories-2.0.0/pyfactories/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     TypeVar,
     Union,
     cast,
 )
 from uuid import NAMESPACE_DNS, UUID, uuid1, uuid3, uuid5
 
 from faker import Faker
-from pydantic import (
+from pydantic.v1 import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
     AmqpDsn,
     AnyHttpUrl,
     AnyUrl,
@@ -79,16 +79,16 @@
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
     create_model_from_typeddict,
 )
-from pydantic.color import Color
-from pydantic.fields import SHAPE_DICT, SHAPE_MAPPING
+from pydantic.v1.color import Color
+from pydantic.v1.fields import SHAPE_DICT, SHAPE_MAPPING
 from typing_extensions import _TypedDictMeta  # type: ignore
 from typing_extensions import TypeGuard, get_args, is_typeddict
 
 from pyfactories.constraints.collection import handle_constrained_collection
 from pyfactories.constraints.date import handle_constrained_date
 from pyfactories.constraints.decimal import handle_constrained_decimal
 from pyfactories.constraints.float import handle_constrained_float
```

### Comparing `pyfactories-1.0.0/pyfactories/fields.py` & `pyfactories-2.0.0/pyfactories/fields.py`

 * *Files identical despite different names*

### Comparing `pyfactories-1.0.0/pyfactories/protocols.py` & `pyfactories-2.0.0/pyfactories/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=unnecessary-ellipsis
 from typing import Any, Dict, List, Protocol, TypeVar, Union, runtime_checkable
 
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 
 
 # According to https://github.com/python/cpython/blob/main/Lib/dataclasses.py#L1213
 # having __dataclass_fields__ is enough to identity a dataclass.
 @runtime_checkable
 class DataclassProtocol(Protocol):
     __dataclass_fields__: Dict[str, Any]
```

### Comparing `pyfactories-1.0.0/pyfactories/utils.py` & `pyfactories-2.0.0/pyfactories/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import Field as DataclassField
 from dataclasses import fields as get_dataclass_fields
 from decimal import Decimal
 from inspect import isclass
 from typing import TYPE_CHECKING, Any, Optional, Tuple, Type, TypeVar, cast
 
-from pydantic import BaseModel, create_model
-from pydantic.generics import GenericModel
-from pydantic.utils import almost_equal_floats
+from pydantic.v1 import BaseModel, create_model
+from pydantic.v1.generics import GenericModel
+from pydantic.v1.utils import almost_equal_floats
 
 T = TypeVar("T", int, float, Decimal)
 
 if TYPE_CHECKING:
     from pydantic.fields import ModelField
     from typing_extensions import NewType, TypeGuard
```

### Comparing `pyfactories-1.0.0/pyfactories/constraints/collection.py` & `pyfactories-2.0.0/pyfactories/constraints/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import TYPE_CHECKING, Any, Type, Union, cast
 
 from pyfactories.exceptions import ParameterError
 from pyfactories.utils import unwrap_new_type_if_needed
 from pyfactories.value_generators.complex_types import handle_complex_type
 
 if TYPE_CHECKING:  # pragma: no cover
-    from pydantic import ConstrainedList, ConstrainedSet
-    from pydantic.fields import ModelField
+    from pydantic.v1 import ConstrainedList, ConstrainedSet
+    from pydantic.v1.fields import ModelField
 
     from pyfactories.factory import ModelFactory
 
 
 def handle_constrained_collection(
     collection_type: Union[Type[list], Type[set]],
     model_factory: Type["ModelFactory"],
```

### Comparing `pyfactories-1.0.0/pyfactories/constraints/date.py` & `pyfactories-2.0.0/pyfactories/constraints/date.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, timedelta
 from typing import TYPE_CHECKING, Type, cast
 
 if TYPE_CHECKING:
     from faker import Faker
-    from pydantic import ConstrainedDate
+    from pydantic.v1 import ConstrainedDate
 
 
 def handle_constrained_date(constrained_date: Type["ConstrainedDate"], faker: "Faker") -> date:
     """
     Generates a date value fulfilling the expected constraints.
     Args:
         constrained_date:
```

### Comparing `pyfactories-1.0.0/pyfactories/constraints/decimal.py` & `pyfactories-2.0.0/pyfactories/constraints/decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pyfactories.value_generators.constrained_number import (
     generate_constrained_number,
     get_constrained_number_range,
 )
 from pyfactories.value_generators.primitives import create_random_decimal
 
 if TYPE_CHECKING:
-    from pydantic import ConstrainedDecimal
+    from pydantic.v1 import ConstrainedDecimal
 
 
 def validate_max_digits(
     max_digits: int,
     minimum: Optional[Decimal],
     decimal_places: Optional[int],
 ) -> None:
```

### Comparing `pyfactories-1.0.0/pyfactories/constraints/float.py` & `pyfactories-2.0.0/pyfactories/constraints/float.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyfactories.value_generators.constrained_number import (
     generate_constrained_number,
     get_constrained_number_range,
 )
 from pyfactories.value_generators.primitives import create_random_float
 
 if TYPE_CHECKING:
-    from pydantic import ConstrainedFloat
+    from pydantic.v1 import ConstrainedFloat
 
 
 def handle_constrained_float(field: "ConstrainedFloat") -> float:
     """Handles 'ConstrainedFloat' instances."""
     multiple_of = field.multiple_of
 
     minimum, maximum = get_constrained_number_range(
```

### Comparing `pyfactories-1.0.0/pyfactories/constraints/integer.py` & `pyfactories-2.0.0/pyfactories/constraints/integer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pyfactories.value_generators.constrained_number import (
     generate_constrained_number,
     get_constrained_number_range,
 )
 from pyfactories.value_generators.primitives import create_random_integer
 
 if TYPE_CHECKING:
-    from pydantic import ConstrainedInt
+    from pydantic.v1 import ConstrainedInt
 
 
 def handle_constrained_int(field: "ConstrainedInt") -> int:
     """Handles 'ConstrainedInt' instances."""
     multiple_of = field.multiple_of
 
     minimum, maximum = get_constrained_number_range(
```

### Comparing `pyfactories-1.0.0/pyfactories/constraints/strings.py` & `pyfactories-2.0.0/pyfactories/constraints/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, Any, Optional, Pattern, Tuple, Union
 
 from pyfactories.exceptions import ParameterError
 from pyfactories.value_generators.primitives import create_random_bytes, create_random_string
 from pyfactories.value_generators.regex import RegexFactory
 
 if TYPE_CHECKING:
-    from pydantic import ConstrainedBytes, ConstrainedStr
+    from pydantic.v1 import ConstrainedBytes, ConstrainedStr
 
 
 def parse_constrained_string_or_bytes(
     field: Union["ConstrainedStr", "ConstrainedBytes"]
 ) -> Tuple[Optional[int], Optional[int], bool]:
     """Parses and validates the given field."""
     lower_case = field.to_lower
```

### Comparing `pyfactories-1.0.0/pyfactories/extensions/beanie_odm.py` & `pyfactories-2.0.0/pyfactories/extensions/beanie_odm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import TYPE_CHECKING, Any, List, Union
 
-from pydantic import BaseModel
+from pydantic.v1 import BaseModel
 
 from pyfactories.factory import ModelFactory
 from pyfactories.protocols import AsyncPersistenceProtocol
 
 try:
     from beanie import Document
 except ImportError:
     Document = BaseModel
 
 if TYPE_CHECKING:
-    from pydantic.fields import ModelField
+    from pydantic.v1.fields import ModelField
 
 
 class BeaniePersistenceHandler(AsyncPersistenceProtocol[Document]):
     async def save(self, data: Document) -> Document:
         """Persists a single instance in mongoDB."""
         return await data.insert()
```

### Comparing `pyfactories-1.0.0/pyfactories/extensions/ormar_orm.py` & `pyfactories-2.0.0/pyfactories/extensions/ormar_orm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import random
 from typing import TYPE_CHECKING, Any, Union
 
-from pydantic import BaseModel
-from pydantic.utils import smart_deepcopy
+from pydantic.v1 import BaseModel
+from pydantic.v1.utils import smart_deepcopy
 
 from pyfactories.factory import ModelFactory
 from pyfactories.utils import is_pydantic_model, is_union
 
 try:
     from ormar import Model
 except ImportError:
     Model = BaseModel
 
 if TYPE_CHECKING:
-    from pydantic.fields import ModelField
+    from pydantic.v1.fields import ModelField
 
 
 class OrmarModelFactory(ModelFactory[Model]):  # pragma: no cover
     @classmethod
     def get_field_value(
         cls, model_field: "ModelField", field_parameters: Union[dict, list, None] = None
     ) -> Any:
```

### Comparing `pyfactories-1.0.0/pyfactories/plugins/pytest_plugin.py` & `pyfactories-2.0.0/pyfactories/plugins/pytest_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from inspect import isclass
 from typing import Any, Callable, ClassVar, Dict, Literal, Optional, Type, Union
 
 import pytest
 from _pytest.config import Config
-from pydantic import validate_arguments
+from pydantic.v1 import validate_arguments
 
 from pyfactories.exceptions import ParameterError
 from pyfactories.factory import ModelFactory
 
 Scope = Union[
     Literal["session", "package", "module", "class", "function"],
     Callable[[str, Config], Literal["session", "package", "module", "class", "function"]],
```

### Comparing `pyfactories-1.0.0/pyfactories/value_generators/complex_types.py` & `pyfactories-2.0.0/pyfactories/value_generators/complex_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import random
 from collections import defaultdict, deque
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Type, Union, cast
 
-from pydantic.fields import (
+from pydantic.v1.fields import (
     SHAPE_DEFAULTDICT,
     SHAPE_DEQUE,
     SHAPE_DICT,
     SHAPE_FROZENSET,
     SHAPE_ITERABLE,
     SHAPE_LIST,
     SHAPE_MAPPING,
```

### Comparing `pyfactories-1.0.0/pyfactories/value_generators/constrained_number.py` & `pyfactories-2.0.0/pyfactories/value_generators/constrained_number.py`

 * *Files identical despite different names*

### Comparing `pyfactories-1.0.0/pyfactories/value_generators/primitives.py` & `pyfactories-2.0.0/pyfactories/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `pyfactories-1.0.0/pyfactories/value_generators/regex.py` & `pyfactories-2.0.0/pyfactories/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `pyfactories-1.0.0/LICENSE` & `pyfactories-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfactories-1.0.0/README.md` & `pyfactories-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # PyFactories
 
 <p align="center">
-  <a href="https://esmerald.dymmond.com"><img src="https://res.cloudinary.com/tarsild/image/upload/v1687347327/packages/pyfactories/logo_lvtl5d.png" alt='Esmerald'></a>
+  <a href="https://pyfactories.tarsild.io"><img src="https://res.cloudinary.com/tarsild/image/upload/v1687347327/packages/pyfactories/logo_lvtl5d.png" alt='PyFactories'></a>
 </p>
 
 
 <p align="center">
     <em>🚀 Mock data generation for pydantic and dataclasses. 🚀</em>
 </p>
 
@@ -23,15 +23,15 @@
 </a>
 </p>
 
 ---
 
 **Documentation**: [https://pyfactories.tarsild.io][docs] 📚
 
-**Source Code**: [https://github.com/dymmond/esmerald][github]
+**Source Code**: [https://github.com/tarsil/pyfactories][github]
 
 ---
 
 ## Motivation
 
 [Pydantic Factories][pydantic_factories] was initially created and used by a lot of people and it
 is an extremely powerful package that was heavily tested by the same authors of Starlite, now,
```

### Comparing `pyfactories-1.0.0/pyproject.toml` & `pyfactories-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "faker>=18.11.1,<30.0.0",
-    "pydantic>=1.10.9,<2.0.0",
+    "pydantic>=2.0.0,<3.0.0",
+    "pydantic-extra-types>=2.0.0,<3.0.0",
     "typing-extensions>=4.6.3,<7.0.0",
 ]
 keywords = ["pyfactories"]
 
 [project.urls]
 Homepage = "https://github.com/tarsil/pyfactories"
 Documentation = "https://pyfactories.tarsild.io"
@@ -58,15 +59,14 @@
     "isort>=5.12.0,<6.0.0",
     "mypy>=1.1.0,<2.0.0",
     "pytest>=7.2.2,<8.0.0",
     "pytest-asyncio>=0.21.0,<1.0.0",
     "pytest-cov>=4.0.0,<5.0.0",
     "requests>=2.28.2",
     "ruff>=0.0.256,<1.0.0",
-    "saffier[testing,postgres]>=0.13.0",
 ]
 
 dev = [
     "email-validator>=2.0.0.post2,<4.0.0",
     "hypothesis>=6.79.1,<7.0.0",
     "ipdb>=0.13.13,<1.0.0",
     "pre-commit>=3.3.1,<4.0.0",
```

### Comparing `pyfactories-1.0.0/PKG-INFO` & `pyfactories-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfactories
-Version: 1.0.0
+Version: 2.0.0
 Summary: Mock data generation for pydantic and dataclasses
 Project-URL: Homepage, https://github.com/tarsil/pyfactories
 Project-URL: Documentation, https://pyfactories.tarsild.io
 Project-URL: Changelog, https://pyfactories.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/pyfactories
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -33,15 +33,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: faker<30.0.0,>=18.11.1
-Requires-Dist: pydantic<2.0.0,>=1.10.9
+Requires-Dist: pydantic-extra-types<3.0.0,>=2.0.0
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Requires-Dist: typing-extensions<7.0.0,>=4.6.3
 Provides-Extra: dev
 Requires-Dist: email-validator<4.0.0,>=2.0.0.post2; extra == 'dev'
 Requires-Dist: hypothesis<7.0.0,>=6.79.1; extra == 'dev'
 Requires-Dist: ipdb<1.0.0,>=0.13.13; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.3.1; extra == 'dev'
 Provides-Extra: doc
@@ -58,21 +59,20 @@
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
 Requires-Dist: mypy<2.0.0,>=1.1.0; extra == 'test'
 Requires-Dist: pytest-asyncio<1.0.0,>=0.21.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.2.2; extra == 'test'
 Requires-Dist: requests>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
-Requires-Dist: saffier[postgres,testing]>=0.13.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # PyFactories
 
 <p align="center">
-  <a href="https://esmerald.dymmond.com"><img src="https://res.cloudinary.com/tarsild/image/upload/v1687347327/packages/pyfactories/logo_lvtl5d.png" alt='Esmerald'></a>
+  <a href="https://pyfactories.tarsild.io"><img src="https://res.cloudinary.com/tarsild/image/upload/v1687347327/packages/pyfactories/logo_lvtl5d.png" alt='PyFactories'></a>
 </p>
 
 
 <p align="center">
     <em>🚀 Mock data generation for pydantic and dataclasses. 🚀</em>
 </p>
 
@@ -90,15 +90,15 @@
 </a>
 </p>
 
 ---
 
 **Documentation**: [https://pyfactories.tarsild.io][docs] 📚
 
-**Source Code**: [https://github.com/dymmond/esmerald][github]
+**Source Code**: [https://github.com/tarsil/pyfactories][github]
 
 ---
 
 ## Motivation
 
 [Pydantic Factories][pydantic_factories] was initially created and used by a lot of people and it
 is an extremely powerful package that was heavily tested by the same authors of Starlite, now,
```

