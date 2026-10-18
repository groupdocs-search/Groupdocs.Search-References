---
title: "IndexingReport"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir indeksleme işlemi hakkında ayrıntılı bilgiyi temsil eder."
type: docs
weight: 25
url: /tr/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Bir indeksleme işlemi hakkında ayrıntılı bilgiyi temsil eder.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belgeleri indeksleme
index.add(documentsFolder1);
index.add(documentsFolder2);
// İndeksleme raporları alınıyor
IndexingReport[] reports = index.getIndexingReports();
// Konsola raporları yazdırma
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Dizindeki toplam belge sayısını alır. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Dizindeki toplam terim sayısını alır. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Dizine eklenen belgelerin toplam uzunluğunu MB cinsinden alır. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Dizin segment sayısını alır. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Toplam dizin boyutunu bayt cinsinden alır. |
|
|  | [getStartTime()](#getStartTime--) | Dizinleme başlangıç zamanını alır. |
|
|  | [getEndTime()](#getEndTime--) | Dizinleme bitiş zamanını alır. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Dizinleme süresini saniye cinsinden alır. |
|
|  | [getErrors()](#getErrors--) | Hata listesini alır. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Dizine eklenen belgelerin listesini alır. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Güncellenen belgelerin listesini alır. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Dizinden kaldırılan belgelerin listesini alır. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Dizindeki toplam belge sayısını alır.


**Returns:**
int - Dizindeki toplam belge sayısı.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Dizindeki toplam terim sayısını alır.


**Returns:**
int - Dizindeki toplam terim sayısı.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Dizine eklenen belgelerin toplam uzunluğunu MB cinsinden alır.


**Returns:**
double - Dizine eklenen belgelerin toplam uzunluğu MB cinsinden.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Dizin segment sayısını alır.


**Returns:**
int - Dizin segment sayısı.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Toplam dizin boyutunu bayt cinsinden alır.


**Returns:**
long - Toplam dizin boyutu bayt cinsinden.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Dizinleme başlangıç zamanını alır.


**Returns:**
java.util.Date - Dizinleme başlangıç zamanı.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Dizinleme bitiş zamanını alır.


**Returns:**
java.util.Date - İndeksleme bitiş zamanı.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Dizinleme süresini saniye cinsinden alır.


**Returns:**
double - İndeksleme süresi saniye cinsinden.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Hata listesini alır.


**Returns:**
java.lang.String[] - Hataların listesi.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Dizine eklenen belgelerin listesini alır.


**Returns:**
java.lang.String[] - İndekslenmiş belgelerin listesi.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Güncellenen belgelerin listesini alır.


**Returns:**
java.lang.String[] - Güncellenmiş belgelerin listesi.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Dizinden kaldırılan belgelerin listesini alır.


**Returns:**
java.lang.String[] - Dizinden kaldırılan belgelerin listesi.

