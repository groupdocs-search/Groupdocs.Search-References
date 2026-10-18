---
title: "DocumentInfo"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет дескриптор проиндексированного документа."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Представляет дескриптор проиндексированного документа.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [toString()](#toString--) | Возвращает  System.String  который представляет текущий  DocumentInfo . |
|
|  | [getFilePath()](#getFilePath--) | Получает путь к файлу, если проиндексировано из файла, или ключ документа, если проиндексировано из потока или структуры. |
|
|  | [getFileType()](#getFileType--) | Получает тип файла. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Получает семейство форматов документа. |
|
|  | [getInnerPath()](#getInnerPath--) | Получает внутренний путь для элемента контейнерного документа. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Получает части внутреннего пути для элемента контейнерного документа. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Получает тип источника документа. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | Получает индикатор ошибки индексации. |
|
|  | [serialize()](#serialize--) | Сериализует текущий экземпляр в массив байтов. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Десериализует экземпляр из массива байтов. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Возвращает  System.String  который представляет текущий  DocumentInfo .


**Returns:**
java.lang.String -  System.String , который представляет текущий  DocumentInfo .

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Получает путь к файлу, если проиндексировано из файла, или ключ документа, если проиндексировано из потока или структуры.


**Returns:**
java.lang.String - Путь к файлу или ключ документа.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Получает тип файла.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Получает семейство форматов документа.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Получает внутренний путь для элемента контейнерного документа.


**Returns:**
java.lang.String - Внутренний путь.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Получает части внутреннего пути для элемента контейнерного документа.


**Returns:**
java.lang.String[] - Части внутреннего пути.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Получает тип источника документа.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


Получает индикатор ошибки индексации.


**Returns:**
boolean - Индикатор ошибки индексации.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Сериализует текущий экземпляр в массив байтов.


**Returns:**
byte[] — массив байтов, представляющий текущий экземпляр.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Десериализует экземпляр из массива байтов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | массив | byte[] | Массив байтов, из которого происходит десериализация. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

