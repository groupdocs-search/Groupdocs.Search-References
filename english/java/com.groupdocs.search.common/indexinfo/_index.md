---
title: IndexInfo
second_title: GroupDocs.Search for Java API Reference
description: Contains basic information on an Index.
type: docs
weight: 24
url: /java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Contains basic information on an  Index .
## Constructors

| Constructor | Description |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getIndexId()](#getIndexId--) | Gets the index unique identifier. |
| [getIndexFolder()](#getIndexFolder--) | Gets the full folder name where index is located. |
| [getIndexStatus()](#getIndexStatus--) | Gets the index status. |
| [getVersion()](#getVersion--) | Gets the index version. |
| [getSegmentCount()](#getSegmentCount--) | Gets the number of index segments. |
| [getTermCount()](#getTermCount--) | Gets the number of words in the index. |
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Gets the index unique identifier.

**Returns:**
java.util.UUID - The index unique identifier.
### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Gets the full folder name where index is located.

**Returns:**
java.lang.String - The full folder name where index is located.
### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Gets the index status.

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.
### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Gets the index version.

**Returns:**
java.lang.String - The index version.
### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Gets the number of index segments.

**Returns:**
int - The number of index segments.
### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Gets the number of words in the index.

**Returns:**
int - The number of words in the index.
