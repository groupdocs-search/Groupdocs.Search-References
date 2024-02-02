---
title: IndexStatus
second_title: GroupDocs.Search for Java API Reference
description: Specifies an index status.
type: docs
weight: 41
url: /java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Specifies an index status.
## Fields

| Field | Description |
| --- | --- |
| [Ready](#Ready) | Index is free and ready to change. |
| [Failed](#Failed) | Index needs to be reloaded due to an error. |
| [Indexing](#Indexing) | Index performs an indexing operation. |
| [Updating](#Updating) | Index performs an updating operation. |
| [Merging](#Merging) | Index performs a merging operation. |
| [Optimizing](#Optimizing) | Index performs an optimizing operation. |
| [Deleting](#Deleting) | Index performs a deleting operation. |
| [Renaming](#Renaming) | Index performs a renaming operation. |
| [ChangingAttributes](#ChangingAttributes) | Index changes attributes. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Index is free and ready to change.

### Failed {#Failed}
```
public static final IndexStatus Failed
```


Index needs to be reloaded due to an error.

### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Index performs an indexing operation.

### Updating {#Updating}
```
public static final IndexStatus Updating
```


Index performs an updating operation.

### Merging {#Merging}
```
public static final IndexStatus Merging
```


Index performs a merging operation.

### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Index performs an optimizing operation.

### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Index performs a deleting operation.

### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Index performs a renaming operation.

### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Index changes attributes.

### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
