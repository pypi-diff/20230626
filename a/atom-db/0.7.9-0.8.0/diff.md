# Comparing `tmp/atom_db-0.7.9-py3-none-any.whl.zip` & `tmp/atom_db-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 34281 bytes, number of entries: 10
+Zip file size: 36408 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 19-Feb-27 13:13 atomdb/__init__.py
--rw-rw-r--  2.0 unx    27746 b- defN 22-Dec-16 02:59 atomdb/base.py
+-rw-rw-r--  2.0 unx    27962 b- defN 23-May-17 14:23 atomdb/base.py
 -rw-rw-r--  2.0 unx     5342 b- defN 22-Feb-18 19:09 atomdb/nosql.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-May-16 17:32 atomdb/py.typed
--rw-rw-r--  2.0 unx    69915 b- defN 22-Aug-07 21:15 atomdb/sql.py
--rw-rw-r--  2.0 unx     1063 b- defN 22-Dec-16 03:14 atom_db-0.7.9.dist-info/LICENSE
--rw-rw-r--  2.0 unx    15347 b- defN 22-Dec-16 03:14 atom_db-0.7.9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Dec-16 03:14 atom_db-0.7.9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 22-Dec-16 03:14 atom_db-0.7.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      742 b- defN 22-Dec-16 03:14 atom_db-0.7.9.dist-info/RECORD
-10 files, 120254 bytes uncompressed, 33031 bytes compressed:  72.5%
+-rw-rw-r--  2.0 unx    80448 b- defN 23-May-17 14:23 atomdb/sql.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-May-17 14:25 atom_db-0.8.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    15311 b- defN 23-May-17 14:25 atom_db-0.8.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 14:25 atom_db-0.8.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-17 14:25 atom_db-0.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      742 b- defN 23-May-17 14:25 atom_db-0.8.0.dist-info/RECORD
+10 files, 130967 bytes uncompressed, 35158 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: atomdb/py.typed
 Comment: 
 
 Filename: atomdb/sql.py
 Comment: 
 
-Filename: atom_db-0.7.9.dist-info/LICENSE
+Filename: atom_db-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: atom_db-0.7.9.dist-info/METADATA
+Filename: atom_db-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: atom_db-0.7.9.dist-info/WHEEL
+Filename: atom_db-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: atom_db-0.7.9.dist-info/top_level.txt
+Filename: atom_db-0.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: atom_db-0.7.9.dist-info/RECORD
+Filename: atom_db-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atomdb/base.py

```diff
@@ -31,22 +31,19 @@
     Dict,
     Float,
     Instance,
     Int,
     List,
     Member,
     Property,
-    Set,
     Str,
-    Tuple,
     Typed,
     Value,
     set_default,
 )
-from bytecode import Bytecode, Instr
 
 T = TypeVar("T")
 M = TypeVar("M", bound="Model")
 ScopeType = DictType[int, Any]
 StateType = DictType[str, Any]
 GetStateFn = Callable[[M, Optional[ScopeType]], StateType]
 RestoreStateFn = Callable[[M, StateType, Optional[ScopeType]], None]
@@ -105,15 +102,15 @@
 
     """
     if isinstance(m, (Bool, Str, Int, Float)):
         return True
     if hasattr(m, "resolve"):
         # These cannot be resolved until their dependencies are available
         return None
-    if isinstance(m, (Tuple, Set, List, Typed, Instance, Dict, Coerced)):
+    if isinstance(m, (List, Typed, Instance, Dict, Coerced)):
         try:
             types = resolve_member_types(m, resolve=False)
         except UnresolvableError:
             return None
         if types is None:
             return False  # Value can be any type
         if types and all(t in (int, float, bool, str) for t in types):
@@ -201,20 +198,20 @@
 
     #: Store all registered models
     registry = Dict()
 
     #: Mapping of type name to coercer function
     coercers = Dict(
         default={
-            "datetime.date": lambda s: date(**s),
-            "datetime.datetime": lambda s: datetime(**s),
-            "datetime.time": lambda s: time(**s),
-            "bytes": lambda s: b64decode(s["bytes"]),
-            "decimal": lambda s: Decimal(s["value"]),
-            "uuid": lambda s: UUID(s["id"]),
+            "datetime.date": lambda v, scope: date(**v),
+            "datetime.datetime": lambda v, scope: datetime(**v),
+            "datetime.time": lambda v, scope: time(**v),
+            "bytes": lambda v, scope: b64decode(v["bytes"]),
+            "decimal": lambda v, scope: Decimal(v["value"]),
+            "uuid": lambda v, scope: UUID(v["id"]),
         }
     )
 
     @classmethod
     def instance(cls: Type["ModelSerializer"]) -> "ModelSerializer":
         if cls not in ModelSerializer._instances:
             ModelSerializer._instances[cls] = cls()
@@ -280,33 +277,40 @@
         Returns
         -------
         result: Object
             The unflattened object
 
         """
         if isinstance(v, dict):
+            unflatten = self.unflatten
             # Circular reference
             if scope and "__ref__" in v:
                 ref = v["__ref__"]
                 if ref in scope:
                     return scope[ref]
 
             # Create the object
             if "__model__" in v:
                 cls = self.registry[v["__model__"]]
                 return await cls.serializer.unflatten_object(cls, v, scope)
 
             # Convert py types
             if "__py__" in v:
-                coercer = self.coercers.get(v.pop("__py__"))
+                py_type = v.pop("__py__")
+                coercer = self.coercers.get(py_type)
                 if coercer:
-                    return coercer(v)
-            unflatten = self.unflatten
+                    if asyncio.iscoroutinefunction(coercer):
+                        return await coercer(v, scope)
+                    return coercer(v, scope)
+                elif py_type == "set" or py_type == "atomset":
+                    return {await unflatten(i) for i in v["values"]}
+                elif py_type == "tuple":
+                    return tuple([await unflatten(i) for i in v["values"]])
             return {k: await unflatten(i, scope) for k, i in v.items()}
-        elif isinstance(v, (list, tuple)):
+        elif isinstance(v, list):
             unflatten = self.unflatten
             return [await unflatten(item, scope) for item in v]
         return v
 
     async def unflatten_object(
         self, cls: Type["Model"], state: StateType, scope: ScopeType
     ) -> Optional["Model"]:
@@ -587,15 +591,17 @@
     # Update restored state
     template.append("self.__restored__ = True")
     source = "\n    ".join(template)
     return generate_function(source, namespace, "__restorestate__")
 
 
 def generate_function(
-    source: str, namespace: DictType[str, Any], fn_name: str, optimize: bool = True
+    source: str,
+    namespace: DictType[str, Any],
+    fn_name: str,
 ) -> Callable[..., Any]:
     """Generate an optimized function
 
     Parameters
     ----------
     source: str
         The function source code
@@ -620,22 +626,14 @@
         raise RuntimeError(f"Could not generate code: {e}:\n{source}")
 
     result: DictType[str, Any] = {}
     exec(code, namespace, result)
 
     # Optimize global access
     fn = result[fn_name]
-    fn.__source__ = source
-    if optimize:
-        bc = Bytecode.from_code(fn.__code__)
-        for i, inst in enumerate(bc):
-            name = getattr(inst, "name", None)
-            if name == "LOAD_GLOBAL" and inst.arg in namespace:
-                bc[i] = Instr("LOAD_CONST", namespace[inst.arg])
-        fn.__code__ = bc.to_code()
     return fn
 
 
 class ModelMeta(AtomMeta):
     def __new__(meta, name, bases, dct):
         cls = AtomMeta.__new__(meta, name, bases, dct)
 
@@ -814,14 +812,18 @@
             return s
         if isinstance(v, bytes):
             return {"__py__": "bytes", "bytes": b64encode(v).decode()}
         if isinstance(v, Decimal):
             return {"__py__": "decimal", "value": str(v)}
         if isinstance(v, UUID):
             return {"__py__": "uuid", "id": str(v)}
+        if isinstance(v, (tuple, set)):
+            flatten = self.flatten
+            type_name = v.__class__.__name__
+            return {"__py__": type_name, "values": [flatten(it) for it in v]}
         return super().flatten(v, scope)
 
     def flatten_object(self, obj: Model, scope: ScopeType) -> DictType[str, Any]:
         """Flatten to just json but add in keys to know how to restore it."""
         ref = obj.__ref__
         if ref in scope:
             return {"__ref__": ref, "__model__": obj.__model__}
```

## atomdb/sql.py

```diff
@@ -23,26 +23,28 @@
 from typing import Type, TypeVar, Union, cast
 
 import sqlalchemy as sa
 from atom import api
 from atom.api import (
     Atom,
     Bool,
+    Coerced,
     ContainerList,
     Dict,
     ForwardInstance,
     ForwardSubclass,
     ForwardTyped,
     Instance,
     Int,
     List,
     Member,
     Set,
     Str,
     Typed,
+    Validate,
     Value,
 )
 from sqlalchemy.engine import ddl
 from sqlalchemy.sql import schema
 from sqlalchemy.sql.type_api import TypeEngine
 
 from .base import (
@@ -51,14 +53,15 @@
     Model,
     ModelManager,
     ModelMeta,
     ModelSerializer,
     RestoreStateFn,
     ScopeType,
     StateType,
+    UnresolvableError,
     find_subclasses,
     generate_function,
     is_db_field,
     is_primitive_member,
     resolve_member_types,
 )
 
@@ -78,14 +81,31 @@
     "quote",
     "unique",
     "system",
     "comment",
 )
 FK_TYPES = (Instance, Typed, ForwardInstance, ForwardTyped)
 
+# Member types that will default to nullable=False unless tagged otherwise
+NON_NULL_MEMBERS = (
+    api.Bool,
+    api.Dict,
+    api.Str,
+    api.Int,
+    api.Float,
+    api.Range,
+    api.Enum,
+    api.FloatRange,
+    api.List,
+    api.ContainerList,
+    api.Tuple,
+    api.Set,
+    api.Bytes,
+)
+
 # kwargs reserved for the serializer
 SERIALIZE_KWARGS = ("flatten", "unflatten")
 
 # ops that can be used with django-style queries
 QUERY_OPS = {
     "eq": "__eq__",
     "gt": "__gt__",
@@ -157,35 +177,215 @@
         if meta:
             # If this is marked as abstract ignore it
             if getattr(meta, "abstract", False):
                 continue
         yield model
 
 
-class Relation(ContainerList):
+def create_related_list(kind, relation: "Relation", default: Any):
+    class RelatedList(Atom):
+        """A custom list which has methods to query a foreign key
+        one to many or many to many relation
+        """
+
+        values = List(ForwardInstance(kind), default=default)
+        owner = ForwardInstance(lambda: SQLModel)
+
+        def __init__(self, values=None, owner=None):
+            super().__init__(values=values or [], owner=owner)
+
+        def __getitem__(self, key):
+            if isinstance(key, slice):
+                return RelatedList(
+                    values=self.values[key],
+                    owner=self.owner,
+                )
+            return self.values[key]
+
+        def __delitem__(self, key):
+            del self.values[key]
+
+        def __setitem__(self, key, value):
+            self.values[key] = value
+
+        def __iter__(self):
+            return self.values.__iter__()
+
+        def __len__(self):
+            return self.values.__len__()
+
+        def __eq__(self, other):
+            return self.values == other
+
+        def __getattr__(self, name):
+            return getattr(self.values, name)
+
+        def __add__(self, other):
+            return RelatedList(
+                values=self.values + other,
+                owner=self.owner,
+            )
+
+        def copy(self):
+            return RelatedList(
+                values=self.values.copy(),
+                owner=self.owner,
+            )
+
+        async def load(self) -> list:
+            """Returns a list of the related values."""
+            owner = self.owner
+            Model = cast(Type[SQLModel], type(owner))
+            ThroughModel = relation.through
+            if ThroughModel is not None:
+                # A many to many relation case. For example:
+                #
+                #   class Pizza(SQLModel):
+                #       toppings = Relation(lambda: Topping, through=lambda: PizzaTopping)
+                #   class Topping(SQLModel):
+                #       name = Str()
+                #   class PizzaTopping(SQLModel):
+                #       pizza = Instance(Pizza)
+                #       topping = Instance(Topping)
+                #
+                # When we have:
+                #   toppings = await pizza.toppings.load()
+                # The pizza is the owner, and the toppings member is the relation.
+                # So inlining it will be the same as the following:
+                #   toppings = [
+                #      row.topping await PizzaTopping.objects.select_related(
+                #          "topping").filter(pizza=pizza)
+                #   ]
+                #
+                RelModel = relation.to
+                relation_backref = resolve_backref(RelModel, ThroughModel)
+                if relation_backref is None:
+                    raise UnresolvableError(
+                        f"relation between {RelModel} and through model {ThroughModel}"
+                        f": Tried {RelModel.__backrefs__}"
+                    )
+                owner_backref = resolve_backref(Model, ThroughModel)
+                if owner_backref is None:
+                    raise UnresolvableError(
+                        f"relation between {Model} and through model {ThroughModel}"
+                        f": Tried {Model.__backrefs__}"
+                    )
+                return [
+                    getattr(row, relation_backref.name)
+                    for row in await ThroughModel.objects.select_related(
+                        relation_backref.name
+                    ).filter(**{owner_backref.name: owner})
+                ]
+            # A many to one relation case. For example:
+            #
+            #   class Page(SQLModel):
+            #       comments = Relation(lambda: Comment)
+            #   class Comment(SQLModel):
+            #       page = Instance(Page)
+            #
+            # When we have:
+            #   comments = await page.comments.load()
+            # The page is the owner, and the comments member is the relation.
+            # So inlining it will be the same as the following:
+            #   comments = await Comments.objects.filter(page=page)
+            RelModel = relation.to
+            owner_backref = resolve_backref(Model, RelModel)
+            if owner_backref is None:
+                raise UnresolvableError(
+                    f"relation between {Model} and {RelModel}"
+                    f": Tried {Model.__backrefs__}"
+                )
+            return await RelModel.objects.filter(**{owner_backref.name: owner})
+
+        async def save(self, connection=None):
+            """Save the current list as the complete set of related items. This
+            should only be used for small sets of items.
+            """
+            owner = self.owner
+            assert owner is not None
+            current = set(self)
+            saved = set(await self.load())
+            ThroughModel = relation.through
+            if ThroughModel is not None:
+                Model = cast(Type[SQLModel], type(owner))
+                RelModel = relation.to
+                owner_backref = resolve_backref(Model, ThroughModel)
+                relation_backref = resolve_backref(RelModel, ThroughModel)
+                removed_ids = [obj._id for obj in saved.difference(current)]
+
+                if removed_ids:
+                    # Remove old
+                    await ThroughModel.objects.filter(
+                        **{
+                            owner_backref.name: owner,
+                            f"{relation_backref.name}__in": removed_ids,
+                        }
+                    ).delete(connection=connection)
+
+                # Add new
+                for added_item in current.difference(saved):
+                    await ThroughModel.objects.create(
+                        **{
+                            owner_backref.name: owner,
+                            relation_backref.name: added_item,
+                        }
+                    )
+            else:
+                for removed_item in saved.difference(current):
+                    await removed_item.delete(connection=connection)
+                for added_item in current.difference(saved):
+                    await added_item.save(connection=connection)
+
+    return RelatedList
+
+
+class Relation(Coerced):
     """A member which serves as a fk relation backref"""
 
-    __slots__ = ("_to",)
+    __slots__ = ("_to", "_through", "type")
 
-    def __init__(self, item: CallableType[[], Type[Model]], default=None):
-        super().__init__(ForwardInstance(item), default=default)  # type: ignore
+    def __init__(
+        self,
+        item: CallableType[[], Type[Model]],
+        default: Any = None,
+        *,
+        through: CallableType[[], Optional[Type[Model]]] = lambda: None,
+    ):
+        RelatedList = create_related_list(item, self, default)
+        super().__init__(RelatedList)  # type: ignore
+        self.type = RelatedList
         self._to: Optional[Type[Model]] = None
+        self._through = through
+        self.tag(store=False)
+        self.set_post_setattr_mode(
+            api.PostSetAttr.MemberMethod_ObjectOldNew, "post_setattr"
+        )
+
+    def post_setattr(self, obj: Model, old: Any, new: Any):
+        """Set owner of RelatedList"""
+        new.owner = obj
+        return new
 
     def resolve(self) -> Type[Model]:
         return self.to
 
     @property
     def to(self) -> Type[Model]:
         to = self._to
         if to is None:
-            types = resolve_member_types(self.validate_mode[-1])
+            types = resolve_member_types(self.type.values.validate_mode[-1])
             assert types is not None
             to = self._to = types[0]
         return to
 
+    @property
+    def through(self) -> Optional[Type[Model]]:
+        """Return the through model"""
+        return self._through()
+
 
 class RelatedInstance(ForwardInstance):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)  # type: ignore
         self.tag(store=False)
 
 
@@ -308,14 +508,24 @@
     col = model.objects.table.columns.get(field)
     if col is None:
         raise ValueError("Invalid field %s on %s" % (field, model))
     return col, related_clauses
 
 
 @functools.lru_cache(1024)
+def resolve_backref(model: Type["SQLModel"], through: Type["SQLModel"]) -> Member:
+    """Find the member on the through model that refers to the given model."""
+    assert model.objects and through.objects  # Force creation
+    for other_model, referring_member in model.__backrefs__:
+        if other_model is through:
+            return referring_member
+    raise ValueError(f"No backref relation found between {model} and {through}")
+
+
+@functools.lru_cache(1024)
 def resolve_relation(
     model: Type["SQLModel"], field: str
 ) -> TupleType[Member, Type[Model], Member, sa.Column]:
     """Lookup a Relation.
 
     Parameters
     ----------
@@ -342,14 +552,16 @@
         # instead of prefetch related.
         types = resolve_member_types(relation)
         if types and len(types) == 1 and issubclass(types[0], Model):
             # RelModel has a one to one relation back to model
             RelModel = types[0]
 
     if RelModel is not None:
+        assert model.objects and RelModel.objects  # Force creation
+
         m = cast(Member, relation)
         # Find the referring member
         # TODO: This does not support multiple backrefs
         for other_model, referring_member in model.__backrefs__:
             if RelModel is other_model:
                 meta = referring_member.metadata or {}
                 name = meta.get("name", referring_member.name)
@@ -383,15 +595,17 @@
     elif isinstance(member, api.Range):
         # TODO: Add min / max
         return sa.Integer()
     elif isinstance(member, api.FloatRange):
         # TODO: Add min / max
         return sa.Float()
     elif isinstance(member, api.Enum):
-        return sa.Enum(*member.items, name=member.name)
+        model_name = model.__model__.replace(".", "_")
+        enum_name = f"{model_name}_{member.name}"
+        return sa.Enum(*member.items, name=enum_name)
     elif hasattr(api, "IntEnum") and isinstance(member, api.IntEnum):  # type: ignore
         return sa.SmallInteger()
     elif isinstance(member, FK_TYPES):
         value_type = resolve_member_types(member)
         if value_type is None:
             raise TypeError("Instance and Typed members must specify types")
         return py_type_to_sql_column(model, member, value_type, **kwargs)
@@ -402,23 +616,23 @@
             raise TypeError("Relation members must specify types")
 
         # Resolve the item type
         value_type = resolve_member_types(item_type)
         if value_type is None:
             raise TypeError("Relation members must specify types")
         return None  # Relations are just syntactic sugar
-    elif isinstance(member, (api.List, api.ContainerList, api.Tuple)):
+    elif isinstance(member, (api.List, api.ContainerList, api.Tuple, api.Set)):
         item_type = member.validate_mode[-1]
         if item_type is None:
-            raise TypeError("List and Tuple members must specify types")
+            raise TypeError("List, Set, and Tuple members must specify types")
 
         # Resolve the item type
         value_type = resolve_member_types(item_type)
         if value_type is None:
-            raise TypeError("List and Tuple members must specify types")
+            raise TypeError("List, Set, and Tuple members must specify types")
         if issubclass(value_type[0], JSONModel):
             return sa.JSON(**kwargs)
         t = py_type_to_sql_column(model, member, value_type, **kwargs)
         if isinstance(t, tuple):
             t = t[0]  # Use only the value type
         return sa.ARRAY(t)
     elif isinstance(member, api.Bytes):
@@ -472,24 +686,40 @@
 
     # Extract column kwargs from member metadata
     kwargs = {}
     for k in COLUMN_KWARGS:
         if k in metadata:
             kwargs[k] = metadata.pop(k)
 
+    # Set default nullable value
+    if "nullable" not in kwargs:
+        if "primary_key" in kwargs:
+            kwargs["nullable"] = False
+        elif isinstance(member, NON_NULL_MEMBERS):
+            kwargs["nullable"] = False
+        elif hasattr(member, "optional"):
+            kwargs["nullable"] = member.optional  # type: ignore
+        elif isinstance(member, Typed):
+            optional = member.validate_mode[0] == Validate.OptionalTyped
+            kwargs["nullable"] = optional
+        elif isinstance(member, Instance):
+            optional = member.validate_mode[0] == Validate.OptionalInstance
+            kwargs["nullable"] = optional
+
     if column_type is None:
         args = atom_member_to_sql_column(model, member, **metadata)
         if args is None:
             return None
         if not isinstance(args, (tuple, list)):
             args = (args,)
     elif isinstance(column_type, (tuple, list)):
         args = column_type
     else:
         args = (column_type,)
+
     return sa.Column(column_name, *args, **kwargs)
 
 
 def create_table(model: Type["SQLModel"], metadata: sa.MetaData) -> sa.Table:
     """Create an sqlalchemy table by inspecting the Model and generating
     a column for each member.
 
@@ -955,32 +1185,77 @@
         return self.__class__(**state)
 
     def query(self, query_type: str = "select", *columns, **kwargs):
         if kwargs:
             return self.filter(**kwargs).query(query_type)
         p = self.proxy
         from_table = p.table
-        tables = [from_table]
-        model = p.model
+        tables = {from_table}
         use_labels = bool(self.related_clauses)
         outer_join = self.outer_join
+        existing_joins = set()
         for clause in self.related_clauses:
-            rel_model = model
+            model = p.model
+            table = p.table
 
             # Walk the fk relations
+            alias = []
             for part in clause.split("__"):
-                m = rel_model.members().get(part)
-                assert m is not None, f"{rel_model} has no field {part}"
+                m = model.members().get(part)
+                assert m is not None, f"{model} has no field {part}"
+                assert issubclass(model, SQLModel)
+
+                alias.append(part)
                 rel_model_types = resolve_member_types(m)
                 assert rel_model_types is not None
                 rel_model = rel_model_types[0]
-                assert issubclass(rel_model, Model)
-                table = rel_model.objects.table
-                from_table = from_table.join(table, isouter=outer_join)
-                tables.append(table)
+                assert issubclass(rel_model, SQLModel)
+                rel_table = rel_model.objects.table
+
+                # For example:
+                # class Job(SQLModel):
+                #    status = Str()
+                #    roles = Relation(Role)
+                # class Role(SQLModel):
+                #    name = Str()
+                #    job = Instance(Job)
+                if isinstance(m, Relation):
+                    # Case when looking though the relation
+                    # r = await Job.objects.filter(roles__name="foo")
+                    backref = resolve_backref(model, m.through or rel_model)
+                    rel_key = backref.name
+                    self_key = model.__pk__
+                else:
+                    # Normal foreign key cases or select related
+                    # r = await JobRole.objects.filter(job__status="live")
+                    rel_key = rel_model.__pk__
+                    self_key = m.name
+
+                # Handled renamed fields
+                if self_key in model.__renamed_fields__:
+                    self_key = model.__renamed_fields__[self_key]
+                if rel_key in rel_model.__renamed_fields__:
+                    rel_key = rel_model.__renamed_fields__[rel_key]
+
+                join_key = (model, self_key, rel_model, rel_key)
+
+                # Avoid duplicate join, eg `select_related('a', 'a__b")`
+                # would join on a twice.
+                # TODO: Cannot join the same table twice, need to use alias
+                # where `select_related('a__b', 'a__b")`
+                if join_key not in existing_joins:
+                    onclause = table.c[self_key] == rel_table.c[rel_key]
+                    from_table = from_table.join(
+                        rel_table, onclause=onclause, isouter=outer_join
+                    )
+                    existing_joins.add(join_key)
+
+                tables.add(rel_table)
+                model = rel_model
+                table = rel_table
 
         if query_type == "select":
             q = sa.select(columns or tables, use_labels=use_labels).select_from(
                 from_table
             )
         elif query_type == "delete":
             q = sa.delete(from_table)
@@ -1002,15 +1277,14 @@
             q = q.order_by(*self.order_clauses)
 
         if self.limit_count:
             q = q.limit(self.limit_count)
 
         if self.query_offset:
             q = q.offset(self.query_offset)
-
         return q
 
     def select_related(
         self, *related: Sequence[str], outer_join: Optional[bool] = None
     ) -> "SQLQuerySet[T]":
         """Define related fields to join in the query.
 
@@ -2019,15 +2293,14 @@
             raise ValueError("Cannot use force_insert and force_update together")
 
         db = self.objects
         table = db.table
         state = self.__prepare_state_for_db__()
         async with db.connection(connection) as conn:
             if force_update or (self._id and not force_insert):
-
                 # If update fields was given, only pass those
                 if update_fields is not None:
                     # Replace any update fields with the appropriate name
                     renamed = self.__renamed_fields__
                     update_fields = [renamed.get(f, f) for f in update_fields]
 
                     # Replace update fields with only those given
```

## Comparing `atom_db-0.7.9.dist-info/LICENSE` & `atom_db-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `atom_db-0.7.9.dist-info/METADATA` & `atom_db-0.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: atom-db
-Version: 0.7.9
+Version: 0.8.0
 Summary: Database abstraction layer for atom objects
 Home-page: https://github.com/codelv/atom-db
 Author: CodeLV
 Author-email: frmdstryr@gmail.com
 License: MIT
+Platform: UNKNOWN
 Requires: atom
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: atom (>=0.7.0)
-Requires-Dist: bytecode
 
 [![status](https://github.com/codelv/atom-db/actions/workflows/ci.yml/badge.svg)](https://github.com/codelv/atom-db/actions)
 [![codecov](https://codecov.io/gh/codelv/atom-db/branch/master/graph/badge.svg)](https://codecov.io/gh/codelv/atom-db)
 
 atom-db is a database abstraction layer for the
 [atom](https://github.com/nucleic/atom) framework. This package provides api's for
 seamlessly saving and restoring atom objects from json based document databases
@@ -33,17 +33,14 @@
 ### Overview
 
 - Supports MySQL and Postgres
 - Uses django like queries or raw sqlalchemy queries
 - Works with alembic database migrations
 - Supports MongoDB using motor
 
-It's still in development....
-
-
 ### Structure
 
 The design is based somewhat on django.
 
 There is a "manager" called `Model.objects` to do queries on the database table
 created for each subclass.
 
@@ -502,7 +499,9 @@
 
 ## Contributing
 
 This is currently used in a few projects but not considered mature by
 any means.
 
 Pull requests and feature requests are welcome!
+
+
```

