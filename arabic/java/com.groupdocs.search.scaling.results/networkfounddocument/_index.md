---
title: "NetworkFoundDocument"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مستندًا تم العثور عليه في شبكة البحث."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

يمثل مستندًا تم العثور عليه في شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | يحصل على المستند الموجود. |
|
|  | [getShardIndex()](#getShardIndex--) | يحصل على فهرس الجزء. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


يحصل على المستند الموجود.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


يحصل على فهرس الجزء.


**Returns:**
int - فهرس الجزء.

