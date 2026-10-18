---
title: "SpellingCorrector"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Sorgudaki terimler için bir yazım düzelticisinin arabirimini tanımlar."
type: docs
weight: 21
url: /tr/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Sorgudaki terimler için bir yazım düzelticisinin arabirimini tanımlar.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCount()](#getCount--) | Bu SpellingCorrector içinde bulunan kelime sayısını alır. |
|
|  | [getWords()](#getWords--) | Bu SpellingCorrector içinde şu anda bulunan kelime koleksiyonunu alır. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Bu SpellingCorrector örneğine belirtilen kelime koleksiyonunu ekler. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Bu SpellingCorrector örneğine belirtilen kelime koleksiyonunu ekler. |
|
|  | [clear()](#clear--) | Bir SpellingCorrector nesnesinden tüm kelimeleri kaldırır. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Bu SpellingCorrector içinde bulunan kelime sayısını alır.


**Returns:**
int - Bu SpellingCorrector içinde bulunan kelime sayısı.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Bu SpellingCorrector içinde şu anda bulunan kelime koleksiyonunu alır.


**Returns:**
java.lang.String[] - Kelime koleksiyonu.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Bu SpellingCorrector örneğine belirtilen kelime koleksiyonunu ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelimeler | java.lang.Iterable<java.lang.String> | Sözlüğe eklemek için kelime koleksiyonu. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Bu SpellingCorrector örneğine belirtilen kelime koleksiyonunu ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | kelimeler | java.lang.String[] | Sözlüğe eklemek için kelime koleksiyonu. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Bir SpellingCorrector nesnesinden tüm kelimeleri kaldırır.


