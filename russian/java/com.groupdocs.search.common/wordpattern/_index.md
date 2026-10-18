---
title: "WordPattern"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет шаблон слова, используемый в поиске с подстановочными символами."
type: docs
weight: 34
url: /ru/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

Представляет шаблон слова, используемый в поиске с подстановочными символами.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | Инициализирует новый экземпляр класса WordPattern. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | Добавляет строку к шаблону слова. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | Добавляет символ к шаблону слова. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | Добавляет подстановочный символ из одного символа к шаблону слова. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | Добавляет подстановочный символ из нуля или одного символа к шаблону слова. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | Добавляет подстановочный символ из нуля или более символов к шаблону слова. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | Добавляет подстановочный символ из одного или более символов к шаблону слова. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | Добавляет подстановочный символ к шаблону слова. |
|
|  | [toString()](#toString--) | Возвращает объект  System.String  который представляет текущий  WordPattern . |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


Инициализирует новый экземпляр класса WordPattern.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


Добавляет строку к шаблону слова.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | текст | java.lang.String | Строка для добавления. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


Добавляет символ к шаблону слова.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | символ | char | Символ для добавления. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


Добавляет подстановочный символ из одного символа к шаблону слова.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


Добавляет подстановочный символ из нуля или одного символа к шаблону слова.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


Добавляет подстановочный символ из нуля или более символов к шаблону слова.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


Добавляет подстановочный символ из одного или более символов к шаблону слова.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


Добавляет подстановочный символ к шаблону слова.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | мин | int | Минимальное количество символов. |
|
|  | макс | int | Максимальное количество символов. |
|

### toString() {#toString--}
```
public String toString()
```


Возвращает объект  System.String  который представляет текущий  WordPattern .


**Returns:**
java.lang.String - Объект  System.String  который представляет текущий  WordPattern .

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
