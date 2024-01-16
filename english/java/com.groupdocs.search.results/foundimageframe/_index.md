---
title: FoundImageFrame
second_title: GroupDocs.Search for Java API Reference
description: Represents a found image frame.
type: docs
weight: 16
url: /java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Represents a found image frame.
## Constructors

| Constructor | Description |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getDocumentInfo()](#getDocumentInfo--) | Gets the document info. |
| [getImageIndex()](#getImageIndex--) | Gets the ordinal number of the image in the document. |
| [getFrameIndex()](#getFrameIndex--) | Gets the index of the frame in the image. |
| [getHashDifferences()](#getHashDifferences--) | Gets the number of mismatched bits in the image hash. |
| [toString()](#toString--) | Returns a  System.String  that represents the current  FoundImageFrame . |
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Gets the document info.

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.
### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Gets the ordinal number of the image in the document.

**Returns:**
int - The ordinal number of the image in the document.
### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Gets the index of the frame in the image.

**Returns:**
int - The index of the frame in the image.
### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Gets the number of mismatched bits in the image hash.

**Returns:**
int - The number of mismatched bits in the image hash.
### toString() {#toString--}
```
public abstract String toString()
```


Returns a  System.String  that represents the current  FoundImageFrame .

**Returns:**
java.lang.String - A  System.String  that represents the current  FoundImageFrame .
