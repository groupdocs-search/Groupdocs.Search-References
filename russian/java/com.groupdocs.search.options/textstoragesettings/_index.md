---
title: "TextStorageSettings"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет настройки хранения текста."
type: docs
weight: 42
url: /ru/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Представляет настройки хранения текста.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Инициализирует новый экземпляр класса  TextStorageSettings . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getCompression()](#getCompression--) | Получает степень сжатия текстового хранилища. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Устанавливает степень сжатия текстового хранилища. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Инициализирует новый экземпляр класса  TextStorageSettings .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Сжатие текстового хранилища. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Получает степень сжатия текстового хранилища. Значение по умолчанию — Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Устанавливает степень сжатия текстового хранилища. Значение по умолчанию — Compression.Normal.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | Сжатие текстового хранилища. |
|

