---
title: "FileLogger"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un logger che registra eventi ed errori in un file locale."
type: docs
weight: 20
url: /it/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Rappresenta un logger che registra eventi ed errori in un file locale.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Specifica il percorso del file di log e una lunghezza massima di 4 MB
Index index = new Index(indexFolder, settings); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchResult result = index.search(query); // Ricerca nell'indice
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Inizializza una nuova istanza della classe  FileLogger  . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Registra un errore verificatosi nell'indice. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Registra un evento verificatosi nell'indice. |
|
|  | [getFilePath()](#getFilePath--) | Ottiene il percorso del file di log. |
|
|  | [getMaxSize()](#getMaxSize--) | Ottiene la dimensione massima del file di log in megabyte. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Inizializza una nuova istanza della classe  FileLogger  .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | filePath | java.lang.String | Il percorso del file di log. |
|
|  | maxSize | double | La dimensione massima del file di log in megabyte. Il valore deve essere nell'intervallo da 0.1 a 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Registra un errore verificatosi nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | messaggio | java.lang.String | Il messaggio di errore. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Registra un evento verificatosi nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | messaggio | java.lang.String | Il messaggio dell'evento. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Ottiene il percorso del file di log.


**Returns:**
java.lang.String - Il percorso del file di log.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Ottiene la dimensione massima del file di log in megabyte.


**Returns:**
double - La dimensione massima del file di log in megabyte.

