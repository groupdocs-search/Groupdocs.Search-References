---
title: "AttributeChangeBatch"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل حاوية لتغييرات السمات."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

يمثل حاوية لتغييرات السمات.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | ينشئ مثيلاً جديداً من الفئة  AttributeChangeBatch  . |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | ينشئ مثيلاً جديداً من الفئة  AttributeChangeBatch  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | يضيف السمات المحددة إلى المستند المفهرس المحدد. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | يضيف السمات المحددة إلى المستندات المفهرسة المحددة. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | يضيف السمات المحددة إلى جميع المستندات في الفهرس. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | يزيل السمات المحددة من المستند المفهرس المحدد. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | يزيل السمات المحددة من المستندات المفهرسة المحددة. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | يزيل جميع السمات من المستند المفهرس المحدد. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | يزيل جميع السمات من المستندات المفهرسة المحددة. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | يزيل السمات المحددة من جميع المستندات في الفهرس. |
|
|  | [clear()](#clear--) | يزيل جميع السمات من جميع المستندات في الفهرس. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


ينشئ مثيلاً جديداً من الفئة  AttributeChangeBatch  .


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


ينشئ مثيلاً جديداً من الفئة  AttributeChangeBatch  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


يضيف السمات المحددة إلى المستند المفهرس المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | مسار المستند. |
|
|  | attributes | java.lang.String[] | السمات التي سيتم إضافتها. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


يضيف السمات المحددة إلى المستندات المفهرسة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المسارات | java.lang.String[] | مسارات المستندات. |
|
|  | attributes | java.lang.String[] | السمات التي سيتم إضافتها. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


يضيف السمات المحددة إلى جميع المستندات في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | attributes | java.lang.String[] | السمات التي سيتم إضافتها. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


يزيل السمات المحددة من المستند المفهرس المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | مسار المستند. |
|
|  | attributes | java.lang.String[] | السمات التي سيتم إزالتها. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


يزيل السمات المحددة من المستندات المفهرسة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المسارات | java.lang.String[] | مسارات المستندات. |
|
|  | attributes | java.lang.String[] | السمات التي سيتم إزالتها. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


يزيل جميع السمات من المستند المفهرس المحدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | path | java.lang.String | مسار المستند. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


يزيل جميع السمات من المستندات المفهرسة المحددة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | المسارات | java.lang.String[] | مسارات المستندات. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


يزيل السمات المحددة من جميع المستندات في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | attributes | java.lang.String[] | السمات التي سيتم إزالتها. |
|

### clear() {#clear--}
```
public void clear()
```


يزيل جميع السمات من جميع المستندات في الفهرس.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
