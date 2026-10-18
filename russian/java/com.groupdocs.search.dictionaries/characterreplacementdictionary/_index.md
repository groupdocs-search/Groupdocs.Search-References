---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря замены символов, используемого в процессе индексации."
type: docs
weight: 16
url: /ru/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Определяет интерфейс словаря замены символов, используемого в процессе индексации. Замена символов может использоваться, например, для удаления диакритических знаков с символов с акцентами или для создания нечувствительного к регистру индекса.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCount()](#getCount--) | Возвращает количество символов, содержащихся в этом  CharacterReplacementDictionary . |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Добавляет указанную коллекцию замен символов в этот экземпляр  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Добавляет указанную коллекцию замен символов в этот экземпляр  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Удаляет указанную коллекцию замен символов из этого экземпляра CharacterReplacementDictionary. |
|
|  | [contains(char character)](#contains-char-) | Определяет, содержит ли объект CharacterReplacementDictionary замену для указанного символа. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Получает замену для указанного символа. |
|
|  | [clear()](#clear--) | Удаляет все замены символов из объекта CharacterReplacementDictionary. |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Возвращает количество символов, содержащихся в этом  CharacterReplacementDictionary .


**Returns:**
int - Количество символов в словаре.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Добавляет указанную коллекцию замен символов в этот экземпляр  CharacterReplacementDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | Коллекция замен символов для добавления в словарь. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Добавляет указанную коллекцию замен символов в этот экземпляр  CharacterReplacementDictionary .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | Коллекция замен символов для добавления в словарь. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Удаляет указанную коллекцию замен символов из этого экземпляра CharacterReplacementDictionary.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | символы | char[] | Коллекция символов для удаления. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Определяет, содержит ли объект CharacterReplacementDictionary замену для указанного символа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | символ | char | Символ для поиска в объекте CharacterReplacementDictionary. |
|

**Returns:**
boolean — true, если объект CharacterReplacementDictionary содержит указанный символ; иначе — false.

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Получает замену для указанного символа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | символ | char | Символ, для которого требуется получить замену. |
|

**Returns:**
char — Замена для указанного символа.

### clear() {#clear--}
```
public abstract void clear()
```


Удаляет все замены символов из объекта CharacterReplacementDictionary.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.Character> - Итератор, который можно использовать для перебора элементов коллекции.

