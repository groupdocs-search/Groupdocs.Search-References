---
title: "Документ"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет базовый класс для документов, добавляемых в индекс из потока файловой системы или структуры."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Представляет базовый класс для документов, добавляемых в индекс из файловой системы, потока или структуры. Содержит статические методы для создания документов из различных типов источников.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Получает тип источника документа. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Получает ключ документа, используемый для идентификации документа в индексе. |
|
|  | [isLazy()](#isLazy--) | Получает значение, указывающее, загружен ли документ по требованию. |
|
|  | [getModificationDate()](#getModificationDate--) | Получает дату последнего изменения документа. |
|
|  | [getExtension()](#getExtension--) | Получает расширение, используемое для этого типа документа. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Получает дополнительные поля документа. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Устанавливает дополнительные поля документа. |
|
|  | [getAttributes()](#getAttributes--) | Получает атрибуты документа. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Устанавливает атрибуты документа. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Создаёт документ из файла. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Создаёт документ из потока. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Создаёт документ из структуры, представляющей массив текстовых полей. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Создаёт документ с отложенной загрузкой. |
|
|  | [toString()](#toString--) | Возвращает  java.lang.String  который представляет текущий  Document . |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Получает тип источника документа.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Получает ключ документа, используемый для идентификации документа в индексе.


**Returns:**
java.lang.String - Ключ документа, используемый для идентификации документа в индексе.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Получает значение, указывающее, загружен ли документ по требованию.


**Returns:**
boolean - Значение, указывающее, загружен ли документ по требованию.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Получает дату последнего изменения документа.


**Returns:**
java.util.Date - Дата последнего изменения документа.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Получает расширение, используемое для этого типа документа.


**Returns:**
java.lang.String - Расширение, используемое для этого типа документа.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Получает дополнительные поля документа.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Дополнительные поля документа.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Устанавливает дополнительные поля документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Дополнительные поля для документа. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Получает атрибуты документа.


**Returns:**
java.lang.String[] - Атрибуты документа.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Устанавливает атрибуты документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String[] | Атрибуты документа. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Создаёт документ из файла.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filePath | java.lang.String | Путь к файлу документа. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Создаёт документ из потока.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentKey | java.lang.String | Ключ документа. |
|
|  | modificationDate | java.util.Date | Дата изменения документа. |
|
|  | extension | java.lang.String | Расширение документа. |
|
|  | stream | java.io.InputStream | Поток документа. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Создаёт документ из структуры, представляющей массив текстовых полей.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentKey | java.lang.String | Ключ документа. |
|
|  | modificationDate | java.util.Date | Дата изменения документа. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Поля документа. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Создаёт документ с отложенной загрузкой.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Тип источника документа. Это значение должно соответствовать типу загруженного документа. |
|
|  | documentKey | java.lang.String | Ключ документа. Это значение должно соответствовать ключу загруженного документа. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Загрузчик документа. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Возвращает  java.lang.String  который представляет текущий  Document .


**Returns:**
java.lang.String - Один java.lang.String который представляет текущий Document.

