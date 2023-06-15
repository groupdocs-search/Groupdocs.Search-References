---
title: OperationType
second_title: GroupDocs.Search for Java API Reference
description: Represents an index operation type.
type: docs
weight: 23
url: /java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Represents an index operation type.
## Fields

| Field | Description |
| --- | --- |
| [Indexing](#Indexing) | Adding documents to an index. |
| [Updating](#Updating) | Updating documents in an index. |
| [Merging](#Merging) | Merging indexes. |
| [Optimizing](#Optimizing) | Optimizing an index. |
| [Deleting](#Deleting) | Deleting paths from an index. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Adding documents to an index.

### Updating {#Updating}
```
public static final OperationType Updating
```


Updating documents in an index.

### Merging {#Merging}
```
public static final OperationType Merging
```


Merging indexes.

### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Optimizing an index.

### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Deleting paths from an index.

### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
