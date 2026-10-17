---
title: "NetworkDocumentInfo"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل واصفًا لمستند مفهرس في شبكة البحث."
type: docs
weight: 10
url: /ar/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

يمثل واصفًا لمستند مفهرس في شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | يحصل على الوصف لمستند مفهرس. |
|
|  | [getShardIndex()](#getShardIndex--) | يحصل على فهرس الجزء. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


يحصل على الوصف لمستند مفهرس.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


يحصل على فهرس الجزء.


**Returns:**
int - فهرس الجزء.

