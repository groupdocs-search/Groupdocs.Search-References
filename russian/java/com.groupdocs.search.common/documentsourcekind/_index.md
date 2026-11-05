---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search для Java API Reference"
description: "Определяет типы источников документов."
type: docs
weight: 39
url: /ru/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Определяет типы источников документов.

## Fields

| Field | Описание |
| --- | --- |
|  | [File](#File) | Источник документа из файла. |
|
|  | [Stream](#Stream) | Источник документа из потока. |
|
|  | [Structure](#Structure) | Источник документа из структуры. |
|
|  | [ExtractedData](#ExtractedData) | Источник документа ранее извлечённых данных. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


Источник документа из файла.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


Источник документа из потока.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


Источник документа из структуры.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


Источник документа ранее извлечённых данных.


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
