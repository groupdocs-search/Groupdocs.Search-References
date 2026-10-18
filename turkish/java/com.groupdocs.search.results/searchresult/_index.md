---
title: "SearchResult"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama sorgusuyla eşleşen bir arama sonucunu temsil eder."
type: docs
weight: 19
url: /tr/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Arama sorgusuyla eşleşen bir arama sonucunu temsil eder.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Örnek, sınıfın tipik bir kullanımını gösterir.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Bir indeks oluşturuluyor
Index index = new Index(indexFolder);
// Belirtilen klasörden belgeler indeksleniyor
index.add(documentFolder);
// Arama seçeneklerini ayarlama
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Bulanık aramayı etkinleştiriyor
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Maksimum fark sayısını 3 olarak ayarlama
// 'Einstein' kelimesini veya 'Theory of Relativity' ifadesini içeren belgeleri ara
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Sonucu yazdırma
System.out.println("Belgeler: " + result.getDocumentCount());
System.out.println("Toplam oluşumlar: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tBelge: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOluşumlar: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tAlan: " + field.getFieldName());
System.out.println("\t\tOluşumlar: " + document.getOccurrenceCount());
// Bulunan terimleri yazdırma
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Bulunan ifadeleri yazdırma
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Bulunan belge sayısını alır. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Bulunan toplam oluşum sayısını alır. |
|
|  | [getTruncated()](#getTruncated--) | Sonucun kesildiğini gösteren bir değeri alır. |
|
|  | [getWarnings()](#getWarnings--) | Sonucu açıklayan uyarıları alır. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Sonraki parçayı aramak için bir chunk arama token'ı alır. |
|
|  | [getStartTime()](#getStartTime--) | Aramanın başlangıç zamanını alır. |
|
|  | [getEndTime()](#getEndTime--) | Aramanın bitiş zamanını alır. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Aramanın süresini saniye cinsinden alır. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | İndeksle bulunan belgeyi alır. |
|
|  | [iterator()](#iterator--) | Bulunan belgelerin koleksiyonunda dolaşan bir yineleyici döndürür. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Sonucun kesildiğini gösteren bir değeri alır.


**Returns:**
boolean - Sonucun kesildiğini gösteren bir değer.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Sonucu açıklayan uyarıları alır.


**Returns:**
java.lang.String - Sonucu açıklayan uyarılar.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Sonraki parçayı aramak için bir chunk arama token'ı alır.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


İndeksle bulunan belgeyi alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | indeks | int | Bulunan bir belgenin indeksi. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Bulunan belgelerin koleksiyonunda dolaşan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Bulunan belgelerin koleksiyonunda yineleme yapmak için kullanılabilecek bir yineleyici.

