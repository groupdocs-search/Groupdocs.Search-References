---
title: "FileLogger"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Olayları ve hataları yerel bir dosyaya kaydeden bir günlüğü temsil eder."
type: docs
weight: 20
url: /tr/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Olayları ve hataları yerel bir dosyaya kaydeden bir günlüğü temsil eder.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Günlük dosyasının yolunu ve maksimum 4 MB uzunluğunu belirtiyor
Index index = new Index(indexFolder, settings); // Belirtilen klasörde bir indeks oluşturuluyor
index.add(documentsFolder); // Belirtilen klasörden belgeleri indeksleme
SearchResult result = index.search(query); // İndekste arama
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | FileLogger sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | İndekte meydana gelen bir hatayı kaydeder. |
|
|  | [trace(String message)](#trace-java.lang.String-) | İndekte meydana gelen bir olayı kaydeder. |
|
|  | [getFilePath()](#getFilePath--) | Günlük dosyası yolunu alır. |
|
|  | [getMaxSize()](#getMaxSize--) | Günlük dosyasının megabayt cinsinden maksimum boyutunu alır. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


FileLogger sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Günlük dosyası yolu. |
|
|  | maxSize | double | Log dosyasının megabayt cinsinden maksimum boyutu. Değer 0.1 ile 1000 arasında olmalıdır. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


İndekte meydana gelen bir hatayı kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | mesaj | java.lang.String | Hata mesajı. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


İndekte meydana gelen bir olayı kaydeder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | mesaj | java.lang.String | Olay mesajı. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Günlük dosyası yolunu alır.


**Returns:**
java.lang.String - Log dosyasının yolu.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Günlük dosyasının megabayt cinsinden maksimum boyutunu alır.


**Returns:**
double - Log dosyasının megabayt cinsinden maksimum boyutu.

