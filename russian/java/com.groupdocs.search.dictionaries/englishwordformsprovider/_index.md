---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет поставщик форм английских слов."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

Представляет поставщик форм английских слов.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | Инициализирует новый экземпляр |
EnglishWordFormsProvider
класс.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | Получает формы слова для указанного слова. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


Инициализирует новый экземпляр
EnglishWordFormsProvider
класс.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


Получает формы слова для указанного слова.
Полученный массив не содержит исходное слово.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | слово | java.lang.String | Слово для предложения форм слова. |
|

**Returns:**
java.lang.String[] - Формы слова для указанного слова или пустой массив, если  IWordFormsProvider  не предоставляет формы слова для указанного слова.

