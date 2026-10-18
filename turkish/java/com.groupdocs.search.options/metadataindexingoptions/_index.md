---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Meta veri alanlarını indeksleme için seçenekler sağlar."
type: docs
weight: 29
url: /tr/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Meta veri alanlarını indeksleme için seçenekler sağlar.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Boş alan değerlerinin indekslenip indekslenmeyeceğini gösteren bir değeri alır. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Boş alan değerlerinin indekslenip indekslenmeyeceğini gösteren bir değeri ayarlar. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Boş alan adlarını indeksleyip indekslemeyeceğini gösteren bir değeri alır. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Boş alan adlarını indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Boş alan adlarını indekslemek için kullanılan varsayılan alan adını alır. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Boş alan adlarını indekslemek için kullanılan varsayılan alan adını ayarlar. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Bir alanın birleşik adındaki ayırıcıyı alır. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Bir alanın birleşik adındaki ayırıcıyı ayarlar. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Alanı indekslemek için byte türündeki bir dizideki maksimum değer sayısını alır. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Alanı indekslemek için byte türündeki bir dizideki maksimum değer sayısını ayarlar. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Alanı indekslemek için int türündeki bir dizideki maksimum değer sayısını alır. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Alanı indekslemek için int türündeki bir dizideki maksimum değer sayısını ayarlar. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Alanı indekslemek için long türündeki bir dizideki maksimum değer sayısını alır. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Alanı indekslemek için long türündeki bir dizideki maksimum değer sayısını ayarlar. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Alanı indekslemek için double türündeki bir dizideki maksimum değer sayısını alır. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Alanı indekslemek için double türündeki bir dizideki maksimum değer sayısını ayarlar. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Dizi türündeki bir alandaki değerler arasındaki ayırıcıyı alır. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Dizi türündeki bir alandaki değerler arasındaki ayırıcıyı ayarlar. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Boş alan değerlerini indeksleyip indekslemeyeceğini gösteren bir değeri alır. Varsayılan değer true.


**Returns:**
boolean - Boş alan değerlerini indeksleyip indekslemeyeceğini gösteren bir değer.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Boş alan değerlerini indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. Varsayılan değer true.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Boş alan değerlerini indeksleyip indekslemeyeceğini gösteren bir değer. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Boş alan adlarını indeksleyip indekslemeyeceğini gösteren bir değeri alır. Varsayılan değer true.


**Returns:**
boolean - Boş alan adlarını indeksleyip indekslemeyeceğini gösteren bir değer.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Boş alan adlarını indeksleyip indekslemeyeceğini gösteren bir değeri ayarlar. Varsayılan değer true.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | boolean | Boş alan adlarını indeksleyip indekslemeyeceğini gösteren bir değer. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Boş alan adlarını indekslemek için kullanılan varsayılan alan adını alır. Varsayılan değer "unknown".


**Returns:**
java.lang.String - Boş alan adlarını indekslemek için kullanılan varsayılan alan adı.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Boş alan adlarını indekslemek için kullanılan varsayılan alan adını ayarlar. Varsayılan değer \"unknown\" .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Boş alan adlarını indekslemek için kullanılan varsayılan alan adı. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Bir alanın birleşik adındaki ayırıcıyı alır. Varsayılan değer \".\" .


**Returns:**
java.lang.String - Bir alanın birleşik adındaki ayırıcı.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Bir alanın birleşik adındaki ayırıcıyı ayarlar. Varsayılan değer \".\" .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Bir alanın birleşik adındaki ayırıcı. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Alanı indekslemek için byte türündeki bir dizideki maksimum değer sayısını alır. Varsayılan değer Integer.MAX_VALUE .


**Returns:**
int - Alanı indekslemek için byte türündeki bir dizideki maksimum değer sayısı.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Alanı indekslemek için byte türündeki bir dizideki maksimum değer sayısını ayarlar. Varsayılan değer Integer.MAX_VALUE .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Alanı indekslemek için byte türündeki bir dizideki maksimum değer sayısı. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Alanı indekslemek için int türündeki bir dizideki maksimum değer sayısını alır. Varsayılan değer Integer.MAX_VALUE .


**Returns:**
int - Alanı indekslemek için int türündeki bir dizideki maksimum değer sayısı.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Alanı indekslemek için int türündeki bir dizideki maksimum değer sayısını ayarlar. Varsayılan değer Integer.MAX_VALUE .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Alanı indekslemek için int türündeki bir dizideki maksimum değer sayısı. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Alanı indekslemek için long türündeki bir dizideki maksimum değer sayısını alır. Varsayılan değer Integer.MAX_VALUE .


**Returns:**
int - Alanı indekslemek için long türündeki bir dizideki maksimum değer sayısı.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Alanı indekslemek için long türündeki bir dizideki maksimum değer sayısını ayarlar. Varsayılan değer Integer.MAX_VALUE .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Alanı indekslemek için long türündeki bir dizideki maksimum değer sayısı. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Alanı indekslemek için double türündeki bir dizideki maksimum değer sayısını alır. Varsayılan değer Integer.MAX_VALUE .


**Returns:**
int - Alanı indekslemek için double türündeki bir dizideki maksimum değer sayısı.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Alanı indekslemek için double türündeki bir dizideki maksimum değer sayısını ayarlar. Varsayılan değer Integer.MAX_VALUE .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Alanı indekslemek için double türündeki bir dizideki maksimum değer sayısı. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Bir dizi türündeki alandaki değerler arasındaki ayırıcıyı alır. Varsayılan değer boşluk işaretidir.


**Returns:**
java.lang.String - Bir dizi türündeki alandaki değerler arasındaki ayırıcı.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Bir dizi tipindeki alandaki değerler arasındaki ayırıcıyı ayarlar. Varsayılan değer boşluk işaretidir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String | Bir dizi tipindeki alandaki değerler arasındaki ayırıcı. |
|

