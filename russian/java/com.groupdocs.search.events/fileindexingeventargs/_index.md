---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события начала индексации документа."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события начала индексации документа.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getDocument()](#getDocument--) | Получает документ. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Получает полный путь к документу. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Получает ключ документа. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | Получает значение, указывающее, что индексирование документа должно быть пропущено. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Устанавливает значение, указывающее, что индексирование документа должно быть пропущено. |
|
|  | [getEncoding()](#getEncoding--) | Получает кодировку документа. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Устанавливает кодировку документа. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | Получает пользовательский извлекатель текста. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Устанавливает пользовательский извлекатель текста. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Получает дополнительные поля документа. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Устанавливает дополнительные поля документа. |
|
|  | [getAttributes()](#getAttributes--) | Получает атрибуты документа. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Устанавливает атрибуты документа. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Получает документ.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Получает полный путь к документу.


**Returns:**
java.lang.String - Полный путь к документу.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Получает ключ документа.


**Returns:**
java.lang.String - Ключ документа.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Получает значение, указывающее, что индексирование документа должно быть пропущено.


**Returns:**
boolean - Значение, указывающее, что индексирование документа должно быть пропущено.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Устанавливает значение, указывающее, что индексирование документа должно быть пропущено.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Значение, указывающее, что индексирование документа должно быть пропущено. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Получает кодировку документа.


**Returns:**
java.lang.String - Кодировка документа.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Устанавливает кодировку документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String | Кодировка документа. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Получает пользовательский извлекатель текста.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Устанавливает пользовательский извлекатель текста.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | Пользовательский извлекатель текста. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Получает дополнительные поля документа.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Дополнительные поля документа.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Устанавливает дополнительные поля документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Дополнительные поля для документа. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Получает атрибуты документа.


**Returns:**
java.lang.String[] - Атрибуты документа.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Устанавливает атрибуты документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | java.lang.String[] | Атрибуты документа. |
|

