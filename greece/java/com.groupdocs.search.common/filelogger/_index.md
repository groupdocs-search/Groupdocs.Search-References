---
title: "FileLogger"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά έναν καταγραφέα που καταγράφει συμβάντα και σφάλματα σε τοπικό αρχείο."
type: docs
weight: 20
url: /el/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Αναπαριστά έναν καταγραφέα που καταγράφει συμβάντα και σφάλματα σε τοπικό αρχείο.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Καθορισμός της διαδρομής του αρχείου καταγραφής και μέγιστου μεγέθους 4 MB
Index index = new Index(indexFolder, settings); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
SearchResult result = index.search(query); // Αναζήτηση στο ευρετήριο
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Αρχικοποιεί μια νέα παρουσία της κλάσης  FileLogger . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Καταγράφει ένα σφάλμα που συνέβη στο ευρετήριο. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Καταγράφει ένα γεγονός που συνέβη στο ευρετήριο. |
|
|  | [getFilePath()](#getFilePath--) | Λαμβάνει τη διαδρομή του αρχείου καταγραφής. |
|
|  | [getMaxSize()](#getMaxSize--) | Λαμβάνει το μέγιστο μέγεθος του αρχείου καταγραφής σε megabytes. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  FileLogger .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή του αρχείου καταγραφής. |
|
|  | maxSize | double | Το μέγιστο μέγεθος του αρχείου καταγραφής σε megabytes. Η τιμή πρέπει να είναι στο εύρος από 0.1 έως 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Καταγράφει ένα σφάλμα που συνέβη στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | μήνυμα | java.lang.String | Το μήνυμα σφάλματος. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Καταγράφει ένα γεγονός που συνέβη στο ευρετήριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | μήνυμα | java.lang.String | Το μήνυμα γεγονότος. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Λαμβάνει τη διαδρομή του αρχείου καταγραφής.


**Returns:**
java.lang.String - Η διαδρομή του αρχείου καταγραφής.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Λαμβάνει το μέγιστο μέγεθος του αρχείου καταγραφής σε megabytes.


**Returns:**
double - Το μέγιστο μέγεθος του αρχείου καταγραφής σε megabytes.

