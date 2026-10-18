---
title: "SearchReport"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir arama işlemiyle ilgili ayrıntılı bilgiyi temsil eder."
type: docs
weight: 30
url: /tr/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Bir arama işlemiyle ilgili ayrıntılı bilgiyi temsil eder.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Belirtilen klasörde bir indeks oluşturma
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentsFolder);
// Dizinde arama
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Arama raporları alınıyor
SearchReport[] reports = index.getSearchReports();
// Konsola raporları yazdırma
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Aramanın başlangıç zamanını alır. |
|
|  | [getEndTime()](#getEndTime--) | Aramanın bitiş zamanını alır. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Aramanın süresini saniye cinsinden alır. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Bulunan belge sayısını alır. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Bulunan toplam oluşum sayısını alır. |
|
|  | [getTextQuery()](#getTextQuery--) | Arama sorgusunu metin biçiminde alır. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Arama sorgusunu nesne biçiminde alır. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Arama seçeneklerini alır. |
|
|  | [toString()](#toString--) | Geçerli SearchReport'ı temsil eden bir String döndürür. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Aramanın başlangıç zamanını alır.


**Returns:**
java.util.Date - Aramanın başlangıç zamanı.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Aramanın bitiş zamanını alır.


**Returns:**
java.util.Date - Aramanın bitiş zamanı.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Aramanın süresini saniye cinsinden alır.


**Returns:**
double - Aramanın süresi saniye cinsinden.

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Bulunan belge sayısını alır.


**Returns:**
int - Bulunan belge sayısı.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Bulunan toplam oluşum sayısını alır.


**Returns:**
int - Bulunan toplam oluşum sayısı.

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Arama sorgusunu metin biçiminde alır.


**Returns:**
java.lang.String - Arama sorgusu metin biçiminde.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Arama sorgusunu nesne biçiminde alır.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Arama seçeneklerini alır.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Geçerli SearchReport'ı temsil eden bir String döndürür.


**Returns:**
java.lang.String - Geçerli SearchReport'ı temsil eden bir String.

