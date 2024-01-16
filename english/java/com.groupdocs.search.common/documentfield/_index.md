---
title: DocumentField
second_title: GroupDocs.Search for Java API Reference
description: Represents a document field data.
type: docs
weight: 15
url: /java/com.groupdocs.search.common/documentfield/
---
**Inheritance:**
java.lang.Object
```
public class DocumentField
```

Represents a document field data.

**Learn more**

 *  [Custom text extractors][]
 *  [Indexing additional fields][]


[Custom text extractors]: https://docs.groupdocs.com/display/searchjava/Custom+text+extractors
[Indexing additional fields]: https://docs.groupdocs.com/display/searchjava/Indexing+additional+fields
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentField(String name, String value)](#DocumentField-java.lang.String-java.lang.String-) | Initializes a new instance of the  DocumentField  class. |
| [DocumentField(Object data)](#DocumentField-java.lang.Object-) | Initializes a new instance of the  DocumentField  class. |
## Methods

| Method | Description |
| --- | --- |
| [getName()](#getName--) | Gets a field name. |
| [getValue()](#getValue--) | Gets a field value. |
| [getCore()](#getCore--) |  |
### DocumentField(String name, String value) {#DocumentField-java.lang.String-java.lang.String-}
```
public DocumentField(String name, String value)
```


Initializes a new instance of the  DocumentField  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | The field name. |
| value | java.lang.String | The field value. |

### DocumentField(Object data) {#DocumentField-java.lang.Object-}
```
public DocumentField(Object data)
```


Initializes a new instance of the  DocumentField  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | java.lang.Object | The serialized data. |

### getName() {#getName--}
```
public String getName()
```


Gets a field name.

**Returns:**
java.lang.String - The field name.
### getValue() {#getValue--}
```
public String getValue()
```


Gets a field value.

**Returns:**
java.lang.String - The field value.
### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
