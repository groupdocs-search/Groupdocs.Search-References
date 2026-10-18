---
title: "IndexUpdater"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un actualizador de índice."
type: docs
weight: 20
url: /es/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Representa un actualizador de índices. Esta clase realiza la reindexación de documentos en un índice de una versión anterior.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


El ejemplo muestra un uso típico de la clase.

````
 ```

String sourceIndexFolder = "c:\\MyOldIndex\\";
String targetIndexFolder = "c:\\MyNewIndex\\";
IndexUpdater updater = new IndexUpdater();
if (updater.canUpdateVersion(sourceIndexFolder)) {
int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
}
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Inicializa una nueva instancia de la  IndexUpdater  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Comprueba si el directorio especificado contiene un índice de la última versión. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Comprueba si un índice en el directorio especificado puede actualizarse a la última versión. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Realiza la reindexación de documentos en un índice de una versión anterior. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Inicializa una nueva instancia de la  IndexUpdater  clase.


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Comprueba si el directorio especificado contiene un índice de la última versión.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexPath | java.lang.String | La ruta del directorio del índice. |
|

**Returns:**
boolean -  true  si el directorio especificado contiene un índice de la última versión; de lo contrario  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Comprueba si un índice en el directorio especificado puede actualizarse a la última versión.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexPath | java.lang.String | La ruta del directorio del índice. |
|

**Returns:**
boolean -  true  si un índice en el directorio especificado puede actualizarse a la última versión; de lo contrario  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Realiza la reindexación de documentos en un índice de una versión anterior. El índice actualizado se colocará en el directorio  newIndexPath . El índice en el directorio  indexPath  no se modificará.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | indexPath | java.lang.String | La ruta del directorio del índice. |
|
|  | newIndexPath | java.lang.String | El directorio para el índice actualizado. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

