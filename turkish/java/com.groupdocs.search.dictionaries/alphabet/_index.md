---
title: "Alfabe"
second_title: "GroupDocs.Search for Java API Referansı"
description: "İndeksleme sırasında karakter tipini tespit etmek için kullanılan karakter sözlüğünün arayüzünü tanımlar."
type: docs
weight: 15
url: /tr/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Dizinleme sırasında karakter tipini tespit etmek için kullanılan karakter sözlüğünün arayüzünü tanımlar. Her karakter ayırıcı, harf ya da her ikisi olarak işlenebilir.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Bir karakterin tipini alır. |
|
|  | [getCount()](#getCount--) | Alfabe içinde bulunan karakter sayısını alır. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Bu Alfabe örneğinde belirtilen koleksiyonun her karakteri için tipi ayarlar. |
|
|  | [clear()](#clear--) | Bu Alfabe içindeki tüm karakterler için  CharacterType.Separator  tipini ayarlar. |
|
|  | [iterator()](#iterator--) | Koleksiyon içinde yineleme yapan bir yineleyici döndürür. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Bir karakterin tipini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | karakter | char | Tipi alınacak karakter. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Alfabe içinde bulunan karakter sayısını alır.


**Returns:**
int - Sözlükteki karakter sayısı.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Bu Alfabe örneğinde belirtilen koleksiyonun her karakteri için tipi ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | karakterler | char[] | Tipi ayarlamak için karakter koleksiyonu. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Karakter tipi. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Bu Alfabe içindeki tüm karakterler için  CharacterType.Separator  tipini ayarlar.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Koleksiyon içinde yineleme yapan bir yineleyici döndürür.


**Returns:**
java.util.Iterator<java.lang.Character> - Koleksiyon içinde yineleme yapmak için kullanılabilecek bir yineleyici.

