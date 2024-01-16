---
title: SearchImage
second_title: GroupDocs.Search for Java API Reference
description: Represents an image to search.
type: docs
weight: 29
url: /java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Represents an image to search.
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Methods

| Method | Description |
| --- | --- |
| [create(String filePath)](#create-java.lang.String-) | Creates an image from a file to search. |
| [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Creates an image from a file to search. |
| [create(InputStream stream)](#create-java.io.InputStream-) | Creates an image from a stream to search. |
| [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Creates an image from a stream to search. |
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Creates an image from a file to search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The image file path. |

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.
### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Creates an image from a file to search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The image file path. |
| imageIndex | int | The image index in multipage images. |

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.
### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Creates an image from a stream to search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The image stream. |

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.
### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Creates an image from a stream to search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The image stream. |
| imageIndex | int | The image index in multipage images. |

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.
