---
title: "AliasDictionary"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Takma ad sözlüğünün arayüzünü tanımlar."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Takma ad sözlüğünün arayüzünü tanımlar.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | AliasDictionary içinde bulunan takma adların sayısını alır. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Belirtilen alias/değiştirme çiftleri koleksiyonunu bu AliasDictionary örneğine ekler. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Belirtilen alias/değiştirme çiftleri koleksiyonunu bu AliasDictionary örneğine ekler. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Belirtilen alias ve ilişkili metin çiftini bu AliasDictionary örneğine ekler. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Belirtilen alias'ı bir AliasDictionary nesnesinden kaldırır. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Bir AliasDictionary nesnesinin belirtilen alias'ı içerip içermediğini belirler. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Belirtilen alias ile ilişkili bir metni alır. |
|
|  | [clear()](#clear--) | Bir AliasDictionary nesnesinden tüm alias'ları kaldırır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


AliasDictionary içinde bulunan takma adların sayısını alır.


**Returns:**
int - AliasDictionary içinde bulunan alias sayısı.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Belirtilen alias/değiştirme çiftleri koleksiyonunu bu AliasDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | çiftler | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | Sözlüğe eklenecek alias/değiştirme çiftleri koleksiyonu. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Belirtilen alias/değiştirme çiftleri koleksiyonunu bu AliasDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | Sözlüğe eklenecek alias/değiştirme çiftleri koleksiyonu. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Belirtilen alias ve ilişkili metin çiftini bu AliasDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alias | java.lang.String | Sözlüğe eklenecek alias. |
|
|  | metin | java.lang.String | Alias ile ilişkilendirilecek metin. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Belirtilen alias'ı bir AliasDictionary nesnesinden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alias | java.lang.String | Kaldırılacak alias. |
|

**Returns:**
boolean - Bu yöntem, alias başarıyla bulunup kaldırılırsa true döndürür. AliasDictionary nesnesinde alias bulunamazsa false döndürür.

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Bir AliasDictionary nesnesinin belirtilen alias'ı içerip içermediğini belirler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alias | java.lang.String | AliasDictionary nesnesinde bulunacak alias. |
|

**Returns:**
boolean - AliasDictionary nesnesi belirtilen alias'ı içeriyorsa true; aksi takdirde false.

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Belirtilen alias ile ilişkili bir metni alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | alias | java.lang.String | AliasDictionary nesnesinde bulunacak alias. |
|

**Returns:**
java.lang.String - Belirtilen alias ile ilişkili bir metin veya null.

### clear() {#clear--}
```
public abstract void clear()
```


Bir AliasDictionary nesnesinden tüm alias'ları kaldırır.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.String> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

