---
title: "HighlightOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для подсветки найденных терминов."
type: docs
weight: 22
url: /ru/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Предоставляет параметры для подсветки найденных терминов.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Инициализирует новый экземпляр класса HighlightOptions. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Инициализирует новый экземпляр класса TextOptions. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Получает максимальное количество слов в фрагменте текста перед выделенным словом. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Устанавливает максимальное количество слов в фрагменте текста перед выделенным словом. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Получает максимальное количество слов в фрагменте текста после выделенного слова. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Устанавливает максимальное количество слов в фрагменте текста после выделенного слова. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Получает максимальное количество слов в фрагменте текста. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Устанавливает максимальное количество слов в фрагменте текста. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Получает значение, указывающее, используются ли встроенные стили для выделения вхождений. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Устанавливает значение, указывающее, используются ли встроенные стили для выделения вхождений. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Получает цвет, используемый для выделения вхождений. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Устанавливает цвет, используемый для выделения вхождений. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Получает начальный тег выделения найденного слова. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Устанавливает начальный тег выделения найденного слова. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Получает конечный тег выделения найденного слова. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Устанавливает конечный тег выделения найденного слова. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Инициализирует новый экземпляр класса HighlightOptions.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Инициализирует новый экземпляр класса TextOptions.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Получает максимальное количество слов в фрагменте текста перед выделенным словом. Значение должно находиться в диапазоне от 0 до 10000. Значение по умолчанию — 7.


**Returns:**
int — Максимальное количество слов в фрагменте текста перед выделенным словом.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Устанавливает максимальное количество слов в фрагменте текста перед выделенным словом. Значение должно находиться в диапазоне от 0 до 10000. Значение по умолчанию — 7.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество слов в фрагменте текста перед выделенным словом. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Получает максимальное количество слов в фрагменте текста после выделенного слова. Значение должно находиться в диапазоне от 0 до 10000. Значение по умолчанию — 7.


**Returns:**
int — Максимальное количество слов в фрагменте текста после выделенного слова.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Устанавливает максимальное количество слов в фрагменте текста после выделенного слова. Значение должно находиться в диапазоне от 0 до 10000. Значение по умолчанию — 7.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество слов в фрагменте текста после выделенного слова. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Получает максимальное количество слов в фрагменте текста. Значение должно находиться в диапазоне от 0 до 10000. Значение по умолчанию — 21.


**Returns:**
int — Максимальное количество слов в фрагменте текста.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Устанавливает максимальное количество слов в фрагменте текста. Значение должно находиться в диапазоне от 0 до 10000. Значение по умолчанию — 21.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество слов в фрагменте текста. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Получает значение, указывающее, используются ли встроенные стили для выделения вхождений. Значение по умолчанию — true.


**Returns:**
boolean — Значение, указывающее, используются ли встроенные стили для выделения вхождений.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Устанавливает значение, указывающее, используются ли встроенные стили для выделения вхождений. Значение по умолчанию — true.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, используются ли встроенные стили для выделения вхождений. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Получает цвет, используемый для выделения вхождений. Значение по умолчанию — #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Устанавливает цвет, используемый для выделения вхождений. Значение по умолчанию — #FFD800.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Цвет, который используется для выделения вхождений. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Получает начальный тег выделения найденного слова. Этот тег используется только при выделении в обычном тексте. Значение по умолчанию — пустая строка.


**Returns:**
java.lang.String - Начальный тег выделения найденного слова.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Устанавливает начальный тег выделения найденного слова. Этот тег используется только при выделении в обычном тексте. Значение по умолчанию — пустая строка.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Начальный тег выделения найденного слова. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Получает конечный тег выделения найденного слова. Этот тег используется только при выделении в обычном тексте. Значение по умолчанию — пустая строка.


**Returns:**
java.lang.String - Конечный тег выделения найденного слова.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Устанавливает конечный тег выделения найденного слова. Этот тег используется только при выделении в обычном тексте. Значение по умолчанию — пустая строка.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Конечный тег выделения найденного слова. |
|

