---
title: DocumentImage
second_title: GroupDocs.Search for Java API Reference
description: Represents a document image data.
type: docs
weight: 16
url: /java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Represents a document image data.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Gets the ordinal number of the image in the document. |
| [getFields()](#getFields--) | Gets the extracted fields. |
| [getFrames()](#getFrames--) | Gets the image frames. |
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Gets the ordinal number of the image in the document.

**Returns:**
int - The ordinal number of the image in the document.
### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Gets the extracted fields.

**Returns:**
com.groupdocs.search.common.DocumentField[] - The extracted fields.
### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Gets the image frames.

**Returns:**
com.groupdocs.search.common.ImageFrame[] - The image frames.
