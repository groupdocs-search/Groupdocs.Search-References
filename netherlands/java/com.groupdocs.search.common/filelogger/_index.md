---
title: "FileLogger"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een logger voor die gebeurtenissen en fouten naar een lokaal bestand logt."
type: docs
weight: 20
url: /nl/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Stelt een logger voor die gebeurtenissen en fouten naar een lokaal bestand logt.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Het pad naar het logbestand opgeven en een maximale lengte van 4 MB
Index index = new Index(indexFolder, settings); // Een index maken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchResult result = index.search(query); // Zoek in index
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Initialiseert een nieuw exemplaar van de  FileLogger  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Logt een fout die zich in de index heeft voorgedaan. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Logt een gebeurtenis die zich in de index heeft voorgedaan. |
|
|  | [getFilePath()](#getFilePath--) | Haalt het pad van het logbestand op. |
|
|  | [getMaxSize()](#getMaxSize--) | Haalt de maximale grootte van het logbestand op in megabytes. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Initialiseert een nieuw exemplaar van de  FileLogger  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het pad van het logbestand. |
|
|  | maxSize | double | De maximale grootte van het logbestand in megabytes. De waarde moet liggen in het bereik van 0,1 tot 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Logt een fout die zich in de index heeft voorgedaan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | bericht | java.lang.String | Het foutbericht. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Logt een gebeurtenis die zich in de index heeft voorgedaan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | bericht | java.lang.String | Het gebeurtenisbericht. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Haalt het pad van het logbestand op.


**Returns:**
java.lang.String - Het pad van het logbestand.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Haalt de maximale grootte van het logbestand op in megabytes.


**Returns:**
double - De maximale grootte van het logbestand in megabytes.

