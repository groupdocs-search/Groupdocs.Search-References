---
title: IndexInfo
second_title: GroupDocs.Search for Java API Reference
description: Contains basic information on an Index.
type: docs
weight: 10
url: /java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public class IndexInfo
```

Contains basic information on an  Index .
## Methods

| Method | Description |
| --- | --- |
| [getIndexId()](#getIndexId--) | Gets the index unique identifier. |
| [getIndexFolder()](#getIndexFolder--) | Gets the full folder name where index is located. |
| [getIndexStatus()](#getIndexStatus--) | Gets the index status. |
| [getVersion()](#getVersion--) | Gets the index version. |
| [getSegmentCount()](#getSegmentCount--) | Gets the number of index segments. |
| [getTermCount()](#getTermCount--) | Gets the number of words in the index. |
### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Gets the index unique identifier.

**Returns:**
java.util.UUID - The index unique identifier.
### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Gets the full folder name where index is located.

**Returns:**
java.lang.String - The full folder name where index is located.
### getIndexStatus() {#getIndexStatus--}
```
public final IndexStatus getIndexStatus()
```


Gets the index status.

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.
### getVersion() {#getVersion--}
```
public final String getVersion()
```


Gets the index version.

**Returns:**
java.lang.String - The index version.
### getSegmentCount() {#getSegmentCount--}
```
public final int getSegmentCount()
```


Gets the number of index segments.

**Returns:**
int - The number of index segments.
### getTermCount() {#getTermCount--}
```
public final int getTermCount()
```


Gets the number of words in the index.

**Returns:**
int - The number of words in the index.
