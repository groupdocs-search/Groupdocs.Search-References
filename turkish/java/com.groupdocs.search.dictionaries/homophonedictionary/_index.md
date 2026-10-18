---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Heterografik homofonlar sözlüğünün arabirimini tanımlar."
type: docs
weight: 18
url: /tr/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Heterografik homofonlar sözlüğünün arabirimini tanımlar.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | Bu HomophoneDictionary içinde bulunan kelime sayısını alır. |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Belirtilen homofon grupları koleksiyonunu bu HomophoneDictionary örneğine ekler. |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Belirtilen homofon grupları koleksiyonunu bu HomophoneDictionary örneğine ekler. |
|
|  | [clear()](#clear--) | Bir HomophoneDictionary nesnesinden tüm kelimeleri kaldırır. |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Belirtilen kelime için homofonları alır. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Belirtilen kelimenin ait olduğu tüm homofon gruplarını alır. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Bu sözlükte bulunan tüm homofon gruplarını alır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Bu HomophoneDictionary içinde bulunan kelime sayısını alır.


**Returns:**
int - Kelime sayısı.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Belirtilen homofon grupları koleksiyonunu bu HomophoneDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | homofonlar | java.lang.Iterable<java.lang.String[]> | Sözlüğe eklemek için homofon grup koleksiyonu. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Belirtilen homofon grupları koleksiyonunu bu HomophoneDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | homofonlar | java.lang.String[][] | Sözlüğe eklemek için homofon grup koleksiyonu. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Bir HomophoneDictionary nesnesinden tüm kelimeleri kaldırır.


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Belirtilen kelime için homofonları alır. Oluşan dizi orijinal kelimeyi içermez.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelime | java.lang.String | Homofonları önermek için kelime. |
|

**Returns:**
java.lang.String[] - Belirtilen kelime için homofonlar veya HomophoneDictionary nesnesi belirtilen kelimeyi içermiyorsa boş dizi.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Belirtilen kelimenin ait olduğu tüm homofon gruplarını alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelime | java.lang.String | Homofon gruplarını almak için kelime. |
|

**Returns:**
java.lang.String[][] - Belirtilen kelimenin ait olduğu tüm homofon grupları.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Bu sözlükte bulunan tüm homofon gruplarını alır.


**Returns:**
java.lang.String[][] - Tüm homofon grupları.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.String> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

