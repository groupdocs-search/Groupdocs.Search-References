---
title: ImageSearchResult
second_title: GroupDocs.Search for Java API Reference
description: Represents the result of a reverse image search.
type: docs
weight: 17
url: /java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

Represents the result of a reverse image search.
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getImageCount()](#getImageCount--) | Gets the number of images found. |
| [getFoundImage(int index)](#getFoundImage-int-) | Gets the found image by index. |
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


Gets the number of images found.

**Returns:**
int - The number of images found.
### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


Gets the found image by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of a found image. |

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.
