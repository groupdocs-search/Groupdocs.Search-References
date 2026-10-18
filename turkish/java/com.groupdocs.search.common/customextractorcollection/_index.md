---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Özel çıkarıcıların bir koleksiyonunu içerir."
type: docs
weight: 13
url: /tr/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Özel çıkarıcıların bir koleksiyonunu içerir. Koleksiyon, yerleşik çıkarıcılar tarafından kapsanan bir dosya uzantısı için bir çıkarıcı içeriyorsa, bu çıkarıcı yerleşik olanın yerine kullanılacaktır.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [size()](#size--) | Koleksiyonda bulunan çıkarıcı sayısını alır. |
|
|  | [isReadOnly()](#isReadOnly--) | Koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır. |
|
|  | [iterator()](#iterator--) | Bu koleksiyon için bir yineleyici döndürür. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Koleksiyona bir çıkarıcı ekler. |
|
|  | [clear()](#clear--) | Koleksiyondaki tüm çıkarıcıları kaldırır. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Koleksiyonun belirli bir çıkarıcı içerip içermediğini belirler. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Koleksiyonun öğelerini belirli bir dizi indeksinden başlayarak bir diziye kopyalar. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Koleksiyondan bir çıkarıcı kaldırır. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Koleksiyonda bulunan çıkarıcı sayısını alır.


**Returns:**
int - Koleksiyonda bulunan çıkarıcı sayısı.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır.


**Returns:**
boolean - Koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Bu koleksiyon için bir yineleyici döndürür.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici nesnesi.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Koleksiyona bir çıkarıcı ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Koleksiyona eklenecek çıkarıcı. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Koleksiyondaki tüm çıkarıcıları kaldırır.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Koleksiyonun belirli bir çıkarıcı içerip içermediğini belirler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Koleksiyonda bulunacak çıkarıcı. |
|

**Returns:**
boolean -  true  eğer öğe koleksiyonda bulunursa; aksi takdirde,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Koleksiyonun öğelerini belirli bir dizi indeksinden başlayarak bir diziye kopyalar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | Koleksiyondan kopyalanan öğelerin hedefi olan tek boyutlu dizi. Dizi sıfır tabanlı indekslemeye sahip olmalıdır. |
|
|  | arrayIndex | int | Kopyalamanın başladığı dizideki sıfır tabanlı indeks. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Koleksiyondan bir çıkarıcı kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Koleksiyondan kaldırılacak çıkarıcı. |
|

**Returns:**
boolean -  true  eğer çıkarıcı koleksiyondan başarıyla kaldırıldıysa; aksi takdirde,  false . Bu yöntem ayrıca çıkarıcı orijinal koleksiyonda bulunamazsa  false  döndürür.

