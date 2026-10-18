---
title: "StopWordDictionary"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Durdurma kelimeleri sözlüğünün arabirimini tanımlar."
type: docs
weight: 22
url: /tr/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Durdurma kelimeleri sözlüğünün arabirimini tanımlar.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | StopWordDictionary içinde bulunan durdurma kelimelerinin sayısını alır. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğine ekler. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğine ekler. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğinden kaldırır. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğinden kaldırır. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Bir StopWordDictionary nesnesinin belirtilen kelimeyi içerip içermediğini belirler. |
|
|  | [clear()](#clear--) | Bir StopWordDictionary nesnesinden tüm kelimeleri kaldırır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


StopWordDictionary içinde bulunan durdurma kelimelerinin sayısını alır.


**Returns:**
int - Sözlükteki durdurma kelimelerinin sayısı.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelimeler | java.lang.Iterable<java.lang.String> | Sözlüğe eklemek için kelime koleksiyonu. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelimeler | java.lang.String[] | Sözlüğe eklemek için kelime koleksiyonu. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğinden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelimeler | java.lang.Iterable<java.lang.String> | Kaldırılacak kelime koleksiyonu. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Belirtilen kelime koleksiyonunu bu StopWordDictionary örneğinden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelimeler | java.lang.String[] | Kaldırılacak kelime koleksiyonu. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Bir StopWordDictionary nesnesinin belirtilen kelimeyi içerip içermediğini belirler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelime | java.lang.String | StopWordDictionary nesnesinde bulunacak kelime. |
|

**Returns:**
boolean - belirtilen kelimeyi StopWordDictionary nesnesi içeriyorsa true; aksi takdirde false.

### clear() {#clear--}
```
public abstract void clear()
```


Bir StopWordDictionary nesnesinden tüm kelimeleri kaldırır.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.String> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

