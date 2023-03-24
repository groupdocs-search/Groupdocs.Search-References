---
title: AttributeChangeBatch
second_title: GroupDocs.Search for Java API Reference
description: Represents a container for attribute changes.
type: docs
weight: 12
url: /java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public abstract class AttributeChangeBatch
```

Represents a container for attribute changes.

**Learn more**

 *  [Document attributes][]
 *  [Document filtering in search result][]


[Document attributes]: https://docs.groupdocs.com/display/searchjava/Document+attributes
[Document filtering in search result]: https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result
## Methods

| Method | Description |
| --- | --- |
| [create()](#create--) | Initializes a new instance of the  AttributeChangeBatch  class. |
| [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Adds the specified attributes to the specified indexed document. |
| [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Adds the specified attributes to the specified indexed documents. |
| [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Adds the specified attributes to all documents in the index. |
| [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Removes the specified attributes from the specified indexed document. |
| [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Removes the specified attributes from the specified indexed documents. |
| [removeAll(String path)](#removeAll-java.lang.String-) | Removes all attributes from the specified indexed document. |
| [removeAll(String[] paths)](#removeAll-java.lang.String---) | Removes all attributes from the specified indexed documents. |
| [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Removes the specified attributes from all documents in the index. |
| [clear()](#clear--) | Removes all attributes from all documents in the index. |
### create() {#create--}
```
public static AttributeChangeBatch create()
```


Initializes a new instance of the  AttributeChangeBatch  class.

**Returns:**
[AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) - A new instance of the  AttributeChangeBatch  class.
### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public abstract void add(String path, String[] attributes)
```


Adds the specified attributes to the specified indexed document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The document path. |
| attributes | java.lang.String[] | The attributes to add. |

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public abstract void add(String[] paths, String[] attributes)
```


Adds the specified attributes to the specified indexed documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| paths | java.lang.String[] | The documents paths. |
| attributes | java.lang.String[] | The attributes to add. |

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public abstract void addToAll(String[] attributes)
```


Adds the specified attributes to all documents in the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| attributes | java.lang.String[] | The attributes to add. |

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public abstract void remove(String path, String[] attributes)
```


Removes the specified attributes from the specified indexed document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The document path. |
| attributes | java.lang.String[] | The attributes to remove. |

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public abstract void remove(String[] paths, String[] attributes)
```


Removes the specified attributes from the specified indexed documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| paths | java.lang.String[] | The documents paths. |
| attributes | java.lang.String[] | The attributes to remove. |

### removeAll(String path) {#removeAll-java.lang.String-}
```
public abstract void removeAll(String path)
```


Removes all attributes from the specified indexed document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The document path. |

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public abstract void removeAll(String[] paths)
```


Removes all attributes from the specified indexed documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| paths | java.lang.String[] | The documents paths. |

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public abstract void removeFromAll(String[] attributes)
```


Removes the specified attributes from all documents in the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| attributes | java.lang.String[] | The attributes to remove. |

### clear() {#clear--}
```
public abstract void clear()
```


Removes all attributes from all documents in the index.

