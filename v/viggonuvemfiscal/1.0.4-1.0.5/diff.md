# Comparing `tmp/viggonuvemfiscal-1.0.4.tar.gz` & `tmp/viggonuvemfiscal-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggonuvemfiscal-1.0.4.tar", last modified: Thu Mar  2 13:27:45 2023, max compression
+gzip compressed data, was "viggonuvemfiscal-1.0.5.tar", last modified: Wed Apr 19 13:20:06 2023, max compression
```

## Comparing `viggonuvemfiscal-1.0.4.tar` & `viggonuvemfiscal-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.265880 viggonuvemfiscal-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 13:27:45.265880 viggonuvemfiscal-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/viggonuvemfiscal/
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-03-02 13:26:53.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:27:45.261880 viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-02 13:27:45.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-02 13:27:45.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:27:45.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-02 13:27:45.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-02 13:27:45.000000 viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.185099 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-19 13:19:01.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:20:06.181099 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-19 13:20:06.000000 viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/top_level.txt
```

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/__init__.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/__init__.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/resources.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/resources.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/manager.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/resource.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/configuracao_nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/controller.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     def do(self, session, **kwargs):
         nfe_id = self.manager.get_nfe_id(**kwargs)
         url = self.manager.get_endpoint(f'/nfe/{nfe_id}')
         return self.manager.executar_requisicao('GET', url)
 
 
-class BaixarXml(operation.List):
+class BaixarXmlNfe(operation.List):
 
     def do(self, session, **kwargs):
         nfe_id = self.manager.get_nfe_id(**kwargs)
         url = self.manager.get_endpoint(f'/nfe/{nfe_id}/xml')
         return self.manager.executar_requisicao('GET', url)
 
 
@@ -178,15 +178,15 @@
         self.consultar_configuracao_nfe = ConsultarConfiguracaoNfe(self)
         self.alterar_configuracao_nfe = AlterarConfiguracaoNfe(self)
         self.emitir_nfe = EmitirNfe(self)
         self.listar_nfe = ListarNfe(self)
         self.consulta_status_do_servico_na_sefaz_autorizadora = \
             ConsultaStatusDoServicoNaSefazAutorizadora(self)
         self.consultar_nfe = ConsultarNfe(self)
-        self.baixar_xml = BaixarXml(self)
+        self.baixar_xml_nfe = BaixarXmlNfe(self)
         self.consultar_cancelamento_nfe = ConsultarCancelamentoNfe(self)
         self.baixar_xml_cancelamento_nfe = BaixarXmlCancelamentoNfe(self)
         self.cancelar_nfe_autorizada = CancelarNfeAutorizada(self)
 
     def get_authorization(self):
         config = self.api.configuracao_nuvem_fiscals().\
             get_configuracao_nuvem_fiscal()
```

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal/subsystem/controle/nuvem_fiscal/router.py`

 * *Files identical despite different names*

### Comparing `viggonuvemfiscal-1.0.4/viggonuvemfiscal.egg-info/SOURCES.txt` & `viggonuvemfiscal-1.0.5/viggonuvemfiscal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

