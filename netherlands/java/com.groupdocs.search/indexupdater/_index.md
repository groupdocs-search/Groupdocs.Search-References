---
title: "IndexUpdater"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een indexbijwerker voor."
type: docs
weight: 20
url: /nl/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Stelt een index-updater voor. Deze klasse voert het opnieuw indexeren van documenten uit in een index van een oude versie.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Het voorbeeld toont een typisch gebruik van de klasse.

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


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Initialiseert een nieuw exemplaar van de  IndexUpdater  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Controleert of de opgegeven map een index van de nieuwste versie bevat. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Controleert of een index in de opgegeven map kan worden bijgewerkt naar de nieuwste versie. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Voert het opnieuw indexeren van documenten uit in een index van een oude versie. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Initialiseert een nieuw exemplaar van de  IndexUpdater  klasse.


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Controleert of de opgegeven map een index van de nieuwste versie bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexPath | java.lang.String | Het pad van de indexmap. |
|

**Returns:**
boolean -  true  als de opgegeven map een index van de nieuwste versie bevat; anders  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Controleert of een index in de opgegeven map kan worden bijgewerkt naar de nieuwste versie.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexPath | java.lang.String | Het pad van de indexmap. |
|

**Returns:**
boolean -  true  als een index in de opgegeven map kan worden bijgewerkt naar de nieuwste versie; anders  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Voert het opnieuw indexeren van documenten uit in een index van een oude versie. De bijgewerkte index wordt geplaatst in de  newIndexPath  map. De index in de  indexPath  map zal niet worden gewijzigd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | indexPath | java.lang.String | Het pad van de indexmap. |
|
|  | newIndexPath | java.lang.String | De map voor de bijgewerkte index. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

