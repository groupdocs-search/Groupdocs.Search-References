---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для индексирования полей метаданных."
type: docs
weight: 29
url: /ru/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

Предоставляет параметры для индексирования полей метаданных.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Получает значение, указывающее, индексировать ли пустые значения полей или нет. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Устанавливает значение, указывающее, индексировать ли пустые значения полей или нет. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Получает значение, указывающее, индексировать ли пустые имена полей или нет. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Устанавливает значение, указывающее, индексировать ли пустые имена полей или нет. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | Получает имя поля по умолчанию, используемое для индексации пустых имён полей. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Устанавливает имя поля по умолчанию, используемое для индексации пустых имён полей. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Получает разделитель в составном имени поля. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Устанавливает разделитель в составном имени поля. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Получает максимальное количество значений в массиве типа byte для индексации поля. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Устанавливает максимальное количество значений в массиве типа byte для индексации поля. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Получает максимальное количество значений в массиве типа int для индексации поля. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Устанавливает максимальное количество значений в массиве типа int для индексации поля. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Получает максимальное количество значений в массиве типа long для индексации поля. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Устанавливает максимальное количество значений в массиве типа long для индексации поля. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Получает максимальное количество значений в массиве типа double для индексации поля. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Устанавливает максимальное количество значений в массиве типа double для индексации поля. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Получает разделитель между значениями в поле типа массив. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Устанавливает разделитель между значениями в поле типа массив. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


Получает значение, указывающее, индексировать ли пустые значения полей или нет. Значение по умолчанию —  true .


**Returns:**
boolean - Значение, указывающее, индексировать ли пустые значения полей или нет.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


Устанавливает значение, указывающее, следует ли индексировать пустые значения полей, или нет. Значение по умолчанию — true.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли индексировать пустые значения полей, или нет. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


Получает значение, указывающее, следует ли индексировать пустые имена полей, или нет. Значение по умолчанию — true.


**Returns:**
boolean — Значение, указывающее, следует ли индексировать пустые имена полей, или нет.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


Устанавливает значение, указывающее, следует ли индексировать пустые имена полей, или нет. Значение по умолчанию — true.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, следует ли индексировать пустые имена полей, или нет. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


Получает имя поля по умолчанию, используемое для индексирования пустых имен полей. Значение по умолчанию — "unknown".


**Returns:**
java.lang.String — Имя поля по умолчанию, используемое для индексирования пустых имен полей.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


Устанавливает имя поля по умолчанию, используемое для индексирования пустых имен полей. Значение по умолчанию — "unknown".


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Имя поля по умолчанию, используемое для индексирования пустых имен полей. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


Получает разделитель в составном имени поля. Значение по умолчанию — ".".


**Returns:**
java.lang.String — Разделитель в составном имени поля.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


Устанавливает разделитель в составном имени поля. Значение по умолчанию — ".".


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Разделитель в составном имени поля. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


Получает максимальное количество значений в массиве типа byte для индексирования поля. Значение по умолчанию — Integer.MAX_VALUE.


**Returns:**
int — Максимальное количество значений в массиве типа byte для индексирования поля.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


Устанавливает максимальное количество значений в массиве типа byte для индексирования поля. Значение по умолчанию — Integer.MAX_VALUE.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество значений в массиве типа byte для индексирования поля. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


Получает максимальное количество значений в массиве типа int для индексирования поля. Значение по умолчанию — Integer.MAX_VALUE.


**Returns:**
int — Максимальное количество значений в массиве типа int для индексирования поля.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


Устанавливает максимальное количество значений в массиве типа int для индексирования поля. Значение по умолчанию — Integer.MAX_VALUE.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество значений в массиве типа int для индексирования поля. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


Получает максимальное количество значений в массиве типа long для индексирования поля. Значение по умолчанию — Integer.MAX_VALUE.


**Returns:**
int — Максимальное количество значений в массиве типа long для индексирования поля.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


Устанавливает максимальное количество значений в массиве типа long для индексирования поля. Значение по умолчанию — Integer.MAX_VALUE.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество значений в массиве типа long для индексации поля. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


Получает максимальное количество значений в массиве типа double для индексации поля. Значение по умолчанию — Integer.MAX_VALUE.


**Returns:**
int — Максимальное количество значений в массиве типа double для индексации поля.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


Устанавливает максимальное количество значений в массиве типа double для индексации поля. Значение по умолчанию — Integer.MAX_VALUE.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество значений в массиве типа double для индексации поля. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


Получает разделитель между значениями в поле типа массив. Значение по умолчанию — пробел.


**Returns:**
java.lang.String — Разделитель между значениями в поле типа массив.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


Устанавливает разделитель между значениями в поле типа массив. Значение по умолчанию — пробел.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Разделитель между значениями в поле типа массив. |
|

