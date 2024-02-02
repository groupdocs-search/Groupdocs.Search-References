---
title: NetworkSearchResult
second_title: GroupDocs.Search for Java API Reference
description: Represents a search result matching a search query.
type: docs
weight: 14
url: /java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

Represents a search result matching a search query.
## Constructors

| Constructor | Description |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDocumentCount()](#getDocumentCount--) | Gets the number of documents found. |
| [getOccurrenceCount()](#getOccurrenceCount--) | Gets the total number of occurrences found. |
| [getTruncated()](#getTruncated--) | Gets a value indicating that the result is truncated. |
| [getWarnings()](#getWarnings--) | Gets a warnings describing the result. |
| [getStartTime()](#getStartTime--) | Gets the start time of the search. |
| [getEndTime()](#getEndTime--) | Gets the end time of the search. |
| [getSearchDuration()](#getSearchDuration--) | Gets the search duration in seconds. |
| [getFoundDocument(int index)](#getFoundDocument-int-) | Gets the found document by index. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection of the documents found. |
| [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Gets a chunk search token for searching the next chunk. |
| [getNodeIndex()](#getNodeIndex--) | Gets the index of the node from which the result was received. |
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Gets the number of documents found.

**Returns:**
int - The number of documents found.
### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Gets the total number of occurrences found.

**Returns:**
int - The total number of occurrences found.
### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Gets a value indicating that the result is truncated.

**Returns:**
boolean - A value indicating that the result is truncated.
### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Gets a warnings describing the result.

**Returns:**
java.lang.String - A warnings describing the result.
### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Gets the start time of the search.

**Returns:**
java.util.Date - The start time of the search.
### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Gets the end time of the search.

**Returns:**
java.util.Date - The end time of the search.
### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Gets the search duration in seconds.

**Returns:**
double - The search duration in seconds.
### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


Gets the found document by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of a found document. |

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.
### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


Returns an iterator that iterates through the collection of the documents found.

**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - An iterator that can be used to iterate through the collection of the found documents.
### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


Gets a chunk search token for searching the next chunk.

**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.
### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


Gets the index of the node from which the result was received.

**Returns:**
int - The index of the node from which the result was received.
