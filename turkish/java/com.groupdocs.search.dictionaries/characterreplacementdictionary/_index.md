---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme sürecinde kullanılan karakter değiştirme sözlüğünün arayüzünü tanımlar."
type: docs
weight: 16
url: /tr/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Dizinleme sürecinde kullanılan bir karakter değiştirme sözlüğünün arayüzünü tanımlar. Karakter değiştirme, örneğin aksanlı karakterlerden aksanları kaldırmak veya büyük/küçük harfe duyarsız bir indeks oluşturmak için kullanılabilir.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | Bu  CharacterReplacementDictionary  içinde bulunan karakter sayısını alır. |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Belirtilen karakter değiştirme koleksiyonunu bu  CharacterReplacementDictionary  örneğine ekler. |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Belirtilen karakter değiştirme koleksiyonunu bu  CharacterReplacementDictionary  örneğine ekler. |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Belirtilen karakter değiştirme koleksiyonunu bu  CharacterReplacementDictionary  örneğinden kaldırır. |
|
|  | [contains(char character)](#contains-char-) | Bir  CharacterReplacementDictionary  nesnesinin belirtilen karakter için bir değiştirme içerip içermediğini belirler. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Belirtilen karakter için bir değiştirme alır. |
|
|  | [clear()](#clear--) | Bir  CharacterReplacementDictionary  nesnesinden tüm karakter değiştirmeleri kaldırır. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Bu  CharacterReplacementDictionary  içinde bulunan karakter sayısını alır.


**Returns:**
int - Sözlükteki karakter sayısı.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Belirtilen karakter değiştirme koleksiyonunu bu  CharacterReplacementDictionary  örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | Sözlüğe eklemek için karakter değiştirme koleksiyonu. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Belirtilen karakter değiştirme koleksiyonunu bu  CharacterReplacementDictionary  örneğine ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | Sözlüğe eklemek için karakter değiştirme koleksiyonu. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Belirtilen karakter değiştirme koleksiyonunu bu  CharacterReplacementDictionary  örneğinden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | karakterler | char[] | Kaldırılacak karakterlerin koleksiyonu. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Bir  CharacterReplacementDictionary  nesnesinin belirtilen karakter için bir değiştirme içerip içermediğini belirler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | karakter | char | CharacterReplacementDictionary nesnesinde bulunacak karakter. |
|

**Returns:**
boolean -  true  eğer CharacterReplacementDictionary nesnesi belirtilen karakteri içeriyorsa; aksi takdirde,  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Belirtilen karakter için bir değiştirme alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | karakter | char | Değiştirmesi alınacak karakter. |
|

**Returns:**
char - Belirtilen karakterin değişimi.

### clear() {#clear--}
```
public abstract void clear()
```


Bir  CharacterReplacementDictionary  nesnesinden tüm karakter değiştirmeleri kaldırır.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.Character> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

