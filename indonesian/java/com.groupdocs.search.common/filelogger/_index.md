---
title: "FileLogger"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili logger yang mencatat peristiwa dan kesalahan ke file lokal."
type: docs
weight: 20
url: /id/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Mewakili logger yang mencatat peristiwa dan kesalahan ke file lokal.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Menentukan jalur ke file log dan panjang maksimum 4 MB
Index index = new Index(indexFolder, settings); // Membuat indeks di folder yang ditentukan
index.add(documentsFolder); // Mengindeks dokumen dari folder yang ditentukan
SearchResult result = index.search(query); // Cari di indeks
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Menginisialisasi sebuah instance baru dari kelas  FileLogger  . |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Mencatat kesalahan yang terjadi di indeks. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Mencatat peristiwa yang terjadi di indeks. |
|
|  | [getFilePath()](#getFilePath--) | Mendapatkan jalur file log. |
|
|  | [getMaxSize()](#getMaxSize--) | Mendapatkan ukuran maksimum file log dalam megabyte. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Menginisialisasi sebuah instance baru dari kelas  FileLogger  .


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Jalur file log. |
|
|  | maxSize | double | Ukuran maksimum file log dalam megabyte. Nilai harus berada dalam rentang dari 0.1 hingga 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Mencatat kesalahan yang terjadi di indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | message | java.lang.String | Pesan kesalahan. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Mencatat peristiwa yang terjadi di indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | message | java.lang.String | Pesan peristiwa. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Mendapatkan jalur file log.


**Returns:**
java.lang.String - Jalur file log.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Mendapatkan ukuran maksimum file log dalam megabyte.


**Returns:**
double - Ukuran maksimum file log dalam megabyte.

