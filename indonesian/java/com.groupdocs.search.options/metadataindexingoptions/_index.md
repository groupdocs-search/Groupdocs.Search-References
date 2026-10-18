---
title: "MetadataIndexingOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk mengindeks bidang metadata."
type: docs
weight: 29
url: /id/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Menyediakan opsi untuk mengindeks bidang metadata.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Mendapatkan nilai yang menunjukkan apakah nilai bidang kosong akan diindeks atau tidak. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Mengatur nilai yang menunjukkan apakah nilai bidang kosong akan diindeks atau tidak. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Mendapatkan nilai yang menunjukkan apakah nama bidang kosong akan diindeks atau tidak. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Mengatur nilai yang menunjukkan apakah nama bidang kosong akan diindeks atau tidak. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Mendapatkan nama bidang default yang digunakan untuk mengindeks nama bidang kosong. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Mengatur nama bidang default yang digunakan untuk mengindeks nama bidang kosong. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Mendapatkan pemisah dalam nama gabungan sebuah bidang. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Mengatur pemisah dalam nama gabungan sebuah bidang. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Mendapatkan jumlah maksimum nilai dalam array tipe byte untuk mengindeks bidang. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Mengatur jumlah maksimum nilai dalam array tipe byte untuk mengindeks bidang. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Mendapatkan jumlah maksimum nilai dalam array tipe int untuk mengindeks bidang. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Mengatur jumlah maksimum nilai dalam array tipe int untuk mengindeks bidang. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Mendapatkan jumlah maksimum nilai dalam array tipe long untuk mengindeks bidang. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Mengatur jumlah maksimum nilai dalam array tipe long untuk mengindeks bidang. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Mendapatkan jumlah maksimum nilai dalam array tipe double untuk mengindeks bidang. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Mengatur jumlah maksimum nilai dalam array tipe double untuk mengindeks bidang. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Mendapatkan pemisah antara nilai dalam bidang tipe array. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Mengatur pemisah antara nilai dalam bidang tipe array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Mendapatkan nilai yang menunjukkan apakah nilai bidang kosong akan diindeks atau tidak. Nilai default adalah  true .


**Returns:**
boolean - Nilai yang menunjukkan apakah nilai bidang kosong akan diindeks atau tidak.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan mengindeks nilai bidang kosong atau tidak. Nilai default adalah true.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah akan mengindeks nilai bidang kosong atau tidak. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Mendapatkan nilai yang menunjukkan apakah akan mengindeks nama bidang kosong atau tidak. Nilai default adalah true.


**Returns:**
boolean - Nilai yang menunjukkan apakah akan mengindeks nama bidang kosong atau tidak.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan mengindeks nama bidang kosong atau tidak. Nilai default adalah true.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Nilai yang menunjukkan apakah akan mengindeks nama bidang kosong atau tidak. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Mendapatkan nama bidang default yang digunakan untuk mengindeks nama bidang kosong. Nilai default adalah "unknown".


**Returns:**
java.lang.String - Nama bidang default yang digunakan untuk mengindeks nama bidang kosong.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Mengatur nama bidang default yang digunakan untuk mengindeks nama bidang kosong. Nilai default adalah "unknown".


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Nama bidang default yang digunakan untuk mengindeks nama bidang kosong. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Mendapatkan pemisah dalam nama gabungan sebuah bidang. Nilai default adalah ".".


**Returns:**
java.lang.String - Pemisah dalam nama gabungan sebuah bidang.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Mengatur pemisah dalam nama gabungan sebuah bidang. Nilai default adalah ".".


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Pemisah dalam nama gabungan sebuah bidang. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Mendapatkan jumlah maksimum nilai dalam array tipe byte untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Returns:**
int - Jumlah maksimum nilai dalam array tipe byte untuk mengindeks bidang.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Mengatur jumlah maksimum nilai dalam array tipe byte untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum nilai dalam array tipe byte untuk mengindeks bidang. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Mendapatkan jumlah maksimum nilai dalam array tipe int untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Returns:**
int - Jumlah maksimum nilai dalam array tipe int untuk mengindeks bidang.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Mengatur jumlah maksimum nilai dalam array tipe int untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum nilai dalam array tipe int untuk mengindeks bidang. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Mendapatkan jumlah maksimum nilai dalam array tipe long untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Returns:**
int - Jumlah maksimum nilai dalam array tipe long untuk mengindeks bidang.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Mengatur jumlah maksimum nilai dalam array tipe long untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum nilai dalam array bertipe long untuk mengindeks bidang. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Mendapatkan jumlah maksimum nilai dalam array bertipe double untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Returns:**
int - Jumlah maksimum nilai dalam array bertipe double untuk mengindeks bidang.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Mengatur jumlah maksimum nilai dalam array bertipe double untuk mengindeks bidang. Nilai default adalah Integer.MAX_VALUE.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | int | Jumlah maksimum nilai dalam array bertipe double untuk mengindeks bidang. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Mendapatkan pemisah antara nilai dalam bidang bertipe array. Nilai default adalah tanda spasi.


**Returns:**
java.lang.String - Pemisah antara nilai dalam bidang bertipe array.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Mengatur pemisah antara nilai dalam bidang bertipe array. Nilai default adalah tanda spasi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | java.lang.String | Pemisah antara nilai dalam bidang bertipe array. |
|

