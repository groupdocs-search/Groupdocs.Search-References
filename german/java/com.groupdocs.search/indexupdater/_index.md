---
title: "IndexUpdater"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Index-Aktualisierer dar."
type: docs
weight: 20
url: /de/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Stellt einen IndexUpdater dar. Diese Klasse führt die Neuinindexierung von Dokumenten in einem Index einer alten Version durch.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

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


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Initialisiert eine neue Instanz der  IndexUpdater  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Prüft, ob das angegebene Verzeichnis einen Index der neuesten Version enthält. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Prüft, ob ein Index im angegebenen Verzeichnis auf die neueste Version aktualisiert werden kann. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Führt die Neuinindexierung von Dokumenten in einem Index einer alten Version durch. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Initialisiert eine neue Instanz der  IndexUpdater  Klasse.


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Prüft, ob das angegebene Verzeichnis einen Index der neuesten Version enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexPath | java.lang.String | Der Pfad des Indexverzeichnisses. |
|

**Returns:**
boolean -  true  wenn das angegebene Verzeichnis einen Index der neuesten Version enthält; andernfalls  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Prüft, ob ein Index im angegebenen Verzeichnis auf die neueste Version aktualisiert werden kann.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexPath | java.lang.String | Der Pfad des Indexverzeichnisses. |
|

**Returns:**
boolean -  true  wenn ein Index im angegebenen Verzeichnis auf die neueste Version aktualisiert werden kann; andernfalls  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Führt die Neuinindexierung von Dokumenten in einem Index einer alten Version durch. Der aktualisierte Index wird im Verzeichnis  newIndexPath  abgelegt. Der Index im Verzeichnis  indexPath  wird nicht geändert.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | indexPath | java.lang.String | Der Pfad des Indexverzeichnisses. |
|
|  | newIndexPath | java.lang.String | Das Verzeichnis für den aktualisierten Index. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

