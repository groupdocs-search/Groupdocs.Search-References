---
title: "FoundDocument"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili dokumen yang ditemukan."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Mewakili dokumen yang ditemukan.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Mendapatkan info dokumen. |
|
|  | [getRelevance()](#getRelevance--) | Mendapatkan relevansi hasil pencarian. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Mendapatkan jumlah kemunculan yang ditemukan. |
|
|  | [getFoundFields()](#getFoundFields--) | Mendapatkan bidang dokumen yang ditemukan. |
|
|  | [getTerms()](#getTerms--) | Mendapatkan istilah yang ditemukan. |
|
|  | [getTermSequences()](#getTermSequences--) | Mendapatkan urutan istilah yang ditemukan. |
|
|  | [getAttributes()](#getAttributes--) | Mendapatkan atribut yang terkait dengan dokumen yang ditemukan. |
|
|  | [toString()](#toString--) | Mengembalikan representasi string dari dokumen yang ditemukan. |
|
|  | [serialize()](#serialize--) | Menyerialkan instance saat ini ke dalam array byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Mendeserialkan sebuah instance dari array byte. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Mendapatkan info dokumen.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Mendapatkan relevansi hasil pencarian.


**Returns:**
double - Relevansi hasil pencarian.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Mendapatkan jumlah kemunculan yang ditemukan.


**Returns:**
int - Jumlah kemunculan yang ditemukan.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Mendapatkan bidang dokumen yang ditemukan.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Bidang dokumen yang ditemukan.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Mendapatkan istilah yang ditemukan. Nilai dievaluasi setiap kali properti diakses.


**Returns:**
java.lang.String[] - Istilah yang ditemukan.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Mendapatkan urutan istilah yang ditemukan.


**Returns:**
java.lang.String[][] - Urutan istilah yang ditemukan.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Mendapatkan atribut yang terkait dengan dokumen yang ditemukan. Opsi yang sesuai harus diaktifkan dalam opsi pencarian untuk mengambil atribut.


**Returns:**
java.lang.String[] - Atribut yang terkait dengan dokumen yang ditemukan.

### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan representasi string dari dokumen yang ditemukan.


**Returns:**
java.lang.String - String yang mewakili dokumen yang ditemukan.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Menyerialkan instance saat ini ke dalam array byte.


**Returns:**
byte[] - Array byte yang mewakili instance saat ini.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Mendeserialkan sebuah instance dari array byte.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | array | byte[] | Array byte untuk dideserialkan. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

