---
title: "Алфавит"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет интерфейс словаря символов, используемого при индексации для определения типа символа."
type: docs
weight: 15
url: /ru/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Определяет интерфейс словаря символов, используемого при индексации для определения типа символа. Каждый символ может обрабатываться как разделитель, как буква или как оба.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Получает тип символа. |
|
|  | [getCount()](#getCount--) | Получает количество символов, содержащихся в  Alphabet . |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Устанавливает тип для каждого символа указанной коллекции в данном экземпляре  Alphabet . |
|
|  | [clear()](#clear--) | Устанавливает тип  CharacterType.Separator  для всех символов в этом  Alphabet . |
|
|  | [iterator()](#iterator--) | Возвращает итератор, который проходит по коллекции. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Получает тип символа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | символ | char | Символ для получения типа. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Получает количество символов, содержащихся в  Alphabet .


**Returns:**
int - Количество символов в словаре.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Устанавливает тип для каждого символа указанной коллекции в данном экземпляре  Alphabet .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | символы | char[] | Коллекция символов для установки типа. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Тип символа. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Устанавливает тип  CharacterType.Separator  для всех символов в этом  Alphabet .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Возвращает итератор, который проходит по коллекции.


**Returns:**
java.util.Iterator<java.lang.Character> - Итератор, который можно использовать для перебора элементов коллекции.

