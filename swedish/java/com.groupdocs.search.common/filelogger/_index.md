---
title: "FileLogger"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en logger som loggar händelser och fel till en lokal fil."
type: docs
weight: 20
url: /sv/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Representerar en logger som loggar händelser och fel till en lokal fil.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Anger sökvägen till loggfilen och en maximal längd på 4 MB
Index index = new Index(indexFolder, settings); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchResult result = index.search(query); // Sök i indexet
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Initierar en ny instans av klassen FileLogger. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Loggar ett fel som inträffade i indexet. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Loggar en händelse som inträffade i indexet. |
|
|  | [getFilePath()](#getFilePath--) | Hämtar sökvägen till loggfilen. |
|
|  | [getMaxSize()](#getMaxSize--) | Hämtar den maximala storleken på loggfilen i megabyte. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Initierar en ny instans av klassen FileLogger.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Loggfilens sökväg. |
|
|  | maxSize | double | Den maximala storleken på loggfilen i megabyte. Värdet måste ligga i intervallet från 0,1 till 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Loggar ett fel som inträffade i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | meddelande | java.lang.String | Felmeddelandet. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Loggar en händelse som inträffade i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | meddelande | java.lang.String | Händelsemeddelandet. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Hämtar sökvägen till loggfilen.


**Returns:**
java.lang.String - Loggfilens sökväg.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Hämtar den maximala storleken på loggfilen i megabyte.


**Returns:**
double - Den maximala storleken på loggfilen i megabyte.

