---
title: "IndexingReport"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili informasi terperinci tentang operasi pengindeksan."
type: docs
weight: 25
url: /id/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Mewakili informasi terperinci tentang operasi pengindeksan.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Contoh ini menunjukkan penggunaan tipikal kelas tersebut.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = \"c:\\\\MyDocuments1\\\\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Membuat indeks di folder yang ditentukan
Index index = new Index(indexFolder);
// Mengindeks dokumen
index.add(documentsFolder1);
index.add(documentsFolder2);
// Mendapatkan laporan pengindeksan
IndexingReport[] reports = index.getIndexingReports();
// Mencetak laporan ke konsol
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Waktu: " + df.format(report.getStartTime()));
System.out.println("Durasi: " + report.getIndexingTime());
System.out.println("Total dokumen: " + report.getTotalDocumentsInIndex());
System.out.println("Total istilah: " + report.getTotalTermCount());
System.out.println("Ukuran dokumen terindeks (MB): " + report.getIndexedDocumentsSize());
System.out.println("Ukuran indeks (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Mendapatkan total jumlah dokumen dalam indeks. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Mendapatkan total jumlah istilah dalam indeks. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Mendapatkan total panjang dokumen terindeks dalam MB. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Mendapatkan jumlah segmen indeks. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Mendapatkan total ukuran indeks dalam byte. |
|
|  | [getStartTime()](#getStartTime--) | Mendapatkan waktu mulai pengindeksan. |
|
|  | [getEndTime()](#getEndTime--) | Mendapatkan waktu selesai pengindeksan. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Mendapatkan durasi pengindeksan dalam detik. |
|
|  | [getErrors()](#getErrors--) | Mendapatkan daftar kesalahan. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Mendapatkan daftar dokumen terindeks. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Mendapatkan daftar dokumen yang diperbarui. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Mendapatkan daftar dokumen yang dihapus dari indeks. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Mendapatkan total jumlah dokumen dalam indeks.


**Returns:**
int - Total jumlah dokumen dalam indeks.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Mendapatkan total jumlah istilah dalam indeks.


**Returns:**
int - Total jumlah istilah dalam indeks.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Mendapatkan total panjang dokumen terindeks dalam MB.


**Returns:**
double - Total panjang dokumen terindeks dalam MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Mendapatkan jumlah segmen indeks.


**Returns:**
int - Jumlah segmen indeks.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Mendapatkan total ukuran indeks dalam byte.


**Returns:**
long - Total ukuran indeks dalam byte.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Mendapatkan waktu mulai pengindeksan.


**Returns:**
java.util.Date - Waktu mulai pengindeksan.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Mendapatkan waktu selesai pengindeksan.


**Returns:**
java.util.Date - Waktu selesai pengindeksan.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Mendapatkan durasi pengindeksan dalam detik.


**Returns:**
double - Durasi pengindeksan dalam detik.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Mendapatkan daftar kesalahan.


**Returns:**
java.lang.String[] - Daftar kesalahan.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Mendapatkan daftar dokumen terindeks.


**Returns:**
java.lang.String[] - Daftar dokumen terindeks.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Mendapatkan daftar dokumen yang diperbarui.


**Returns:**
java.lang.String[] - Daftar dokumen yang diperbarui.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Mendapatkan daftar dokumen yang dihapus dari indeks.


**Returns:**
java.lang.String[] - Daftar dokumen yang dihapus dari indeks.

