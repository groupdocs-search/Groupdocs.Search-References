---
title: FileLogger
second_title: GroupDocs.Search for Java API Reference
description: Represents a logger that logs events and errors to a local file.
type: docs
weight: 20
url: /java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Represents a logger that logs events and errors to a local file.

**Learn more**

 *  [Logging][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 String logPath = "c:\\Log.txt";
 IndexSettings settings = new IndexSettings();
 settings.setLogger(new FileLogger(logPath, 4.0)); // Specifying the path to the log file and a maximum length of 4 MB
 Index index = new Index(indexFolder, settings); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchResult result = index.search(query); // Search in index
 
```


[Logging]: https://docs.groupdocs.com/display/searchjava/Logging
## Constructors

| Constructor | Description |
| --- | --- |
| [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Initializes a new instance of the  FileLogger  class. |
## Methods

| Method | Description |
| --- | --- |
| [error(String message)](#error-java.lang.String-) | Logs an error that occurred in the index. |
| [trace(String message)](#trace-java.lang.String-) | Logs an event that occurred in the index. |
| [getFilePath()](#getFilePath--) | Gets the log file path. |
| [getMaxSize()](#getMaxSize--) | Gets the maximum size of log file in megabytes. |
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Initializes a new instance of the  FileLogger  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The log file path. |
| maxSize | double | The maximum size of the log file in megabytes. The value must be in the range from 0.1 to 1000. |

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Logs an error that occurred in the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The error message. |

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Logs an event that occurred in the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The event message. |

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Gets the log file path.

**Returns:**
java.lang.String - The log file path.
### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Gets the maximum size of log file in megabytes.

**Returns:**
double - The maximum size of log file in megabytes.
