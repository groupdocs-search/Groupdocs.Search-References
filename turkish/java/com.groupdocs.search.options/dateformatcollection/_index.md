---
title: "DateFormatCollection"
second_title: "GroupDocs.Search for Java API Referansı"
description: "DateFormat nesnelerinin bir koleksiyonunu temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

DateFormat nesnelerinin bir koleksiyonunu temsil eder.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Koleksiyona bir tarih formatı nesnesi ekler. |
|
|  | [clear()](#clear--) | Koleksiyondaki tüm öğeleri kaldırır. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Koleksiyonun belirli bir öğeyi içerip içermediğini belirler. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Koleksiyonun öğelerini belirli bir Array dizininden başlayarak bir Array'e kopyalar. |
|
|  | [size()](#size--) | Koleksiyonda bulunan öğe sayısını alır. |
|
|  | [isReadOnly()](#isReadOnly--) | Koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Koleksiyondan belirli bir öğenin ilk oluşumunu kaldırır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir enumerator döndürür. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Koleksiyona bir tarih formatı nesnesi ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Koleksiyona eklenecek tarih formatı nesnesi. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Koleksiyondaki tüm öğeleri kaldırır.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Koleksiyonun belirli bir öğeyi içerip içermediğini belirler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Koleksiyonda bulunacak öğe. |
|

**Returns:**
boolean - öğe koleksiyonda bulunursa true; aksi takdirde false.

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Koleksiyonun öğelerini belirli bir Array dizininden başlayarak bir Array'e kopyalar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | Koleksiyondan kopyalanan öğelerin hedefi olan tek boyutlu Array. |
|
|  | arrayIndex | int | Kopyalamanın başladığı dizideki sıfır tabanlı indeks. |
|

### size() {#size--}
```
public abstract int size()
```


Koleksiyonda bulunan öğe sayısını alır.


**Returns:**
int - Koleksiyonda bulunan öğe sayısı.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır.


**Returns:**
boolean -  true  koleksiyon yalnızca okunabilir ise; aksi takdirde,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Koleksiyondan belirli bir öğenin ilk oluşumunu kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | Koleksiyondan kaldırılacak öğe. |
|

**Returns:**
boolean -  true  öğe koleksiyondan başarıyla kaldırıldıysa; aksi takdirde,  false . Bu yöntem ayrıca öğe koleksiyonda bulunamazsa  false  döndürür.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Koleksiyon içinde yineleme yapan bir enumerator döndürür.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - Koleksiyon içinde yineleme yapmak için kullanılabilen bir yineleyici.

