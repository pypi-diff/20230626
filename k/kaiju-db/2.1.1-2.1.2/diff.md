# Comparing `tmp/kaiju_db-2.1.1-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,14 @@
-Zip file size: 22984 bytes, number of entries: 17
--rw-r--r--  2.0 unx      282 b- defN 23-Jun-15 16:09 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3127 b- defN 23-Jun-15 16:09 kaiju_db/fixtures.py
--rw-r--r--  2.0 unx     3665 b- defN 23-Jun-15 16:09 kaiju_db/functions.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jun-15 16:09 kaiju_db/ltree.py
--rw-r--r--  2.0 unx     4522 b- defN 23-Jun-15 16:09 kaiju_db/migrations.py
--rw-r--r--  2.0 unx      386 b- defN 23-Jun-15 16:09 kaiju_db/services.py
--rw-r--r--  2.0 unx    39661 b- defN 23-Jun-15 16:09 kaiju_db/sql_service.py
--rw-r--r--  2.0 unx     9761 b- defN 23-Jun-15 16:09 kaiju_db/transport.py
--rw-r--r--  2.0 unx      206 b- defN 23-Jun-15 16:09 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-15 16:09 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3568 b- defN 23-Jun-15 16:09 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx    13635 b- defN 23-Jun-15 16:09 kaiju_db/tests/test_services.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-15 16:09 kaiju_db-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3090 b- defN 23-Jun-15 16:09 kaiju_db-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 16:09 kaiju_db-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-15 16:09 kaiju_db-2.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1332 b- defN 23-Jun-15 16:09 kaiju_db-2.1.1.dist-info/RECORD
-17 files, 84150 bytes uncompressed, 20814 bytes compressed:  75.3%
+Zip file size: 19507 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-26 16:22 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3665 b- defN 23-Jun-26 16:22 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    57079 b- defN 23-Jun-26 16:22 kaiju_db/services.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-26 16:22 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:22 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3240 b- defN 23-Jun-26 16:22 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4125 b- defN 23-Jun-26 16:22 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3090 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jun-26 16:22 kaiju_db-2.1.2.dist-info/RECORD
+12 files, 73485 bytes uncompressed, 17935 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,52 +1,37 @@
 Filename: kaiju_db/__init__.py
 Comment: 
 
-Filename: kaiju_db/fixtures.py
-Comment: 
-
 Filename: kaiju_db/functions.py
 Comment: 
 
-Filename: kaiju_db/ltree.py
-Comment: 
-
-Filename: kaiju_db/migrations.py
-Comment: 
-
 Filename: kaiju_db/services.py
 Comment: 
 
-Filename: kaiju_db/sql_service.py
-Comment: 
-
-Filename: kaiju_db/transport.py
-Comment: 
-
 Filename: kaiju_db/types.py
 Comment: 
 
 Filename: kaiju_db/tests/__init__.py
 Comment: 
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
-Filename: kaiju_db/tests/test_services.py
+Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.1.dist-info/LICENSE
+Filename: kaiju_db-2.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.1.dist-info/METADATA
+Filename: kaiju_db-2.1.2.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.1.dist-info/WHEEL
+Filename: kaiju_db-2.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.1.dist-info/top_level.txt
+Filename: kaiju_db-2.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.1.dist-info/RECORD
+Filename: kaiju_db-2.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,12 +1,8 @@
 from .types import *
-from .ltree import *
 from .functions import *
-from .migrations import *
-from .transport import *
-from .sql_service import *
-from .fixtures import *
+from .services import *
 
-__version__ = '2.1.1'
+__version__ = '2.1.2'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/services.py

```diff
@@ -1,9 +1,1472 @@
-from kaiju_tools.app import service_class_registry
-from .transport import DatabaseService
-from .migrations import DatabaseMigrationService
-from .sql_service import SQLService
-from .fixtures import FixtureService
+"""Database services."""
+
+import abc
+from pathlib import Path
+from typing import cast, List, Collection, TypedDict, AsyncGenerator, Union, Optional
+
+import sqlalchemy as sa
+import sqlalchemy.dialects.postgresql as sa_pg
+from sqlalchemy.exc import IntegrityError
+from sqlalchemy.sql.expression import nullslast
+from sqlalchemy import MetaData, text, Table  # noqa pycharm
+from sqlalchemy.ext.asyncio import create_async_engine  # noqa pycharm
+
+from kaiju_tools.app import ContextableService, service_class_registry, Service
+from kaiju_tools.interfaces import DataStore
+from kaiju_tools.exceptions import ValidationError, NotFound, Conflict, InternalError, MethodNotAllowed
+from kaiju_tools.serialization import dumps, loads, load
+from kaiju_db.functions import functions_registry, UserFunction
+
+__all__ = ['DatabaseService', 'SQLService', 'FixtureService', 'DatabaseMigrationService']
+
+
+class DatabaseService(ContextableService):
+    """Postgresql database transport service.
+
+    Initializes a connection pool and can provide connections and basic execution commands. It also can perform initial
+    database, functions and tables initialization.
+    """
+
+    service_name = 'db'
+
+    def __init__(
+        self,
+        app,
+        *,
+        host: str,
+        port: str,
+        database: str,
+        user: str,
+        password: str,
+        root_user: str = '',
+        root_password: str = '',
+        root_database: str = 'postgres',
+        metadata: MetaData = None,
+        init_db: bool = True,
+        init_tables: bool = True,
+        pool_size: int = 10,
+        idle_connection_lifetime: int = 3600,
+        extensions: List[str] = None,
+        functions=functions_registry,
+        logger=None,
+    ):
+        """Initialize.
+
+        :param app:
+        :param host: db url or address
+        :param port: db port
+        :param database: db name
+        :param user: db user (non-root)
+        :param password: db user password (non-root)
+        :param root_user: root user is required only for database and extensions initialization
+        :param root_password: root user is required only for database and extensions initialization
+        :param root_database: root db is required only for database and extensions initialization
+        :param metadata: optional SA metadata object
+        :param init_db: perform database and pg extensions initialization upon start (requires root credentials)
+        :param init_tables: initialize tables upon start (in not present)
+        :param pool_size: connection pool size
+        :param idle_connection_lifetime: connection idle lifetime before recycling
+        :param extensions: list of pg extensions to init (init_db flag should be enabled)
+        :param functions: optional function registry for pre-defined functions
+        :param logger:
+        """
+        super().__init__(app, logger)
+        self.metadata = metadata if metadata else MetaData()
+        self._host = host
+        self._port = port
+        self._db = database
+        self._user = user
+        self._password = password
+        self._root_user = root_user if root_user else user
+        self._root_password = root_password if root_password else password
+        self._root_database = root_database
+        self._init_db = init_db
+        self._init_tables = any((init_tables, init_db))
+        self._pool_size = pool_size
+        self._idle_connection_lifetime = idle_connection_lifetime
+        self._extensions = extensions
+        self._functions_registry = functions
+        self._engine = None
+
+    @property
+    def engine(self):
+        """Alias to the SA async engine."""
+        return self._engine
+
+    def begin(self, *args, **kws):
+        """Alias to the SA engine transaction begin.
+
+        .. code-block:: python
+
+            async with db.begin() as conn:
+                ...  # transaction block
+                await conn.commit()
+
+        """
+        return self.engine.begin(*args, **kws)
+
+    def connect(self, *args, **kws):
+        """Alias to the SA engine connection.
+
+        .. code-block:: python
+
+            async with db.connect() as conn:
+                ...
+                await conn.commit()
+
+        """
+        return self.engine.connect(*args, **kws)
+
+    async def execute(self, __obj, *args, _commit=True, _conn=None, **kws):
+        """Execute an SQL command."""
+        if type(__obj) is str:
+            __obj = text(__obj)
+        if _conn:
+            result = await _conn.execute(__obj, *args, **kws)
+        else:
+            async with self._engine.connect() as conn:
+                result = await conn.execute(__obj, *args, **kws)
+                if _commit:
+                    await conn.commit()
+        return result
+
+    async def fetchrow(self, __obj, *args, _commit=True, _conn=None, **kws):
+        """Execute an SQL command and fetch the first result."""
+        result = await self.execute(__obj, *args, _commit=_commit, _conn=_conn, **kws)
+        result = result.first()
+        return result._asdict() if result else None  # noqa
+
+    async def fetch(self, __obj, *args, _commit=True, _conn=None, **kws):
+        """Execute an SQL command and fetch all results."""
+        result = await self.execute(__obj, *args, _commit=_commit, _conn=_conn, **kws)
+        return [r._asdict() for r in result.all()]  # noqa
+
+    async def fetchval(self, __obj, *args, _commit=True, _conn=None, **kws):
+        """Execute an SQL command and fetch a first column in the first result."""
+        result = await self.execute(__obj, *args, _commit=_commit, _conn=_conn, **kws)
+        return result.scalar()
+
+    async def init(self):
+        if self._init_db:
+            await self._init_database()
+        # self._root_user = None
+        # self._root_password = None
+        self._engine = self._create_engine(self._user, self._password, self._db)
+        if self._init_tables:
+            async with self._engine.connect() as conn:
+                await conn.execution_options(**{'isolation_level': 'AUTOCOMMIT'})
+                await self._create_functions(conn)
+                await conn.run_sync(self.metadata.create_all, checkfirst=True)
+
+    async def close(self):
+        if self._engine:
+            await self._engine.dispose()
+            self._engine = None
+
+    def add_table(self, table: Table) -> Table:
+        """Register a table in SA metadata.
+
+        This method must be called before async init if you want to automatically create this table at start time.
+        """
+        if table.name in self.metadata:
+            return self.metadata.tables[table.name]
+        else:
+            self.metadata._add_table(table.name, None, table)  # noqa
+            table.metadata = self.metadata
+            return table
+
+    async def _init_database(self):
+        # root pool for root db
+        engine = self._create_engine(self._root_user, self._root_password, self._root_database)
+        async with engine.connect() as conn:
+            await conn.execution_options(**{'isolation_level': 'AUTOCOMMIT'})
+            if not await self._db_exists(conn):
+                await self._create_db(conn)
+            if not await self._user_exists(conn):
+                await self._create_user(conn)
+        await engine.dispose()
+        if self._extensions:
+            # postgres can create extension only if superuser :-(
+            engine = self._create_engine(self._root_user, self._root_password, self._db)
+            async with engine.connect() as conn:
+                await conn.execution_options(**{'isolation_level': 'AUTOCOMMIT'})
+                for ext in self._extensions:
+                    await self._create_extension(conn, ext)
+            await engine.dispose()
+
+    def _create_engine(self, user: str, password: str, db: str):
+        self.logger.debug('Initializing a pool for user "%s" in database "%s".', user, db)
+        engine = create_async_engine(
+            f'postgresql+asyncpg://{user}:{password}@{self._host}:{self._port}/{db}',
+            json_serializer=dumps,
+            json_deserializer=loads,
+            pool_size=self._pool_size,
+            pool_recycle=self._idle_connection_lifetime,
+        )
+        return engine
+
+    async def _db_exists(self, conn) -> bool:
+        self.logger.debug('Checking database "%s".', self._db)
+        result = await conn.execute(text(f"SELECT 1 FROM pg_database WHERE datname = '{self._db}';"))  # noqa
+        return bool(result.first())
+
+    async def _create_db(self, conn) -> None:
+        self.logger.info('Creating database "%s".', self._db)
+        await conn.execute(text(f"CREATE DATABASE {self._db} WITH ENCODING 'UTF8';"))  # noqa
+
+    async def _user_exists(self, conn) -> bool:
+        self.logger.debug('Checking user "%s".', self._user)
+        result = await conn.execute(text(f"SELECT 1 FROM pg_roles WHERE rolname='{self._user}';"))  # noqa
+        return bool(result.first())
+
+    async def _create_user(self, conn) -> None:
+        self.logger.info('Creating user "%s".', self._user)
+        await conn.execute(text(f"CREATE ROLE {self._user} WITH LOGIN PASSWORD '{self._password}';"))
+        await conn.execute(text(f'GRANT CONNECT ON DATABASE {self._db} TO {self._user};'))
+        await conn.execute(text(f'GRANT pg_read_all_data TO {self._user};'))
+        await conn.execute(text(f'GRANT pg_write_all_data TO {self._user};'))
+        await conn.execute(text(f'GRANT EXECUTE ON ALL FUNCTIONS IN SCHEMA public TO {self._user};'))
+        await conn.execute(text(f'GRANT USAGE, SELECT ON ALL SEQUENCES IN SCHEMA public TO {self._user};'))
+
+    async def _create_extension(self, conn, ext: str) -> None:
+        self.logger.info('Creating extension "%s" in database "%s".', ext, self._db)
+        result = await conn.execute(text(f"SELECT 1 FROM pg_extension WHERE extname='{ext}';"))  # noqa
+        if not result.first():
+            await conn.execute(text(f'CREATE EXTENSION "{ext}";'))
+
+    async def _create_functions(self, conn):
+        for _function_key in self._functions_registry:
+            _function = self._functions_registry[_function_key]
+            if issubclass(_function, UserFunction):
+                _function = _function.sql()
+            await conn.execute(text(f'CREATE OR REPLACE {_function}'))
+
+
+class SQLService(Service, DataStore, abc.ABC):
+    """Base SQL service interface with common commands and errors.
+
+    Optimized for a single primary key only with a name "id"
+
+    Example of use:
+
+    You need to set your own table and, if needed, define column whitelists
+    for different operations.
+
+    .. code-block:: python
+
+        class MyService(SQLService):
+            table = my_table
+            select_columns = {'id', 'data', 'flag'}
+            insert_columns = {'data', 'flag'}
+            update_columns = {'flag'}
+
+    Here you can access some basic methods: "exists", "get", "create", "update",
+    "delete" and their bulk versions (for multiple objects at once).
+
+    You can change any of SQL base for these commands by redefining query
+    constructors.
+
+    .. code-block:: python
+
+        class MyService(SQLService):
+
+            ...
+
+            def _create_get_query(id, columns, table=None):
+                ... # custom query
+
+            def _create_m_get_query(self, id: list, columns, table=None):
+                ... # custom query
+
+    :param app: web app instance
+    :param database_service: database service instance or instance name
+    :param logger: optional logger instance
+    """
+
+    class _List(TypedDict):
+        """Type hinting for a list query."""
+
+        count: Optional[int]  #: total rows matching the query, None if count hasn't been requested
+        offset: int  #: row offset for this selection
+        page: Optional[int]  #: current page number, None if count hasn't been requested
+        pages: Optional[int]  #: total pages, None if count hasn't been requested
+        on_page: int  #: number of rows on this page
+        data: Optional[List[dict]]  #: returned rows, None if limit was set to 0
+
+    class ErrorCode:
+        """These error codes should be commonly used for SQL related errors."""
+
+        EXISTS = 'query.exists'
+        REFERENCE_NOT_FOUND = 'query.reference_not_found'
+        NOT_FOUND = 'query.not_found'
+        INTERNAL_ERROR = 'query.internal_error'
+        FIELD_DOES_NOT_EXISTS = 'query.field_does_not_exists'
+        INVALID_CONDITION = 'query.invalid_condition_command'
+        INVALID_ORDERING = 'query.invalid_ordering_command'
+        INVALID_PAGINATION_OFFSET = 'query.invalid_pagination_offset'
+        INVALID_PAGINATION_LIMIT = 'query.invalid_pagination_limit'
+        INVALID_COLUMN = 'query.invalid_insert_column'
+
+    DEFAULT_ROW_LIMIT = 24  #: defaults of LIMIT on queries
+    MAX_ROW_LIMIT = 1000  #: max size of queries
+
+    select_columns = None  #: you can specify a whitelist of output columns here
+    select_columns_blacklist = None
+    update_columns = None  #: you may specify columns for update here
+    update_columns_blacklist = None
+    insert_columns = None  #: you may specify insert columns here
+    insert_columns_blacklist = None
+    table = None  #: here should be your table
+
+    virtual_columns = None  # virtual SQL columns (i.e. functions) names and definitions
+    # virtual columns can be selected but never updated / inserted
+
+    def __init__(self, app, database_service: Union[DatabaseService, str] = None, logger=None):
+        """Initialize."""
+
+        def _prepare_whitelist(whitelist, blacklist):
+            if blacklist:
+                whitelist = {col.name for col in self.table.columns} if whitelist is None else set(whitelist)
+                return frozenset(whitelist.difference(set(blacklist)))
+            elif whitelist:
+                return frozenset(whitelist)
+
+        Service.__init__(self, app=app, logger=logger)
+        self._db = self.discover_service(database_service, cls=DatabaseService)
+        self.table = self._db.add_table(self.table)  # registers table in the db service meta
+        self._primary_keys = frozenset(col.name for col in self.table.primary_key)
+        self._composite_primary_key = len(self._primary_keys) > 1
+        if self._composite_primary_key:
+            self._primary_key_condition = self._create_primary_key_condition_for_composite_key
+            self._list_primary_key_condition = self._create_list_primary_key_condition_for_composite_key
+            self._primary_key = self._primary_key_list = list(self.table.primary_key)
+        elif len(self._primary_keys) == 1:
+            self._primary_key_condition = self._create_primary_key_condition_for_single_key
+            self._list_primary_key_condition = self._create_list_primary_key_condition_for_single_key
+            self._primary_key = next(iter(self.table.primary_key))
+            self._primary_key_list = [self._primary_key]
+        else:
+            self._primary_key_condition = self._raise_primary_key_condition_for_no_keys
+            self._list_primary_key_condition = self._raise_primary_key_condition_for_no_keys
+            self._primary_key = None
+        self.select_columns = _prepare_whitelist(self.select_columns, self.select_columns_blacklist)
+        self.insert_columns = _prepare_whitelist(self.insert_columns, self.insert_columns_blacklist)
+        self.update_columns = _prepare_whitelist(self.update_columns, self.update_columns_blacklist)
+
+    @property
+    def routes(self) -> dict:
+        """Get RPC routes."""
+        return {
+            'exists': self.exists,
+            'get': self.get,
+            'create': self.create,
+            'update': self.update,
+            'delete': self.delete,
+            'm_exists': self.m_exists,
+            'm_get': self.m_get,
+            'm_create': self.m_create,
+            'm_update': self.m_update,
+            'm_delete': self.m_delete,
+            'list': self.list,
+        }
+
+    @staticmethod
+    def get_condition_hook(sql):
+        """Set up specific get conditions."""
+        return sql
+
+    @staticmethod
+    def insert_condition_hook(sql):
+        """Set up specific insert conditions."""
+        return sql
+
+    @staticmethod
+    def update_condition_hook(sql):
+        """Set up specific update conditions."""
+        return sql
+
+    @staticmethod
+    def delete_condition_hook(sql):
+        """Set up specific delete conditions."""
+        return sql
+
+    def _create_primary_key_condition_for_single_key(self, sql, _id):
+        return sql.where(self._primary_key == _id)
+
+    def _create_list_primary_key_condition_for_single_key(self, sql, _id):
+        if not isinstance(_id, (list, tuple, set)):
+            _id = [_id]
+        return sql.where(self._primary_key.in_(_id))
+
+    def _parse_composite_id(self, _id):
+        conditions = []
+        try:
+            if isinstance(_id, dict):
+                for col in self._primary_key:
+                    conditions.append(col == _id[col.name])
+            else:
+                for value, col in zip(_id, self._primary_key):
+                    conditions.append(col == value)
+        except KeyError:
+            raise ValidationError('Primary key field is not present.')
+        else:
+            return sa.and_(*conditions)
+
+    def _create_list_primary_key_condition_for_composite_key(self, sql, _id):
+        if not isinstance(_id, (list, tuple, set)):
+            _id = [_id]
+        condition = sa.or_(*(self._parse_composite_id(n) for n in _id))
+        return sql.where(condition)
+
+    def _create_primary_key_condition_for_composite_key(self, sql, _id: dict):
+        condition = self._parse_composite_id(_id)
+        return sql.where(condition)
+
+    def _raise_primary_key_condition_for_no_keys(self, *_, **__):
+        raise MethodNotAllowed(
+            message='Direct referencing objects in the table is forbidden'
+            ' because there are no primary keys in this table.'
+        )
+
+    async def _wrap_get(self, connection, sql):
+        """Wrap a GET query to reraise SQL errors in a different format."""
+        try:
+            if connection:
+                return await connection.execute(sql)
+            else:
+                async with self._db.connect() as connection:
+                    return await connection.execute(sql)
+        except Exception as exc:
+            self.logger.debug('Internal error.', exc_info=exc)
+            raise InternalError('Error processing query.', base_exc=exc, service=self.service_name)
+
+    async def _wrap_insert(self, connection, sql):
+        """Wrap an INSERT query to reraise SQL errors in a different format."""
+        try:
+            if connection:
+                return await connection.execute(sql)
+            else:
+                async with self._db.begin() as connection:
+                    return await connection.execute(sql)
+        except IntegrityError as exc:
+            raise Conflict(
+                'Name conflict. Object already exists.',
+                code=SQLService.ErrorCode.EXISTS,
+                base_exc=exc,
+                service=self.service_name,
+            )
+        except Exception as exc:
+            self.logger.debug('Internal error.', exc_info=exc)
+            raise InternalError(
+                'Error processing query.',
+                code=SQLService.ErrorCode.INTERNAL_ERROR,
+                base_exc=exc,
+                service=self.service_name,
+            )
+
+    def _wrap_update(self, connection, sql):
+        """Wrap an UPDATE query to reraise SQL errors in a different format."""
+        return self._wrap_insert(connection, sql)
+
+    def _wrap_delete(self, connection, sql):
+        """Wrap a DELETE query to reraise SQL errors in a different format."""
+        return self._wrap_insert(connection, sql)
+
+    def _create_exists_query(self, _id, table=None):
+        if table is None:
+            table = self.table
+        sql = table.select().with_only_columns(sa.text('1'))
+        sql = self._primary_key_condition(sql, _id)
+        sql = self.get_condition_hook(sql)
+        sql = sql.limit(1)
+        return sql
+
+    async def exists(self, id, _connection=None) -> bool:
+        """Return True if object exists. False otherwise.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.exists({'id': 1, 'key': 'abc'})
+
+        """
+        sql = self._create_exists_query(id)
+        result = await self._wrap_get(_connection, sql)
+        return bool(result.first())
+
+    def _create_m_exists_query(self, _id: list, table=None):
+        if table is None:
+            table = self.table
+        sql = table.select().with_only_columns(*self._primary_key_list)
+        sql = self._list_primary_key_condition(sql, _id)
+        sql = self.get_condition_hook(sql)
+        return sql
+
+    async def m_exists(self, id: list, _connection=None):
+        """Return a set of existing IDs for a list of IDs.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.m_exists([{'id': 1, 'key': 'abc'}, ...])
+
+        """
+        sql = self._create_m_exists_query(id)
+        result = await self._wrap_get(_connection, sql)
+        rows = result.all()
+        if rows:
+            if self._composite_primary_key:
+                result = frozenset(
+                    tuple(row[key.name] for key in self._primary_key) for row in (row._asdict() for row in rows)
+                )
+                return result
+            else:
+                result = frozenset(next(iter(row._asdict().values())) for row in rows)
+                return result
+        else:
+            return frozenset()
+
+    def _sql_get_column(self, table, column: str):
+        """Return an SQLAlchemy column by its name."""
+        try:
+            return self.table.columns[column]
+        except KeyError:
+            raise ValidationError(
+                'Requested field doesn\'t exists',
+                obj=table.name,
+                field=column,
+                service=self.service_name,
+                code=SQLService.ErrorCode.FIELD_DOES_NOT_EXISTS,
+            )
+
+    def _sql_get_columns(self, columns, table=None) -> list:
+        """Construct a list of columns from their names.
+
+        .. code-block:: python
+
+            '*'             # all columns
+            "..."           # single column
+            ["...", "..."]  # multiple columns
+
+        """
+        if table is None:
+            table = self.table
+
+        if not columns:
+            return []
+
+        elif columns == '*':
+            if self.select_columns is None:
+                columns = self.table.columns
+            else:
+                columns = [col for col in self.table.columns if col.name in self.select_columns]
+            if self.virtual_columns:
+                virtual = [sa.text(value + f' AS {name}') for name, value in self.virtual_columns.items()]
+                columns = [*columns, *virtual]
+        else:
+            if isinstance(columns, str):
+                columns = [columns]
+
+            if self.virtual_columns:
+
+                _columns = []
+
+                for column in columns:
+                    if column in self.virtual_columns:
+                        value = self.virtual_columns[column]
+                        _columns.append(sa.text(value + f' AS {column}'))
+                    elif self.select_columns:
+                        if column in self.select_columns:
+                            _columns.append(self._sql_get_column(table, column))
+                    else:
+                        _columns.append(self._sql_get_column(table, column))
+
+                columns = _columns
+
+            else:
+                if self.select_columns:
+                    columns = [self._sql_get_column(table, key) for key in columns if key in self.select_columns]
+                else:
+                    columns = [self._sql_get_column(table, key) for key in columns]
+
+        return columns
+
+    @staticmethod
+    def _filter_columns(columns: List[sa.Column], whitelist: Optional[frozenset]):
+        if whitelist is None:
+            return columns
+        else:
+            return [col for col in columns if col.name in whitelist]
+
+    def _create_get_query(self, _id, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        sql = table.select().with_only_columns(*columns)
+        sql = self._primary_key_condition(sql, _id)
+        sql = self.get_condition_hook(sql)
+        sql = sql.limit(1)
+        return sql
+
+    async def get(self, id, columns='*', _connection=None):
+        """Return information about an object.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.get({'id': 1, 'key': 'abc'}, ...)
+
+        :raises NotFound:
+        """
+        if columns is None:
+            raise ValidationError('Null "columns" param is not allowed in a get query.')
+
+        sql = self._create_get_query(id, columns)
+        result = await self._wrap_get(_connection, sql)
+        result = result.first()
+        if not result:
+            raise NotFound(
+                'Object doesn\'t exist.',
+                service=self.service_name,
+                object_id=str(id),
+                code=SQLService.ErrorCode.NOT_FOUND,
+            )
+        if columns:
+            return result._asdict()
+
+    def _create_m_get_query(self, _id: list, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        sql = table.select().with_only_columns(*columns)
+        sql = self._list_primary_key_condition(sql, _id)
+        sql = self.get_condition_hook(sql)
+        return sql
+
+    async def m_get(self, id: list, columns='*', _connection=None):
+        """Return multiple objects.
+
+        Objects that don't exist will be skipped.
+        Returns all data at once without pagination. Use `SQLService.list` if
+        you want pagination or sorting.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.m_get([{'id': 1, 'key': 'abc'}, ...], ...)
+
+        """
+        sql = self._create_m_get_query(id, columns)
+        result = await self._wrap_get(_connection, sql)
+        return [row._asdict() for row in result.all()]
+
+    def _create_delete_query(self, _id, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        sql = table.delete()
+        sql = self._primary_key_condition(sql, _id)
+        sql = self.delete_condition_hook(sql)
+        if columns:
+            sql = sql.returning(*columns)
+        else:
+            sql = sql.returning(sa.literal_column('1'))
+        return sql
+
+    async def delete(self, id, columns=None, _connection=None):
+        """Remove a single object from a table.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.delete({'id': 1, 'key': 'abc'}, ...)
+
+        :raises NotFound: if object doesn't exist or already was deleted
+        """
+        sql = self._create_delete_query(id, columns)
+        result = await self._wrap_delete(_connection, sql)
+        result = result.first()
+        if result is None:
+            raise NotFound(
+                'Object doesn\'t exist thus it can\'t be removed.',
+                service=self.service_name,
+                object_id=str(id),
+                code=SQLService.ErrorCode.NOT_FOUND,
+            )
+        if columns:
+            return result._asdict()
+
+    def _create_m_delete_query(self, _id, conditions, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        sql = table.delete()
+        if _id:
+            sql = self._list_primary_key_condition(sql, _id)
+        if conditions:
+            sql = self._create_conditions(sql, conditions, table)
+        sql = self.delete_condition_hook(sql)
+        sql = sql.returning(*columns)
+        return sql
+
+    async def m_delete(self, id: list = None, conditions=None, columns=None, _connection=None):
+        """Remove multiple objects from a table. Non-existing objects will be skipped.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.m_delete([{'id': 1, 'key': 'abc'}, ...], ...)
+
+        """
+        sql = self._create_m_delete_query(id, conditions, columns)
+        result = await self._wrap_delete(_connection, sql)
+        if columns:
+            result = result.all()
+            return [row._asdict() for row in result]
+
+    @staticmethod
+    def prepare_insert_data(data: dict):
+        """Define your custom row init logic here."""
+        return data
+
+    def _validate_row(self, data: dict, whitelist: frozenset):
+        """Validate and prepare insert row data."""
+        if not data:
+            raise ValidationError(
+                'There are no columns for insert.',
+                data=data,
+                service=self.service_name,
+                allowed_columns=self.insert_columns,
+                code=SQLService.ErrorCode.INVALID_COLUMN,
+            )
+
+        if whitelist:
+            if not set(data).issubset(whitelist):
+                raise ValidationError(
+                    'There are not consumed columns in the update statement.',
+                    data=data,
+                    service=self.service_name,
+                    allowed_columns=self.insert_columns,
+                    code=SQLService.ErrorCode.INVALID_COLUMN,
+                )
+
+    def _create_insert_query(self, data, columns, table=None, **on_conflict_clause):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        self._validate_row(data, whitelist=self.insert_columns)
+        data = self.prepare_insert_data(data)
+        sql = sa_pg.insert(table).values(data)
+        sql = self._on_conflict_clause(sql, **on_conflict_clause)
+        sql = self.insert_condition_hook(sql)
+        sql = sql.returning(*columns)
+        return sql
+
+    def _on_conflict_clause(self, sql, on_conflict=None, on_conflict_keys=None, on_conflict_values=None):
+        if on_conflict == 'do_nothing':
+            sql = sql.on_conflict_do_nothing(index_elements=on_conflict_keys)
+        elif on_conflict == 'do_update':
+            if on_conflict_values:
+                on_conflict_values = self.prepare_update_data(on_conflict_values)
+            sql = sql.on_conflict_do_update(index_elements=on_conflict_keys, set_=on_conflict_values)
+        return sql
+
+    async def create(
+        self,
+        data: dict,
+        columns='*',
+        _connection=None,
+        on_conflict=None,
+        on_conflict_keys=None,
+        on_conflict_values=None,
+    ):
+        """Create a single object.
+
+        :param data: objects data
+        :param columns: columns to return, None for no return
+        :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
+        :param on_conflict_keys: list of on conflict constraints
+        :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
+        :param _connection: optional connection object (when using inside a transactional block)
+        :returns: inserted object
+        """
+        sql = self._create_insert_query(
+            data,
+            columns,
+            on_conflict=on_conflict,
+            on_conflict_keys=on_conflict_keys,
+            on_conflict_values=on_conflict_values,
+        )
+        result = await self._wrap_insert(_connection, sql)
+        if columns:
+            return result.first()._asdict()
+
+    def _create_m_insert_query(self, data: List[dict], columns, table=None, **on_conflict_clause):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        _data = []
+        for row in data:
+            self._validate_row(row, whitelist=self.insert_columns)
+            _data.append(self.prepare_insert_data(row))
+        sql = sa_pg.insert(table).values(_data)
+        sql = self._on_conflict_clause(sql, **on_conflict_clause)
+        sql = self.insert_condition_hook(sql)
+        sql = sql.returning(*columns)
+        return sql
+
+    async def m_create(
+        self,
+        data: List[dict],
+        columns='*',
+        _connection=None,
+        on_conflict: str = None,
+        on_conflict_keys: list = None,
+        on_conflict_values: dict = None,
+    ):
+        """Create multiple objects.
+
+        :param data: list of objects data
+        :param columns: columns to return, None for no return
+        :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
+        :param on_conflict_keys: list of on conflict constraints
+        :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
+        :param _connection: optional connection object (when using inside a transactional block)
+        :returns: inserted objects
+        """
+        sql = self._create_m_insert_query(
+            data,
+            columns,
+            on_conflict=on_conflict,
+            on_conflict_keys=on_conflict_keys,
+            on_conflict_values=on_conflict_values,
+        )
+        result = await self._wrap_insert(_connection, sql)
+        if columns:
+            return [row._asdict() for row in result.all()]
+
+    @staticmethod
+    def prepare_update_data(data: dict):
+        """You may define your custom row update logic here."""
+        return data
+
+    def _create_update_query(self, _id, data: dict, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        self._validate_row(data, whitelist=self.update_columns)
+        data = self.prepare_update_data(data)
+        sql = table.update().values(data)
+        sql = self._primary_key_condition(sql, _id)
+        sql = self.update_condition_hook(sql)
+        sql = sql.returning(*columns) if columns else sql.returning(sa.literal_column('1'))
+        return sql
+
+    async def update(self, id, data: dict, columns='*', _connection=None) -> dict:
+        """Update a single object. Raises error if object doesn't exist.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.update({'id': 1, 'key': 'abc'}, ...)
+
+        """
+        sql = self._create_update_query(id, data, columns)
+        result = await self._wrap_update(_connection, sql)
+        result = result.first()
+        if not result:
+            raise NotFound(
+                'Object doesn\'t exist thus it can\'t be updated.',
+                service=self.service_name,
+                object_id=str(id),
+                code=SQLService.ErrorCode.NOT_FOUND,
+            )
+        if columns:
+            return result._asdict()
+
+    def _create_m_update_query(self, _id, data: dict, conditions, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        self._validate_row(data, whitelist=self.update_columns)
+        data = self.prepare_update_data(data)
+        sql = table.update().values(data)
+        if _id:
+            sql = self._list_primary_key_condition(sql, _id)
+        if conditions:
+            sql = self._create_conditions(sql, conditions, table)
+        sql = self.update_condition_hook(sql)
+        sql = sql.returning(*columns)
+        return sql
+
+    async def m_update(self, id: list, data: dict, conditions=None, columns='*', _connection=None):
+        """Update multiple objects with the same data. Non-existing objects will be skipped.
+
+        If you have composite primary keys you should pass dictionary objects
+        in id field, like this:
+
+        .. code-block:: python
+
+            await service.m_update([{'id': 1, 'key': 'abc'}, ...], ...)
+
+        """
+        sql = self._create_m_update_query(id, data, conditions, columns)
+        result = await self._wrap_update(_connection, sql)
+        if columns:
+            return [row._asdict() for row in result.all()]
+
+    def _create_conditions(self, sql, conditions, table=None):
+        """Add SQL conditions to an sql query.
+
+        Allows some simple queries to be constructed.
+
+        .. code-block:: python
+
+            [ ... ]  # OR
+            { ... }  # AND
+
+            { "...": "..." }            # ==
+            { "...": ["...", "..."] }   # IN
+
+        """
+        if table is None:
+            table = self.table
+
+        def _get_conditions(condition):
+            if type(condition) is dict:
+                _condition = []
+                for key, value in condition.items():
+                    if self.select_columns and key not in self.select_columns:
+                        raise ValidationError(
+                            'Invalid condition requested. Unknown condition key.',
+                            service=self.service_name,
+                            key=key,
+                            code=SQLService.ErrorCode.INVALID_CONDITION,
+                        )
+
+                    column = self._sql_get_column(table, key)
+                    if type(value) is list:
+                        _c = column.in_(value)
+                    elif type(value) is dict:
+                        _sub_cond = []
+                        for key, _value in value.items():
+                            key = key.lower()
+                            if key == 'gt':
+                                _sub_cond.append(column > _value)
+                            elif key == 'lt':
+                                _sub_cond.append(column < _value)
+                            elif key == 'ge':
+                                _sub_cond.append(column >= _value)
+                            elif key == 'le':
+                                _sub_cond.append(column <= _value)
+                            elif key == 'eq':
+                                _sub_cond.append(column == _value)
+                            elif key == 'like':
+                                _sub_cond.append(column.like(_value))
+                            elif key == '~':
+                                _sub_cond.append(sa.func.lower(column).op('~')(sa.func.lower(_value)))
+                            elif key == 'not':
+                                _sub_cond.append(sa.not_(column == _value))  # noqa
+                            else:
+                                raise ValidationError(
+                                    'Invalid condition requested.',
+                                    service=self.service_name,
+                                    condition_key=key,
+                                    code=SQLService.ErrorCode.INVALID_CONDITION,
+                                )
+                        _c = sa.and_(*_sub_cond)
+                    else:
+                        _c = column == value
+                    _condition.append(_c)
+                return sa.and_(*_condition)
+            elif type(condition) is list:
+                _condition = [_get_conditions(c) for c in condition]
+                return sa.or_(*_condition)
+            else:
+                raise ValidationError(
+                    'Invalid condition requested.' ' Condition must be an object or an array of objects.',
+                    service=self.service_name,
+                    code=SQLService.ErrorCode.INVALID_CONDITION,
+                )
+
+        conditions = _get_conditions(conditions)
+        return sql.where(conditions)
+
+    def _create_sort(self, sql, ordering, table=None):
+        """Add SQL ordering command to a query.
+
+        .. code-block:: python
+
+            "..."            # sort ASC by a key
+            {"desc": "..."}  # sort DESC by a key
+            [ ..., ... ]     # sort by multiple keys in order
+
+        """
+
+        def _get_ordering(o):
+            if isinstance(o, dict):
+                key, name = next(iter(o.items()), None)
+                key = key.lower()
+            else:
+                key = 'asc'
+                name = o
+            if type(name) is str:
+                column = self._sql_get_column(table, name)
+            else:
+                column = name
+            if key == 'desc':
+                column = sa.desc(column)
+            elif key == 'asc':
+                pass
+            else:
+                raise ValidationError(
+                    'Invalid ordering requested.',
+                    service=self.service_name,
+                    ordering_key=key,
+                    code=SQLService.ErrorCode.INVALID_ORDERING,
+                )
+            return nullslast(column)
+
+        if table is None:
+            table = self.table
+        if type(ordering) is list:
+            sql = sql.order_by(*(_get_ordering(o) for o in ordering))
+        else:
+            sql = sql.order_by(_get_ordering(ordering))
+        return sql
+
+    def _create_pagination(self, sql, offset, limit):
+        """Add pagination directives to an SQL query.
+
+        Limit < 1 transforms to 1 and offset < 0 transforms to 0 by default.
+        """
+        if offset:
+            try:
+                offset = max(0, int(offset))
+            except ValueError:
+                raise ValidationError(
+                    'Invalid offset.',
+                    service=self.service_name,
+                    pagination_key='offset',
+                    value=offset,
+                    code=SQLService.ErrorCode.INVALID_PAGINATION_OFFSET,
+                )
+            sql = sql.offset(offset)
+
+        if limit is None:
+            limit = self.DEFAULT_ROW_LIMIT
+
+        try:
+            limit = min(max(1, int(limit)), self.MAX_ROW_LIMIT)
+        except ValueError:
+            raise ValidationError(
+                'Invalid limit.',
+                service=self.service_name,
+                pagination_key='limit',
+                value=limit,
+                code=SQLService.ErrorCode.INVALID_PAGINATION_LIMIT,
+            )
+
+        sql = sql.limit(limit)
+        return sql
+
+    def _create_count_query(self, conditions, precision=None, table=None):
+        """Use COUNT(id) for slow precise count or TABLESAMPLE for estimate."""
+        if table is None:
+            table = self.table
+        key = next(iter(self._primary_key_list))
+        sql = table.select().with_only_columns(sa.func.count(key))
+        if conditions:
+            sql = self._create_conditions(sql, conditions, table=table)
+        sql = self.get_condition_hook(sql)
+        if precision:
+            precision = min(max(1, precision), 100)
+            sql = f'SELECT count({key.name})' f' FROM {table.name} TABLESAMPLE system({precision});'
+        return sql
+
+    def _create_list_query(self, conditions, sort, offset, limit, columns, table=None):
+        if table is None:
+            table = self.table
+        columns = self._sql_get_columns(columns, table=table)
+        sql = table.select().with_only_columns(*columns)
+        if conditions:
+            sql = self._create_conditions(sql, conditions, table=table)
+        sql = self.get_condition_hook(sql)
+        if sort:
+            sql = self._create_sort(sql, sort, table=table)
+        if offset or limit:
+            sql = self._create_pagination(sql, offset, limit)
+        return sql
+
+    @staticmethod
+    def _get_page_count(count: int, offset: int, page_size: int) -> (int, int):
+        """Return current page number and number of pages."""
+        if page_size:
+            n = count - offset
+            pages = max(1, count // page_size + bool(n % page_size))
+            page = max(1, offset // page_size + bool(n % page_size))
+            return page, pages
+        else:
+            return None, None
+
+    async def list(
+        self,
+        conditions=None,
+        sort=None,
+        offset=0,
+        limit=DEFAULT_ROW_LIMIT,
+        count=True,
+        precision=None,
+        columns='*',
+        _connection=None,
+    ) -> _List:
+        """List rows with pagination and conditions.
+
+        :param conditions: optional query conditions
+        :param sort: optional row ordering
+        :param offset: optional row offset
+        :param limit: optional row limit
+        :param count: calculate page count
+        :param precision: count precision, if None then table sampling won't be used
+            must be from 0 to 100
+        :param columns: columns to return
+        :param _connection: optional connection object (when using inside a transactional block)
+        :returns: This method may return different data depending on the provided params
+
+        Condition example:
+
+        .. code-block:: python
+
+            service.list(
+                conditions={
+                    'tag': ['tag_1', 'tag_2', 'tag_3'],  # IN condition
+                    'active': True,                      # EQ condition
+                    'value': {'gt': 41, 'le': 42'},      # num conditions,
+                    'text': {'like': 'sht'},             # text field "likeness"
+                }
+            )
+
+        Available numeric conditions: gt, lt, ge, le, eq
+        Available other conditions: like
+
+        Sort example:
+
+        .. code-block:: python
+
+            service.list(
+                sort=['tag', {'desc': 'timestamp'}]     # order matters
+            )
+
+        Available sorting conditions: desc, asc (default)
+
+        You can use this method for counting without returning any results.
+        Just set the limit to zero. Optionally, you can also set the counting
+        precision.
+
+        .. code-block::
+
+            service.list(
+                conditions={ ... },
+                precision=50
+                limit=0
+            )
+
+        Contrary, if you don't need counting, you can disable it. No count / page
+        data will be available then.
+
+        .. code-block::
+
+            service.list(
+                conditions={ ... },
+                count=False
+            )
+
+        Precision uses a number of table samples to estimate the count. If
+        the precision is set to 0 or None, then the exact count will be performed.
+
+        .. attention::
+
+            Precision is not working at the moment (don't know why).
+
+        If count argument is False, then count, page and pages result values
+        will be None.
+
+        If columns is None, then data will be None and on_page will be zero.
+
+        .. code-block:: python
+
+            {
+                count: Optional[int]          #: total rows matching the query, None if count hasn't been requested
+                offset: int                   #: row offset for this selection
+                page: Optional[int]           #: current page number, None if count hasn't been requested
+                pages: Optional[int]          #: total pages, None if count hasn't been requested
+                on_page: int                  #: number of rows on this page
+                data: Optional[List[dict]]    #: returned rows, None if limit was set to 0
+            }
+
+        """
+        if columns and limit:
+            sql = self._create_list_query(conditions, sort, offset, limit, columns)
+            result = await self._wrap_get(_connection, sql)
+            result = result.all()
+            result = [row._asdict() for row in result]
+            if count:
+                sql_count = self._create_count_query(conditions, precision)
+                count = await self._wrap_get(_connection, sql_count)
+                count = count.scalar()
+                page, pages = self._get_page_count(count, offset, limit)
+            else:
+                count, page, pages = None, None, None
+            on_page = len(result)
+        else:
+            on_page, result = 0, None
+            if count:
+                sql_count = self._create_count_query(conditions, precision)
+                count = await self._wrap_get(_connection, sql_count)
+                count = count.scalar()
+                page, pages = self._get_page_count(count, offset, limit)
+            else:
+                count, page, pages, on_page = None, None, None, 0
+
+        return {'count': count, 'offset': offset, 'page': page, 'pages': pages, 'on_page': on_page, 'data': result}
+
+    async def iter(
+        self, conditions=None, sort=None, offset=0, limit=DEFAULT_ROW_LIMIT, columns='*'
+    ) -> AsyncGenerator[List[dict], None]:
+        """Iterate over listed data.
+
+        Almost the same as `SQLService.list` but returns a generator which iterates
+        over the query content. It's not intended to be used by a client
+        but inside the app or the service itself.
+
+        See `SQLService.list` for info about params.
+        """
+        if not sort:
+            sort = self._primary_key_list
+
+        result = await self.list(
+            conditions=conditions, sort=sort, offset=offset, limit=limit, columns=columns, count=True
+        )
+
+        page, pages = result['page'], result['pages']
+        yield result['data']
+
+        page += 1
+
+        while page <= pages:
+            offset = (page - 1) * limit
+            result = await self.list(
+                conditions=conditions, sort=sort, offset=offset, limit=limit, columns=columns, count=False
+            )
+            yield result['data']
+            page += 1
+
+
+class FixtureService(ContextableService):
+    """Fixture service.
+
+    It can load data from json files using SQLService interface.
+    """
+
+    def __init__(
+        self,
+        app,
+        root_dir: str = './fixtures',
+        fixtures: Collection[str] = None,
+        empty_tables_only: bool = True,
+        load_on_init: bool = True,
+        logger=None,
+    ):
+        """Initialize.
+
+        :param app: web app
+        :param root_dir: fixtures base dir
+        :param fixtures: list of fixtures (service names) to load, None - load all
+        :param empty_tables_only: load only when the service table is empty
+        :param load_on_init: load all fixtures on service init (when starting the app)
+        :param logger: parent logger instance
+        """
+        super().__init__(app=app, logger=logger)
+        self.root_dir = Path(root_dir).resolve()
+        self.fixtures = fixtures
+        self.empty_tables_only = empty_tables_only
+        self.load_on_init = load_on_init
+
+    async def init(self):
+        if not self.root_dir.exists():
+            self.logger.warn('Fixture path does not exist', root_dir=str(self.root_dir))
+        if self.load_on_init:
+            await self.load_all()
+
+    async def load_all(self) -> None:
+        """Load all fixtures in the root dir."""
+        for path in self.root_dir.rglob('*.json'):
+            if self.fixtures and path.stem not in self.fixtures:
+                continue
+            await self.load_fixture(path)
+
+    async def load_fixture(self, path: Path) -> None:
+        """Load a single service fixture.
+
+        A file must be a JSON list with rows of data.
+        """
+        service_name = path.stem
+
+        if service_name not in self.app.services:
+            self.logger.debug('Cannot load fixture: no such service', fixture=service_name)
+            return
+
+        service = cast(SQLService, self.app.services[service_name])
+        if not isinstance(service, SQLService):
+            self.logger.debug('Cannot load fixture: not an SQLService interface', fixture=service_name)
+            return
+
+        if not path.exists() or not path.is_file():
+            self.logger.debug('Cannot load fixture: file does not exist', fixture=service_name, filename=str(path))
+            return
+
+        if self.empty_tables_only:
+            if await self._table_not_empty(service_name):
+                self.logger.debug('Cannot load fixture: table is not empty', fixture=service_name)
+                return
+
+        data = load(path)
+        if data:
+            self.logger.info('Loading fixture', fixture=service_name, filename=str(path))
+            await service.m_create(data=data, columns=[], on_conflict='do_nothing')
+
+    async def _table_not_empty(self, service_name: str) -> bool:
+        service = cast(SQLService, self.app.services[service_name])
+        data = await service.list(limit=1, count=False)
+        return bool(data['data'])
+
+
+class DatabaseMigrationService(ContextableService):
+    """Simple migration tool."""
+
+    class State(TypedDict, total=False):
+        """Migration state as in the migrations json file."""
+
+        id: int  #: identifier
+        comments: str  #: commit SHA
+        commands: List[str]  #: command or a set of commands to perform
+
+    _state_table = sa.Table('db_info', sa.MetaData(), sa.Column('key', sa.TEXT), sa.Column('value', sa_pg.JSONB))
+    _state_key = 'state'
+    _null_state = -1
+
+    def __init__(
+        self,
+        app,
+        *,
+        database_service: DatabaseService = None,
+        migrations_file='./etc/migrations.json',
+        migrate_on_start: bool = False,
+        logger=None,
+    ):
+        """Initialize.
+
+        :param app:
+        :param database_service:
+        :param migrations_file: default migrations file
+        :param migrate_on_start: perform an automatic migration from the current state at async init
+        :param logger:
+        """
+        super().__init__(app, logger=logger)
+        self._migrations_file = migrations_file
+        self._db = self.discover_service(database_service, cls=DatabaseMigrationService)
+        self._db.add_table(self._state_table)
+        self._migrate_on_start = migrate_on_start
+
+    async def init(self):
+        if self._migrate_on_start:
+            await self.migrate()
+
+    async def migrate(self, from_: int = None, to_: int = None, migrations_file: str = None) -> int:
+        """Migrate DB from one state to another.
+
+        Migration file is expected to be a json file with a number of sorted states containing state id and a list of
+        sequential SQL commands. State ids must start from 0.
+
+        .. code-block:: json
+
+            [
+                {
+                    "id": 0,
+                    "comments": "dev comments",
+                    "commands": [
+                        "ALTER TABLE my_table ADD COLUMN new_col DEFAULT NULL;",
+                        "ALTER TABLE my_table DROP COLUMN old_col;",
+                    ]
+                }
+            ]
+
+        :param from_: state to migrate from (by default the current state is used)
+        :param to_: state to migrate to (by default the last state is used)
+        :param migrations_file: optional migrations file path
+        :return: current state id
+        """
+        if migrations_file is None:
+            migrations_file = self._migrations_file
+        with open(migrations_file) as f:
+            migrations: List[DatabaseMigrationService.State] = load(f)
+        state_id = await self.get_state()
+        self.logger.info('Start state: #%d.', state_id)
+        if from_ is None:
+            from_ = state_id
+        if to_ is None:
+            to_ = migrations[-1]['id']
+        self.logger.info('Performing migration: #%d -> #%d', from_, to_)
+        for state in migrations:
+            state_id = state['id']
+            if state_id <= from_:
+                continue
+            elif state_id > to_:
+                break
+            self.logger.info('Migrating state: #%d', state['id'])
+            async with self._db.begin() as conn:
+                for n, cmd in enumerate(state['commands']):
+                    self.logger.info('Migrating state: #%d/%d.', state['id'], n)
+                    await conn.execute(sa.text(cmd))
+                sql = (
+                    self._state_table.update()
+                    .where(self._state_table.c.key == self._state_key)
+                    .values({'value': state['id']})
+                )
+                await conn.execute(sql)
+                await conn.commit()
+
+        state_id = await self.get_state()
+        self.logger.info('End state: #%d', state_id)
+        return state_id
+
+    async def get_state(self) -> int:
+        """Get current (supposed) database state."""
+        sql = self._state_table.select().where(self._state_table.c.key == self._state_key)
+        state = await self._db.fetchrow(sql)
+        if state is None:
+            sql = self._state_table.insert().values({'key': self._state_key, 'value': self._null_state})
+            await self._db.execute(sql)
+            state_id = self._null_state
+        else:
+            state_id = state['value']
+        return state_id
+
 
 service_class_registry.register_class(DatabaseService)
 service_class_registry.register_class(DatabaseMigrationService)
 service_class_registry.register_class(FixtureService)
```

## kaiju_db/types.py

```diff
@@ -1,10 +1,20 @@
 import sqlalchemy.types as types
 import sqlalchemy.dialects.postgresql as sa_pg
+from sqlalchemy_utils import Ltree as PGLtree
 
-__all__ = ['CITEXT']
+__all__ = ['CITEXT', 'Ltree']
 
 
 class CITEXT(types.UserDefinedType, sa_pg.TEXT):
+    """Postgres case-insensitive text data type."""
 
-    def get_col_spec(self):
+    def get_col_spec(self):  # noqa: required
         return 'CITEXT'
+
+
+class Ltree(PGLtree):
+    """Postgresql Ltree data type."""
+
+    @classmethod
+    def validate(cls, path):
+        pass
```

## kaiju_db/tests/fixtures.py

```diff
@@ -1,127 +1,114 @@
-import pytest
+import pytest  # noqa: pycharm
 import sqlalchemy as sa
+import sqlalchemy.dialects.postgresql as sa_pg
 
-from kaiju_tools.tests.fixtures import *
-from kaiju_tools.docker import DockerContainer
+from kaiju_tools.docker import DockerContainer, DockerImage
+from kaiju_tools.tests.fixtures import get_app
 
-from ..functions import UserFunction
-from ..services import DatabaseService
+from kaiju_db.services import *
 
+__all__ = [
+    'postgres',
+    'postgres_glob',
+    'database_service',
+    'test_table',
+    'database_settings',
+    'migrations_file',
+    'migrations_service',
+]
 
-DB_NAME = 'test_db'
+DB_NAME = 'pytest'
 DB_PORT = 5444
-
 ROOT_CREDENTIALS = {'user': 'postgres', 'password': 'postgres'}
-
 DEFAULT_CREDENTIALS = {'user': 'test', 'password': 'test'}
 
 
 @pytest.fixture
 def database_settings():
     """Get default test database settings."""
     return {
         'host': 'localhost',
         'port': DB_PORT,
-        'database': DB_NAME,
-        'user': DEFAULT_CREDENTIALS['user'],
-        'password': DEFAULT_CREDENTIALS['password'],
-        'root_user': ROOT_CREDENTIALS['user'],
-        'root_password': ROOT_CREDENTIALS['password'],
+        'database': 'pytest',
+        'user': 'test',
+        'password': 'test',
+        'root_user': 'postgres',
+        'root_password': 'postgres',
         'root_database': 'postgres',
         'init_db': True,
         'init_tables': True,
         'pool_size': 10,
         'idle_connection_lifetime': 3600,
         'extensions': ['uuid-ossp', 'ltree'],
     }
 
 
-@pytest.fixture
-def database_service(logger, database_settings):
-    """Return a new instance of database service."""
-    service = DatabaseService(app=None, metadata=None, logger=logger, **database_settings)
-    return service
-
-
-def _database_container(logger):
+def _pg_container(app):
     return DockerContainer(
-        image={'tag': 'postgres', 'version': '14'},
+        image=DockerImage(app=app, tag='postgres', version='14'),
         name='pytest-postgres',
         ports={'5432': str(DB_PORT)},
         env={'POSTGRES_USER': 'postgres', 'POSTGRES_PASSWORD': 'postgres'},
         healthcheck={
             'test': 'pg_isready',
             'interval': 100000000,
             'timeout': 3000000000,
             'start_period': 1000000000,
             'retries': 3,
         },
-        sleep_interval=0.5,
+        sleep_interval=1,
         remove_on_exit=True,
-        logger=logger,
+        app=app,
     )
 
 
 @pytest.fixture
-def database(logger):
+def postgres(app):
     """Return a new database container. See `kaiju_tools.tests.fixtures.container` for more info."""
-    with _database_container(logger) as c:
+    with _pg_container(app) as c:
         yield c
 
 
 @pytest.fixture(scope='session')
-def per_session_database(logger):
+def postgres_glob(logger):
     """Return a new database container. See `kaiju_tools.tests.fixtures.per_session_container` for more info."""
-    with _database_container(logger) as c:
+    app = get_app(logger)
+    with _pg_container(app) as c:
         yield c
 
 
 @pytest.fixture
-def test_table():
-    t = sa.Table(
-        'test_table',
-        sa.MetaData(),
-        sa.Column('id', sa.Integer, primary_key=True),
-        sa.Column('value', sa.Boolean, default=False),
-        sa.Column('other_value', sa.Boolean, default=False),
-        sa.Column('secret_value', sa.TEXT, default=''),
-        sa.Column('null_value', sa.TEXT, default=None),
-        sa.Column('t', sa.TIMESTAMP),
-    )
-    return t
+def database_service(postgres_glob, app, database_settings) -> DatabaseService:
+    """Return a new instance of database service."""
+    service = DatabaseService(app, metadata=sa.MetaData(), **database_settings)
+    app.services.add_service(service)
+    return service
 
 
 @pytest.fixture
-def test_composite_table():
-    t = sa.Table(
-        'test_composite_table',
-        sa.MetaData(),
-        sa.Column('id', sa.Integer, primary_key=True),
-        sa.Column('key', sa.Integer, primary_key=True),
-        sa.Column('value', sa.Boolean, default=False),
-        sa.Column('other_value', sa.Boolean, default=False),
-        sa.Column('secret_value', sa.TEXT, default=''),
-        sa.Column('null_value', sa.TEXT, default=None),
-        sa.Column('t', sa.TIMESTAMP),
-    )
-    return t
+def migrations_file(tmp_path):
+    path = tmp_path / 'migrations.json'
+    return path
 
 
 @pytest.fixture
-def test_function():
-    class MyFunction(UserFunction):
-        package = 'utils'
-        name = 'my_func'
-        type = sa.types.Integer
-        body = """
-        FUNCTION my_func(v integer) RETURNS integer AS $$
-        BEGIN
-        RETURN v * v;
-        END; $$
-        LANGUAGE PLPGSQL
-        """
+def migrations_service(postgres_glob, app, database_service, migrations_file) -> DatabaseMigrationService:
+    """Return a new instance of database service."""
+    service = DatabaseMigrationService(app, database_service=database_service, migrations_file=str(migrations_file))
+    app.services.add_service(service)
+    return service
 
-        def __init__(self, v: int):
-            super(MyFunction, self).__init__(v)
 
-    return MyFunction
+@pytest.fixture
+def test_table(database_service):
+    t = sa.Table(
+        'test_table',
+        database_service.metadata,
+        sa.Column('id', sa_pg.TEXT, primary_key=True),
+        sa.Column('name', sa_pg.TEXT),
+        sa.Column('value', sa_pg.INTEGER),
+        sa.Column('enabled', sa_pg.BOOLEAN),
+        sa.Column('timestamp', sa_pg.INTEGER),
+        sa.Column('created', sa_pg.TIMESTAMP),
+    )
+    return t
```

## Comparing `kaiju_db-2.1.1.dist-info/LICENSE` & `kaiju_db-2.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.1.dist-info/METADATA` & `kaiju_db-2.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.1
+Version: 2.1.2
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

## Comparing `kaiju_db-2.1.1.dist-info/RECORD` & `kaiju_db-2.1.2.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-kaiju_db/__init__.py,sha256=UaoyWUgwUSEytOKYYYlZqYXHnZZFpukfR_CcGJOJgSk,282
-kaiju_db/fixtures.py,sha256=AuzsoL8HAWMCPITs9TvqZVv6iQaJ9no5Z4bp_iuQcwo,3127
+kaiju_db/__init__.py,sha256=sNhwNLlRyT73ileUc9FTyOCFRUBZfCjXQ4vEV51Cv0Q,183
 kaiju_db/functions.py,sha256=0E7H85QZkRvPBMa6H5n9eC5tJlCvKXPvKT6e5O-nuGQ,3665
-kaiju_db/ltree.py,sha256=Y2g_GZ9T7dQRYknAkuUmDjHTrrdyPEu1d9QQDJ-Gsus,204
-kaiju_db/migrations.py,sha256=mv4ytDcoUasB1-DlcrxBBkF1UJ3PKuoEN7l921EyYLc,4522
-kaiju_db/services.py,sha256=VczBFT8V9q-N7EleZ2DvgY_SMOHaTL_NRiJ7C2f_9M8,386
-kaiju_db/sql_service.py,sha256=I1fx1PDB5OHBjmsdCalIys22ERIIUh2_vnFRWKF9dvs,39661
-kaiju_db/transport.py,sha256=fP1qLLz6wywhsA6FHsjen-vh-LW3_X81TkZJn2paZgI,9761
-kaiju_db/types.py,sha256=Au_j6lWIRLDrHdmbRiHDquxEnjOOU1bCDmJftkHxJmY,206
+kaiju_db/services.py,sha256=C8f_KK_q14xbtgjn-CsBkSRd226ONiZf6oHQKEK7OTA,57079
+kaiju_db/types.py,sha256=0ORvc2CaCcKUNibTR5o9EI5DOFQjM_uDg5S58aF8MyU,453
 kaiju_db/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kaiju_db/tests/fixtures.py,sha256=a4hayXLJyEJOjxQgzHpaqUusp5urpR-I6x_x1SaANcA,3568
-kaiju_db/tests/test_services.py,sha256=sEzOtI4e3I6sakqBCzq1fMNZR5q-D0G7rQ66tpyiRGo,13635
-kaiju_db-2.1.1.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_db-2.1.1.dist-info/METADATA,sha256=TodZOu9MNc2eBXy-ZsOmCH3jmMkjbgTRwZeea6Uzuys,3090
-kaiju_db-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_db-2.1.1.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
-kaiju_db-2.1.1.dist-info/RECORD,,
+kaiju_db/tests/fixtures.py,sha256=vkf27hrIx4meIa-A3uKbmXSmjkeih6QMUBpxQ-xwljI,3240
+kaiju_db/tests/test_db.py,sha256=V7rmNkGeDIOr_Wf_e6IaSqEkfK_wRDJ2nsJdcnDUU-8,4125
+kaiju_db-2.1.2.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_db-2.1.2.dist-info/METADATA,sha256=lrlsmg6ToSDBJ9P8cID-KEP4sWpgJogmV8JPygRQkcY,3090
+kaiju_db-2.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_db-2.1.2.dist-info/top_level.txt,sha256=-jcfPgSkIz8rxFCPp_XIg5g9tVsDmBd1wdxayb_mkNU,9
+kaiju_db-2.1.2.dist-info/RECORD,,
```

