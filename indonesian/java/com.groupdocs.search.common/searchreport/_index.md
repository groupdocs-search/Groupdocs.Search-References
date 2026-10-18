---
title: "SearchReport"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili informasi terperinci tentang operasi pencarian."
type: docs
weight: 30
url: /id/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Mewakili informasi terperinci tentang operasi pencarian.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen dari folder yang ditentukan
index.add(documentsFolder);
// Mencari di indeks
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Mendapatkan laporan pencarian
SearchReport[] reports = index.getSearchReports();
// Mencetak laporan ke konsol
for (SearchReport report : reports) {
System.out.println("Kueri: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Waktu: " + df.format(report.getStartTime()));
System.out.println("Durasi: " + report.getSearchDuration());
System.out.println("Dokumen: " + report.getDocumentCount());
System.out.println("Kejadian: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Mendapatkan waktu mulai pencarian. |
|
|  | [getEndTime()](#getEndTime--) | Mendapatkan waktu akhir pencarian. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Mendapatkan durasi pencarian dalam detik. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Mendapatkan jumlah dokumen yang ditemukan. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Mendapatkan total jumlah kemunculan yang ditemukan. |
|
|  | [getTextQuery()](#getTextQuery--) | Mendapatkan kueri pencarian dalam bentuk teks. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Mendapatkan kueri pencarian dalam bentuk objek. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Mendapatkan opsi pencarian. |
|
|  | [toString()](#toString--) | Mengembalikan sebuah String yang mewakili SearchReport saat ini. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Mendapatkan kueri pencarian dalam bentuk teks.


**Returns:**
java.lang.String - Kuery pencarian dalam bentuk teks.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Mendapatkan kueri pencarian dalam bentuk objek.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Mendapatkan opsi pencarian.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan sebuah String yang mewakili SearchReport saat ini.


**Returns:**
java.lang.String - Sebuah String yang mewakili SearchReport saat ini.

