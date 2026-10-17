---
title: "IndexUpdater"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une mise à jour d'index."
type: docs
weight: 20
url: /fr/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Représente un IndexUpdater. Cette classe réindexe les documents dans un index d'une ancienne version.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


L'exemple montre une utilisation typique de la classe.

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


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Initialise une nouvelle instance de la classe  IndexUpdater  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Vérifie si le répertoire spécifié contient un index de la dernière version. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Vérifie si un index dans le répertoire spécifié peut être mis à jour vers la dernière version. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Effectue le réindexage des documents dans un index d'une ancienne version. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Initialise une nouvelle instance de la classe  IndexUpdater  .


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Vérifie si le répertoire spécifié contient un index de la dernière version.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexPath | java.lang.String | Le chemin du répertoire d'index. |
|

**Returns:**
booléen -  true  si le répertoire spécifié contient un index de la dernière version ; sinon  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Vérifie si un index dans le répertoire spécifié peut être mis à jour vers la dernière version.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexPath | java.lang.String | Le chemin du répertoire d'index. |
|

**Returns:**
booléen -  true  si un index dans le répertoire spécifié peut être mis à jour vers la dernière version ; sinon  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Effectue le réindexage des documents dans un index d'une ancienne version. L'index mis à jour sera placé dans le répertoire  newIndexPath . L'index dans le répertoire  indexPath  ne sera pas modifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | indexPath | java.lang.String | Le chemin du répertoire d'index. |
|
|  | newIndexPath | java.lang.String | Le répertoire pour l'index mis à jour. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

