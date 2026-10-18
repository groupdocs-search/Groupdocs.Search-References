---
title: "FoundDocumentField"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili bidang dokumen yang ditemukan."
type: docs
weight: 15
url: /id/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Mewakili bidang dokumen yang ditemukan.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Mendapatkan nama bidang. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Mendapatkan jumlah kemunculan yang ditemukan. |
|
|  | [getTerms()](#getTerms--) | Mendapatkan istilah yang ditemukan. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Mendapatkan kemunculan istilah yang ditemukan. |
|
|  | [getTermSequences()](#getTermSequences--) | Mendapatkan urutan istilah yang ditemukan. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Mendapatkan kemunculan urutan istilah yang ditemukan. |
|
|  | [toString()](#toString--) | Mengembalikan representasi string dari bidang dokumen yang ditemukan. |
|
|  | [serialize()](#serialize--) | Menyerialkan instance saat ini ke dalam array byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Mendeserialkan sebuah instance dari array byte. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Mendapatkan nama bidang.


**Returns:**
java.lang.String - Nama bidang.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Mendapatkan jumlah kemunculan yang ditemukan.


**Returns:**
int - Jumlah kemunculan yang ditemukan.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Mendapatkan istilah yang ditemukan.


**Returns:**
java.lang.String[] - Istilah yang ditemukan.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Mendapatkan kemunculan istilah yang ditemukan.


**Returns:**
int[] - Kemunculan istilah yang ditemukan.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Mendapatkan urutan istilah yang ditemukan.


**Returns:**
java.lang.String[][] - Urutan istilah yang ditemukan.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Mendapatkan kemunculan urutan istilah yang ditemukan.


**Returns:**
int[] - Kemunculan urutan istilah yang ditemukan.

### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan representasi string dari bidang dokumen yang ditemukan.


**Returns:**
java.lang.String - String yang mewakili bidang dokumen yang ditemukan.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Menyerialkan instance saat ini ke dalam array byte.


**Returns:**
byte[] - Array byte yang mewakili instance saat ini.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Mendeserialkan sebuah instance dari array byte.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | array | byte[] | Array byte untuk dideserialkan. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

