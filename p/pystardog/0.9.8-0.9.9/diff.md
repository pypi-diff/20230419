# Comparing `tmp/pystardog-0.9.8-py3-none-any.whl.zip` & `tmp/pystardog-0.9.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,20 @@
-Zip file size: 21395 bytes, number of entries: 17
+Zip file size: 23988 bytes, number of entries: 18
 -rw-r--r--  2.0 unx      261 b- defN 21-Feb-15 06:18 stardog/__init__.py
--rw-r--r--  2.0 unx    26876 b- defN 21-Apr-28 16:35 stardog/admin.py
--rw-r--r--  2.0 unx    25253 b- defN 21-Apr-28 16:35 stardog/connection.py
--rw-r--r--  2.0 unx     3514 b- defN 21-Feb-15 06:18 stardog/content.py
+-rw-r--r--  2.0 unx    33580 b- defN 21-May-14 18:44 stardog/admin.py
+-rw-r--r--  2.0 unx    25405 b- defN 21-May-06 22:53 stardog/connection.py
+-rw-r--r--  2.0 unx     3514 b- defN 21-May-11 07:43 stardog/content.py
 -rw-r--r--  2.0 unx     1660 b- defN 21-Feb-15 06:18 stardog/content_types.py
 -rw-r--r--  2.0 unx      181 b- defN 21-Feb-15 06:18 stardog/exceptions.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Feb-15 06:18 stardog/http/__init__.py
--rw-r--r--  2.0 unx     2179 b- defN 21-Apr-22 01:29 stardog/http/client.py
+-rw-r--r--  2.0 unx     2179 b- defN 21-Apr-28 18:53 stardog/http/client.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Feb-15 06:18 test/__init__.py
--rw-r--r--  2.0 unx     9076 b- defN 21-Apr-28 16:35 test/test_admin.py
--rw-r--r--  2.0 unx     9944 b- defN 21-Apr-28 16:35 test/test_connection.py
+-rw-r--r--  2.0 unx     1373 b- defN 21-May-14 18:44 test/conftest.py
+-rw-r--r--  2.0 unx    12202 b- defN 21-May-14 18:44 test/test_admin.py
+-rw-r--r--  2.0 unx     9966 b- defN 21-May-06 22:53 test/test_connection.py
 -rw-r--r--  2.0 unx     1118 b- defN 21-Feb-15 06:18 test/test_utils.py
--rw-r--r--  2.0 unx      554 b- defN 21-Apr-28 16:50 pystardog-0.9.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2257 b- defN 21-Apr-28 16:50 pystardog-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Apr-28 16:50 pystardog-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 21-Apr-28 16:50 pystardog-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1313 b- defN 21-Apr-28 16:50 pystardog-0.9.8.dist-info/RECORD
-17 files, 84291 bytes uncompressed, 19263 bytes compressed:  77.1%
+-rw-r--r--  2.0 unx      554 b- defN 21-May-14 18:48 pystardog-0.9.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2198 b- defN 21-May-14 18:48 pystardog-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-May-14 18:48 pystardog-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 21-May-14 18:48 pystardog-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1387 b- defN 21-May-14 18:48 pystardog-0.9.9.dist-info/RECORD
+18 files, 95683 bytes uncompressed, 21748 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -21,32 +21,35 @@
 
 Filename: stardog/http/client.py
 Comment: 
 
 Filename: test/__init__.py
 Comment: 
 
+Filename: test/conftest.py
+Comment: 
+
 Filename: test/test_admin.py
 Comment: 
 
 Filename: test/test_connection.py
 Comment: 
 
 Filename: test/test_utils.py
 Comment: 
 
-Filename: pystardog-0.9.8.dist-info/LICENSE
+Filename: pystardog-0.9.9.dist-info/LICENSE
 Comment: 
 
-Filename: pystardog-0.9.8.dist-info/METADATA
+Filename: pystardog-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: pystardog-0.9.8.dist-info/WHEEL
+Filename: pystardog-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: pystardog-0.9.8.dist-info/top_level.txt
+Filename: pystardog-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pystardog-0.9.8.dist-info/RECORD
+Filename: pystardog-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stardog/admin.py

```diff
@@ -275,15 +275,14 @@
             'username': username,
             'password': list(password),
             'superuser': superuser,
         }
 
         self.client.post('/admin/users', json=meta)
         return self.user(username)
-        return User(username, self.client)
 
     def role(self, name):
         """Retrieves an object representing a role.
 
         Args:
           name (str): The name of the Role
 
@@ -331,15 +330,46 @@
         Returns:
           list[VirtualGraph]: A list of VirtualGraph objects
         """
         r = self.client.get('/admin/virtual_graphs')
         virtual_graphs = r.json()['virtual_graphs']
         return list(map(lambda name: VirtualGraph(name, self.client), virtual_graphs))
 
-    def new_virtual_graph(self, name, mappings, options):
+
+    def import_virtual_graph(self, db, mappings, named_graph, remove_all, options):
+        """Import (materialize) a virtual graph directly into the local knowledge graph.
+
+        Args:
+          db (str): The database into which to import the graph
+          mappings (Content): New mapping contents. An empty string can be passed for autogenerated mappings.
+          named_graph (str): Name of the graph into which import the VG.
+          remove_all (bool): Should the target named graph be cleared before importing?
+          options (dict): Options for the new virtual graph, https://docs.stardog.com/virtual-graphs/virtual-graph-configuration#virtual-graph-properties
+
+        Examples:
+            >>> admin.import_virtual_graph(
+                  'db-name', mappings=File('mappings.ttl'),
+                  named_graph='my-graph', remove_all=True, options={'jdbc.driver': 'com.mysql.jdbc.Driver'}
+                )
+        """
+
+        if mappings:
+            with mappings.data() as data:
+                mappings = data.read().decode() if hasattr(data, 'read') else data
+        meta = {
+            'db': db,
+            'mappings': mappings,
+            'named_graph': named_graph,
+            'remove_all': remove_all,
+            'options': options
+        }
+        r = self.client.post('/admin/virtual_graphs/import_db', json=meta)
+
+
+    def new_virtual_graph(self, name, mappings, options={}, datasource=None, db=None):
         """Creates a new Virtual Graph.
 
         Args:
           name (str): The name of the virtual graph
           mappings (Content): New mapping contents
           options (dict): Options for the new virtual graph
 
@@ -348,32 +378,128 @@
 
         Examples:
             >>> admin.new_virtual_graph(
                   'users', File('mappings.ttl'),
                   {'jdbc.driver': 'com.mysql.jdbc.Driver'}
                 )
         """
-        with mappings.data() as data:
+
+        if mappings:
+            with mappings.data() as data:
+                mappings = data.read().decode() if hasattr(data, 'read') else data
+
+        if options:
             meta = {
                 'name': name,
-                'mappings': data.read().decode() if hasattr(data, 'read') else data,
+                'mappings': mappings,
                 'options': options,
             }
+        else:
+            meta = {
+                'name': name,
+                'mappings': mappings,
+                'data_source': datasource,
+                'db': db
+            }
+
+
+        self.client.post('/admin/virtual_graphs', json=meta)
+        return VirtualGraph(name, self.client)
+
+    def datasource(self, name):
+        """Retrieves an object representing a DataSource.
+
+        Args:
+          name (str): The name of the data source
+
+        Returns:
+          DataSource: The DataSource object
+        """
+        return DataSource(name, self.client)
+
+    def datasources(self):
+        """Retrieves all data sources.
+
+        Returns:
+          list[DataSources]: A list of DataSources
+        """
+        r = self.client.get('/admin/data_sources')
+        data_sources = r.json()['data_sources']
+        return list(map(lambda name: DataSource(name, self.client), data_sources))
+
+    def datasources_info(self):
+        """List data sources info
+
+        Returns:
+          list: A list of data sources info
+        """
+
+        r = self.client.get('/admin/data_sources/list')
+        return r.json()['data_sources']
 
-            self.client.post('/admin/virtual_graphs', json=meta)
-            return VirtualGraph(name, self.client)
+    def new_datasource(self, name, options):
+        """Creates a new DataSource.
+
+        Args:
+          name (str): The name of the data source
+          options (dict): Data source options
+
+        Returns:
+          User: The new DataSource object
+        """
+
+        if options is None:
+            options = {}
+
+        meta = {
+            "name": name,
+            "options": options
+        }
+
+        self.client.post('/admin/data_sources', json=meta)
+        return self.datasource(name)
+
+    def get_server_properties(self):
+        """Get the value of any set server-level properties
+
+        Returns
+            dict: Server properties
+        """
+
+        r = self.client.get('/admin/properties')
+        return r.json()
 
     def validate(self):
         """Validates an admin connection.
 
         Returns:
           bool: The connection state
         """
         self.client.get('/admin/users/valid')
 
+    def cluster_status(self):
+        """Prints status information for each node
+        in the cluster
+
+        Returns:
+            dict: Nodes of the cluster and extra information
+        """
+        r = self.client.get('/admin/cluster/status')
+        return r.json()
+
+    def cluster_info(self):
+        """Prints info about the nodes in the Stardog
+        Pack cluster.
+
+        Returns:
+            dict: Nodes of the cluster.
+        """
+        r = self.client.get('/admin/cluster')
+        return r.json()
+
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         self.client.close()
 
 
@@ -895,35 +1021,46 @@
 
     @property
     def name(self):
         """The name of the virtual graph.
         """
         return self.graph_name
 
-    def update(self, name, mappings, options):
+    def update(self, name, mappings, options={}, datasource=None, db=None):
         """Updates the Virtual Graph.
 
         Args:
           name (str): The new name
           mappings (Content): New mapping contents
           options (dict): New options
 
         Examples:
             >>> vg.update('users', File('mappings.ttl'),
                          {'jdbc.driver': 'com.mysql.jdbc.Driver'})
         """
-        with mappings.data() as data:
+        if mappings:
+            with mappings.data() as data:
+                mappings = data.read().decode() if hasattr(data, 'read') else data
+
+        if options:
             meta = {
                 'name': name,
-                'mappings': data.read().decode() if hasattr(data, 'read') else data,
+                'mappings': mappings,
                 'options': options,
             }
+        else:
+            meta = {
+                'name': name,
+                'mappings': mappings,
+                'data_source': datasource,
+                'db': db
+            }
 
-            self.client.put(self.path, json=meta)
-            self.graph_name = name
+        self.client.put(self.path, json=meta)
+        self.graph_name = name
 
     def delete(self):
         """Deletes the Virtual Graph.
         """
         self.client.delete(self.path)
 
     def options(self):
@@ -931,14 +1068,34 @@
 
         Returns:
           dict: Options
         """
         r = self.client.get(self.path + '/options')
         return r.json()['options']
 
+    def info(self):
+        """Gets Virtual Graph info.
+
+        Returns:
+          dict: Info
+        """
+
+        r = self.client.get(self.path + '/info')
+        return r.json()['info']
+
+    def get_database(self):
+        """Gets database associated with the VirtualGraph.
+
+        Returns:
+          string: Database name
+        """
+
+        r = self.client.get(self.path + '/database')
+        return r.text
+
     def mappings(self, content_type=content_types.TURTLE):
         """Gets the Virtual Graph mappings.
 
         Args:
           content_type (str): Content type for results.
             Defaults to 'text/turtle'
 
@@ -956,7 +1113,111 @@
           bool: Availability state
         """
         r = self.client.get(self.path + '/available')
         return bool(r.json()['available'])
 
     def __repr__(self):
         return self.name
+
+
+class DataSource(object):
+    """Initializes a DataSource
+
+    See Also:
+        https://docs.stardog.com/virtual-graphs/virtual-sources
+    """
+
+    def __init__(self, name, client):
+        """Initializes a DataSource.
+
+        Use :meth:`stardog.admin.Admin.data_source`,
+        :meth:`stardog.admin.Admin.data_sources`, or
+        :meth:`stardog.admin.Admin.new_data_source` instead of
+        constructing manually.
+        """
+
+        self.data_source_name = name
+        self.path = '/admin/data_sources/{}'.format(name)
+        self.client = client
+
+    @property
+    def name(self):
+        """The name of the data source.
+        """
+        return self.data_source_name
+
+    def available(self):
+        """Checks if the data source is available.
+
+        Returns:
+          bool: Availability state
+        """
+        r = self.client.get(self.path + '/available')
+        return bool(r.json())
+
+    def refresh_count(self, meta=None):
+        """Refresh table row-count estimates
+        """
+
+        if meta is None:
+            meta = {}
+
+        self.client.post(self.path + '/refresh_counts', json=meta)
+
+    def update(self, options=None):
+        """Update data source
+        """
+        if options is None:
+            options = {}
+
+        meta = {
+            "options": options
+        }
+
+        self.client.put(self.path, json=meta)
+
+    def delete(self):
+        """Deletes a data source
+        """
+
+        self.client.delete(self.path)
+
+    def online(self):
+        """Online a data source
+        """
+
+        self.client.post(self.path + '/online')
+
+    def info(self):
+        """Get data source info
+
+        Returns:
+          dict: Info
+        """
+
+        r = self.client.get(self.path + '/info')
+        return r.json()['info']
+
+    def refresh_metadata(self, meta=None):
+        """Refresh metadata
+        """
+
+        if meta is None:
+            meta = {}
+
+        self.client.post(self.path + '/refresh_metadata', json=meta)
+
+    def share(self):
+        """Share data source
+        """
+
+        self.client.post(self.path + '/share')
+
+    def get_options(self):
+        """Get data source options
+        """
+
+        r = self.client.get(self.path + '/options')
+        return r.json()['options']
+
+    def __repr__(self):
+        return self.name
```

## stardog/connection.py

```diff
@@ -640,14 +640,20 @@
             )
 
     def clear(self):
         """Removes all integrity constraints from the database.
         """
         self.client.post('/icv/clear')
 
+    def list(self):
+        """List all integrity constraints from the database.
+        """
+        r = self.client.get('/icv')
+        return r.text
+
     def is_valid(self, content, graph_uri=None):
         """Checks if given integrity constraints are valid.
 
         Args:
           content (Content): Data to check for validity
           graph_uri (str, optional): Named graph to check for validity
```

## test/test_admin.py

```diff
@@ -1,43 +1,56 @@
 import pytest
 import datetime
 import os
 
+
 import stardog.admin
 import stardog.connection as connection
 import stardog.content as content
 import stardog.content_types as content_types
 import stardog.exceptions as exceptions
 
 DEFAULT_USERS = ['admin', 'anonymous']
 DEFAULT_ROLES = ['reader']
 
 
-@pytest.fixture(scope="module")
-def admin():
-    with stardog.admin.Admin() as admin:
+@pytest.fixture()
+def admin(conn_string):
+    with stardog.admin.Admin(**conn_string) as admin:
+
+        # IMO we should remove these. reason being, if by mistake a user decides to run this
+        # tests against their own stardog deployment, and they don't go trough the code first,
+        # they are risking dropping all databases, users, roles, and others.
 
+        # alternatively we could warn somewhere (README, when running the tests, or other places)
+        # that this are not intended to run against any other stardog deployment that is not a clean one.
         for db in admin.databases():
             db.drop()
 
         for user in admin.users():
             if user.name not in DEFAULT_USERS:
                 user.delete()
 
         for role in admin.roles():
             if role.name not in DEFAULT_ROLES:
                 role.delete()
 
         for stored_query in admin.stored_queries():
             stored_query.delete()
 
+        for vg in admin.virtual_graphs():
+            vg.delete()
+
+        for ds in admin.datasources():
+            ds.delete()
+
         yield admin
 
 
-def test_databases(admin):
+def test_databases(admin, conn_string):
     assert len(admin.databases()) == 0
 
     # create database
     db = admin.new_database('db', {
         'search.enabled': True,
         'spatial.enabled': True
     })
@@ -77,37 +90,39 @@
         content.URL('https://www.w3.org/2000/10/rdf-tests/'
                     'RDF-Model-Syntax_1.0/ms_4.1_1.rdf')
     ]
 
     bl = admin.new_database('bulkload', {}, *contents)
 
     with connection.Connection(
-            'bulkload', username='admin', password='admin') as c:
+            'bulkload', **conn_string) as c:
         q = c.select('select * where { graph <urn:context> {?s ?p ?o}}')
         assert len(q['results']['bindings']) == 1
         assert c.size() == 7
 
     # clear
     db.drop()
     bl.drop()
 
     assert len(admin.databases()) == 0
 
 
-def test_backup_and_restore(admin):
+def test_backup_and_restore(admin, conn_string):
     def check_db_for_contents(dbname, num_results):
         with connection.Connection(
-                dbname, username='admin', password='admin') as c:
+                dbname, **conn_string) as c:
             q = c.select('select * where { ?s ?p ?o }')
             assert len(q['results']['bindings']) == num_results
 
     # determine the path to the backups
     now = datetime.datetime.now()
     date = now.strftime('%Y-%m-%d')
-    stardog_home = os.getenv('STARDOG_HOME', '/data/stardog')
+    # This only makes sense if stardog server is running in the same server. Recommended STARDOG_HOME
+    # should be /var/opt/stardog which I am setting as default in case of hitting a remote server.
+    stardog_home = os.getenv('STARDOG_HOME', '/var/opt/stardog')
     restore_from = os.path.join(
         f"{stardog_home}", '.backup', 'backup_db', f"{date}")
 
     # make a db with test data loaded
     db = admin.new_database(
         'backup_db', {}, content.File('test/data/starwars.ttl'))
 
@@ -142,32 +157,31 @@
     db.backup(to=os.path.join(stardog_home, 'backuptest'))
 
     # clean up
     db.drop()
     admin.database('backup_db2').drop()
 
 
-def test_users(admin):
+def test_users(admin, conn_string):
     assert len(admin.users()) == len(DEFAULT_USERS)
 
     # new user
     user = admin.new_user('username', 'password', False)
 
     assert len(admin.users()) == len(DEFAULT_USERS) + 1
     assert not user.is_superuser()
     assert user.is_enabled()
 
     # check if able to connect
-    with stardog.admin.Admin(
-            username='username', password='password') as uadmin:
+    with stardog.admin.Admin(**conn_string) as uadmin:
         uadmin.validate()
 
     # change password
     user.set_password('new_password')
-    with stardog.admin.Admin(
+    with stardog.admin.Admin(endpoint=conn_string['endpoint'],
             username='username', password='new_password') as uadmin:
         uadmin.validate()
 
     # disable/enable
     user.set_enabled(False)
     assert not user.is_enabled()
     user.set_enabled(True)
@@ -285,50 +299,98 @@
     # clear the stored queries
     stored_query = admin.new_stored_query('everything', query)
     stored_query = admin.new_stored_query('everything2', query)
     assert len(admin.stored_queries()) == 2
     admin.clear_stored_queries()
     assert len(admin.stored_queries()) == 0
 
-
-def test_virtual_graphs(admin):
+def test_virtual_graphs(admin, music_options):
     assert len(admin.virtual_graphs()) == 0
 
-    options = {
-        "namespaces": "stardog=tag:stardog:api",
-        "jdbc.driver": "com.mysql.jdbc.Driver",
-        "jdbc.username": "admin",
-        "jdbc.password": "admin",
-        "jdbc.url": "jdbc:mysql://localhost/support"
-    }
+    #creating a VG using empty mappings, and specifying a datasource
+    ds = admin.new_datasource('music', music_options)
+    vg = admin.new_virtual_graph('test_vg', mappings='', datasource=ds.name)
+    vg.delete()
+    ds.delete()
+
+    # existing datasource name, plus dbname, plus empty mappings#
+    ds = admin.new_datasource('music', music_options)
+    vg = admin.new_virtual_graph('test_vg', mappings='', datasource=ds.name, db='somedb')
+    vg.delete()
+    ds.delete()
+
+    # test passing options instead of a datasource
+    vg = admin.new_virtual_graph('test_vg', mappings='', options=music_options)
+    vg.delete()
+
+
+    # specify a mappings file, and options.
+    vg = admin.new_virtual_graph('test_vg', mappings=content.File('test/data/music_mappings.ttl'), options=music_options)
+    vg.delete()
+
+    # passing options and a datasource should not conflict
+    ds = admin.new_datasource('music', music_options)
+    vg = admin.new_virtual_graph('test_vg', mappings='', options=music_options, datasource=ds.name, db='no-db')
+    vg.delete()
+    ds.delete()
+
 
+    # Testing basic errors
     vg = admin.virtual_graph('test')
 
-    # TODO add VG to test server
-    with pytest.raises(
-            exceptions.StardogException, match='java.sql.SQLException'):
-        admin.new_virtual_graph('vg', content.File('test/data/r2rml.ttl'),
-                                options)
+    with pytest.raises(TypeError, match="missing 1 required positional argument: 'mappings'"):
+        admin.new_virtual_graph('test_vg', datasource='non-existent')
 
-    with pytest.raises(
-            exceptions.StardogException, match='java.sql.SQLException'):
-        vg.update('vg', content.File('test/data/r2rml.ttl'), options)
+    with pytest.raises(exceptions.StardogException, match='Unable to determine data source type'):
+        admin.new_virtual_graph('vg', content.File('test/data/r2rml.ttl'))
 
-    with pytest.raises(
-            exceptions.StardogException,
-            match='Virtual Graph test Not Found!'):
-        vg.available()
+    with pytest.raises(exceptions.StardogException, match='Unable to determine data source type'):
+        vg.update('vg', content.File('test/data/r2rml.ttl'))
 
-    with pytest.raises(
-            exceptions.StardogException,
-            match='Virtual Graph test Not Found!'):
+    with pytest.raises(exceptions.StardogException, match='Virtual Graph test Not Found!'):
+        vg.available()
         vg.options()
-
-    with pytest.raises(
-            exceptions.StardogException,
-            match='Virtual Graph test Not Found!'):
         vg.mappings()
-
-    with pytest.raises(
-            exceptions.StardogException,
-            match='Virtual Graph test Not Found!'):
         vg.delete()
+
+
+def count_records(bd_name, conn_string):
+
+    with connection.Connection(bd_name, **conn_string) as conn:
+        graph_name = conn.select('select ?g { graph ?g {}}')['results']['bindings'][0]['g']['value']
+        q = conn.select('SELECT * { GRAPH <' + graph_name + '> { ?s ?p ?o }}')
+        count = len(q['results']['bindings'])
+    return count
+
+
+def test_import(admin, conn_string, music_options, videos_options):
+
+    bd = admin.new_database('test-db')
+    graph_name = 'test-graph'
+
+    # tests passing mappings
+    admin.import_virtual_graph('test-db', mappings=content.File('test/data/music_mappings.ttl'), named_graph=graph_name, remove_all=True, options=music_options)
+    # specified mapping file generates a graph with total of 37 triples
+    assert 37 == count_records(bd.name, conn_string)
+
+    # tests passing empty mappings
+    admin.import_virtual_graph('test-db', mappings='', named_graph=graph_name, remove_all=True, options=music_options)
+    # if mapping is not specified, music bd generates a graph with 79 triples
+    assert 79 == count_records(bd.name, conn_string)
+
+    # test removing_all false, it should return  music records + video records.
+    admin.import_virtual_graph('test-db', mappings='', named_graph=graph_name, remove_all=False, options=videos_options)
+    # if no mapping is specified, videos db generates a graph with 800 triples. adding un-mapped music sums up to 879.
+    assert 879 == count_records(bd.name, conn_string)
+
+def test_data_source(admin, music_options):
+
+    ds = admin.new_datasource('music', music_options)
+    assert len(admin.datasources()) == 1
+    assert ds.name == 'music'
+    assert ds.get_options() == music_options
+    ds.delete()
+    assert len(admin.datasources()) == 0
+
+
+
+
```

## test/test_connection.py

```diff
@@ -3,23 +3,23 @@
 import stardog.admin
 import stardog.connection as connection
 import stardog.content as content
 import stardog.content_types as content_types
 import stardog.exceptions as exceptions
 
 
-@pytest.fixture(scope="module")
-def conn():
-    with connection.Connection('newtest') as conn:
+@pytest.fixture()
+def conn(conn_string):
+    with connection.Connection('newtest', **conn_string) as conn:
         yield conn
 
 
-@pytest.fixture(scope="module", autouse="True")
-def db():
-    with stardog.admin.Admin() as admin:
+@pytest.fixture(autouse="True")
+def db(conn_string):
+    with stardog.admin.Admin(**conn_string) as admin:
         db = admin.new_database('newtest', {'search.enabled': True})
         yield admin
         db.drop()
 
 
 def test_transactions(conn):
     data = content.Raw('<urn:subj> <urn:pred> <urn:obj> .', content_types.TURTLE)
@@ -316,22 +316,21 @@
     conn.add(content.Raw(':Alice a :Employee .', content_types.TURTLE))
     conn.commit()
 
     assert icv.is_valid(constraint)
 
     assert 'SELECT DISTINCT' in icv.convert(constraint)
 
-
-def test_graphql():
-    with stardog.admin.Admin() as admin:
+def test_graphql(conn_string):
+    with stardog.admin.Admin(**conn_string) as admin:
         db = admin.new_database('graphql', {},
                             content.File('test/data/starwars.ttl'))
 
     with connection.Connection(
-            'graphql', username='admin', password='admin') as c:
+            'graphql', **conn_string) as c:
         gql = c.graphql()
 
         # query
         assert gql.query('{ Planet { system } }') == [{
             'system': 'Tatoo'
         }, {
             'system': 'Alderaan'
```

## Comparing `pystardog-0.9.8.dist-info/LICENSE` & `pystardog-0.9.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pystardog-0.9.8.dist-info/METADATA` & `pystardog-0.9.9.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystardog
-Version: 0.9.8
+Version: 0.9.9
 Summary: Use Stardog with Python!
 Home-page: https://github.com/stardog-union/pystardog
 Author: Stardog Union
 Author-email: support@stardog.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -43,33 +43,19 @@
 
     pip install -r requirements.txt
     cd docs
     make html
 
 ## Tests
 
-Create a virtual environment:
+To run the tests locally, a valid Stardog license is required and placed in the `dockerfiles/stardog-license-key.bin`. 
+Docker and docker-compose are also required.
 
 ```shell script
-virtualenv -p $(which python3) venv
-```
-
-Activate the virtualenv:
-
-```shell script
-$ . venv/bin/activate
-(venv) $
-```
-Install the dependencies
-```shell script
-pip install -r requirements.txt
-```
-Run the tests 
-```
-python setup.py test
+docker-compose up --exit-code-from tests
 ```
 
 ## Quick Example
 
 ```python
 import stardog
```

## Comparing `pystardog-0.9.8.dist-info/RECORD` & `pystardog-0.9.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 stardog/__init__.py,sha256=-5LomLxFHjxwKwcg1sk5Dno_pqGIneb6eXS_83f2Woc,261
-stardog/admin.py,sha256=FvSBCFsjnSshpNAxm1S5Eq-SLldrMwql_jnk1uFgyz0,26876
-stardog/connection.py,sha256=yY4RTLBKJqoQ63hSTjBcyCw7l-UHTBEHWskB6Hai-ms,25253
+stardog/admin.py,sha256=Bk77WcyKqPp5AXojCyxqxU7BLcWTbzCEQw71ZNt_KW8,33580
+stardog/connection.py,sha256=DsaAbOwIDLkzDWr5lD_nbzMVg9AyEqFHcFnAhfECqVc,25405
 stardog/content.py,sha256=3zhgN8nPGR4qywpKAMbpu7whvRLcepni9suho7qhGIk,3514
 stardog/content_types.py,sha256=8WABigLt7cT4oMjAtlDyWOKNqlbOFntqaohJQJEO9aE,1660
 stardog/exceptions.py,sha256=5yriWYziw3vHBXUBbrEtzG2ipiMUnQIg0DDNXFU_Mz8,181
 stardog/http/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 stardog/http/client.py,sha256=zZlr8nL3XMwkTQBZ-lo9J6m5Ph1WlwUwX9xju8TUcaU,2179
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-test/test_admin.py,sha256=tfduUVjG9yTh8RFTAbEvyU3nF6v1CGTp0MbzS0I-aks,9076
-test/test_connection.py,sha256=auNR21h1z7sCbRL4pCSOFgaSOJnB3xpy4ORlqNiH2YA,9944
+test/conftest.py,sha256=rd6nnFWjp5iluKXLx58q9BTBhiy1rzAZz47n0HXWGUo,1373
+test/test_admin.py,sha256=8dx0wHBpAAjDHNvZjd30HAyrYmgZmIQxIvlM_hDDIBA,12202
+test/test_connection.py,sha256=OWieaI-RcVKvf3mwqAcaRJc8MBr-id5N-NR7bAkpFgU,9966
 test/test_utils.py,sha256=_HljUChn3qBeCCJ8BPnf3RWRmJbRc1rjEp_YXLNG4sg,1118
-pystardog-0.9.8.dist-info/LICENSE,sha256=CXVamMJjLNpBYqeUESRVDB24Si5t1S9-IaZUXD49TR0,554
-pystardog-0.9.8.dist-info/METADATA,sha256=jJ-qyGre5s0hLPb-KLj1azzrXU-ONgeqoII04oIvsfM,2257
-pystardog-0.9.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-pystardog-0.9.8.dist-info/top_level.txt,sha256=r4cVimQwJElzUY-DQ8MLyJffyQkNxvCwQnokl4_u590,13
-pystardog-0.9.8.dist-info/RECORD,,
+pystardog-0.9.9.dist-info/LICENSE,sha256=CXVamMJjLNpBYqeUESRVDB24Si5t1S9-IaZUXD49TR0,554
+pystardog-0.9.9.dist-info/METADATA,sha256=aH9QmhQSmwBxabYrvBUn-d8wK9zH4SvvYLGMfCL44ms,2198
+pystardog-0.9.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+pystardog-0.9.9.dist-info/top_level.txt,sha256=r4cVimQwJElzUY-DQ8MLyJffyQkNxvCwQnokl4_u590,13
+pystardog-0.9.9.dist-info/RECORD,,
```

