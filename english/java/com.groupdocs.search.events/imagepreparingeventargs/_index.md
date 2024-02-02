---
title: ImagePreparingEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of an image preparing start.
type: docs
weight: 16
url: /java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event of an image preparing start.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getDocumentKey()](#getDocumentKey--) | Gets the document key. |
| [getInnerPath()](#getInnerPath--) | Gets the inner path of a nested document. |
| [getImageIndex()](#getImageIndex--) | Gets the ordinal number of the image in the document. |
| [getImageFrames()](#getImageFrames--) | Gets the image frames. |
| [getImageStream()](#getImageStream--) | Gets the image stream. |
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Gets the document key.

**Returns:**
java.lang.String - The document key.
### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Gets the inner path of a nested document.

**Returns:**
java.lang.String[] - The inner path of a nested document.
### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Gets the ordinal number of the image in the document.

**Returns:**
int - The ordinal number of the image in the document.
### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Gets the image frames.

**Returns:**
com.groupdocs.search.common.ImageFrame[] - The image frames.
### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Gets the image stream.

**Returns:**
java.io.InputStream - The image stream.
