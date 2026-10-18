---
title: "IndexUpdater"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en indexuppdaterare."
type: docs
weight: 20
url: /sv/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Representerar en indexuppdaterare. Denna klass utför omindexering av dokument i ett index av en äldre version.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

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


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Initierar en ny instans av klassen  IndexUpdater  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Kontrollerar om den angivna katalogen innehåller ett index av den senaste versionen. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Kontrollerar om ett index i den angivna katalogen kan uppdateras till den senaste versionen. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Utför omindexering av dokument i ett index av en äldre version. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Initierar en ny instans av klassen  IndexUpdater  .


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Kontrollerar om den angivna katalogen innehåller ett index av den senaste versionen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexPath | java.lang.String | Sökvägen till indexkatalogen. |
|

**Returns:**
boolean -  true  om den angivna katalogen innehåller ett index av den senaste versionen; annars  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Kontrollerar om ett index i den angivna katalogen kan uppdateras till den senaste versionen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexPath | java.lang.String | Sökvägen till indexkatalogen. |
|

**Returns:**
boolean -  true  om ett index i den angivna katalogen kan uppdateras till den senaste versionen; annars  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Utför omindexering av dokument i ett index av en äldre version. Det uppdaterade indexet kommer att placeras i katalogen  newIndexPath . Indexet i katalogen  indexPath  kommer inte att ändras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | indexPath | java.lang.String | Sökvägen till indexkatalogen. |
|
|  | newIndexPath | java.lang.String | Katalogen för det uppdaterade indexet. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

