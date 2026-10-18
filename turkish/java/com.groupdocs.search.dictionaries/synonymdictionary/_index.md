---
title: "SynonymDictionary"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Eşanlamlılar sözlüğünün arabirimini tanımlar."
type: docs
weight: 23
url: /tr/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Eşanlamlılar sözlüğünün arabirimini tanımlar.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | Bu SynonymDictionary içinde bulunan kelime sayısını alır. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Belirtilen eşanlamlı grup koleksiyonunu bu SynonymDictionary örneğine ekler. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Belirtilen eşanlamlı grup koleksiyonunu bu SynonymDictionary örneğine ekler. |
|
|  | [clear()](#clear--) | Bu SynonymDictionary nesnesinden tüm kelimeleri kaldırır. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Belirtilen kelime için eşanlamlıları alır. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Belirtilen kelimenin ait olduğu tüm eşanlamlı grup kümelerini alır. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Bu sözlükte bulunan tüm eşanlamlı grup kümelerini alır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Bu SynonymDictionary içinde bulunan kelime sayısını alır.


**Returns:**
int - Bu SynonymDictionary içinde bulunan kelime sayısı.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Belirtilen eşanlamlı grup koleksiyonunu bu SynonymDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | eşanlamlılar | java.lang.Iterable<java.lang.String[]> | Sözlüğe eklenecek eşanlamlı grup koleksiyonu. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Belirtilen eşanlamlı grup koleksiyonunu bu SynonymDictionary örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | eşanlamlılar | java.lang.String[][] | Sözlüğe eklenecek eşanlamlı grup koleksiyonu. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Bu SynonymDictionary nesnesinden tüm kelimeleri kaldırır.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Belirtilen kelime için eşanlamlıları alır. Sonuç dizisi orijinal kelimeyi içermez.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelime | java.lang.String | Eşanlamlıları önermek için kelime. |
|

**Returns:**
java.lang.String[] - Belirtilen kelime için eşanlamlılar veya SynonymDictionary nesnesi belirtilen kelimeyi içermiyorsa boş dizi.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Belirtilen kelimenin ait olduğu tüm eşanlamlı grup kümelerini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelime | java.lang.String | Eşanlamlı grup kümelerini almak için kelime. |
|

**Returns:**
java.lang.String[][] - Belirtilen kelimenin ait olduğu tüm eşanlamlı grup kümeleri.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Bu sözlükte bulunan tüm eşanlamlı grup kümelerini alır.


**Returns:**
java.lang.String[][] - Tüm eşanlamlı grup kümeleri.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.String> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

