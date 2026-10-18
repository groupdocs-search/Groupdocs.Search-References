---
title: "SearchResult"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili hasil pencarian yang cocok dengan kueri pencarian."
type: docs
weight: 19
url: /id/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Mewakili hasil pencarian yang cocok dengan kueri pencarian.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Membuat sebuah indeks
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentFolder);
// Mengatur opsi pencarian
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Mengaktifkan pencarian fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Mengatur jumlah maksimum perbedaan menjadi 3
// Cari dokumen yang berisi kata 'Einstein' atau frasa 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Mencetak hasil
System.out.println("Documents: " + result.getDocumentCount());
System.out.println("Total occurrences: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocument: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOccurrences: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tField: " + field.getFieldName());
System.out.println("\t\tOccurrences: " + document.getOccurrenceCount());
// Mencetak istilah yang ditemukan
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Mencetak frasa yang ditemukan
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


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Mendapatkan jumlah dokumen yang ditemukan. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Mendapatkan total jumlah kemunculan yang ditemukan. |
|
|  | [getTruncated()](#getTruncated--) | Mendapatkan nilai yang menunjukkan bahwa hasil dipotong. |
|
|  | [getWarnings()](#getWarnings--) | Mendapatkan peringatan yang menjelaskan hasil. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Mendapatkan token pencarian chunk untuk mencari chunk berikutnya. |
|
|  | [getStartTime()](#getStartTime--) | Mendapatkan waktu mulai pencarian. |
|
|  | [getEndTime()](#getEndTime--) | Mendapatkan waktu akhir pencarian. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Mendapatkan durasi pencarian dalam detik. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Mendapatkan dokumen yang ditemukan berdasarkan indeks. |
|
|  | [iterator()](#iterator--) | Mengembalikan iterator yang mengiterasi koleksi dokumen yang ditemukan. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Mendapatkan jumlah dokumen yang ditemukan.


**Returns:**
int - Jumlah dokumen yang ditemukan.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Mendapatkan total jumlah kemunculan yang ditemukan.


**Returns:**
int - Total jumlah kemunculan yang ditemukan.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Mendapatkan nilai yang menunjukkan bahwa hasil dipotong.


**Returns:**
boolean - Nilai yang menunjukkan bahwa hasil dipotong.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Mendapatkan peringatan yang menjelaskan hasil.


**Returns:**
java.lang.String - Peringatan yang menjelaskan hasil.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Mendapatkan token pencarian chunk untuk mencari chunk berikutnya.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Mendapatkan waktu mulai pencarian.


**Returns:**
java.util.Date - Waktu mulai pencarian.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Mendapatkan waktu akhir pencarian.


**Returns:**
java.util.Date - Waktu akhir pencarian.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Mendapatkan durasi pencarian dalam detik.


**Returns:**
double - Durasi pencarian dalam detik.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Mendapatkan dokumen yang ditemukan berdasarkan indeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | indeks | int | Indeks dokumen yang ditemukan. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Mengembalikan iterator yang mengiterasi koleksi dokumen yang ditemukan.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Iterator yang dapat digunakan untuk mengiterasi koleksi dokumen yang ditemukan.

