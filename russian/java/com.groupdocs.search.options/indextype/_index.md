---
title: "IndexType"
second_title: "GroupDocs.Search для Java API Reference"
description: "Указывает тип индекса."
type: docs
weight: 49
url: /ru/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Указывает тип индекса.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | Описание |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Обычный индекс с метаданными документов и их содержимым, поддерживающий все функции поиска. |
|
|  | [MetadataIndex](#MetadataIndex) | Индекс, содержащий только метаданные документов, без содержимого. |
|
|  | [CompactIndex](#CompactIndex) | Тип индекса, который занимает значительно меньше места на диске, но не поддерживает поиск по фразам и поиск по диапазону дат. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Обычный индекс с метаданными документов и их содержимым, поддерживающий все функции поиска.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Индекс, содержащий только метаданные документов, без содержимого.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Тип индекса, который занимает значительно меньше места на диске, но не поддерживает поиск по фразам и поиск по диапазону дат.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
