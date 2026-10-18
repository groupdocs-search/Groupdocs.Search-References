---
title: "FileLogger"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Logger dar, der Ereignisse und Fehler in eine lokale Datei protokolliert."
type: docs
weight: 20
url: /de/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Stellt einen Logger dar, der Ereignisse und Fehler in eine lokale Datei protokolliert.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Pfad zur Protokolldatei und eine maximale Länge von 4 MB angeben
Index index = new Index(indexFolder, settings); // Einen Index im angegebenen Ordner erstellen
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchResult result = index.search(query); // Suche im Index
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Initialisiert eine neue Instanz der  FileLogger  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Protokolliert einen Fehler, der im Index aufgetreten ist. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Protokolliert ein Ereignis, das im Index aufgetreten ist. |
|
|  | [getFilePath()](#getFilePath--) | Liefert den Pfad der Protokolldatei. |
|
|  | [getMaxSize()](#getMaxSize--) | Liefert die maximale Größe der Protokolldatei in Megabyte. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Initialisiert eine neue Instanz der  FileLogger  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | filePath | java.lang.String | Der Pfad der Protokolldatei. |
|
|  | maxSize | double | Die maximale Größe der Protokolldatei in Megabyte. Der Wert muss im Bereich von 0,1 bis 1000 liegen. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Protokolliert einen Fehler, der im Index aufgetreten ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | message | java.lang.String | Die Fehlermeldung. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Protokolliert ein Ereignis, das im Index aufgetreten ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | message | java.lang.String | Die Ereignismeldung. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Liefert den Pfad der Protokolldatei.


**Returns:**
java.lang.String - Der Pfad der Protokolldatei.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Liefert die maximale Größe der Protokolldatei in Megabyte.


**Returns:**
double - Die maximale Größe der Protokolldatei in Megabyte.

