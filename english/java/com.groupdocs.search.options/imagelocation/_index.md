---
title: ImageLocation
second_title: GroupDocs.Search for Java API Reference
description: Specifies an image location.
type: docs
weight: 48
url: /java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

Specifies an image location.
## Fields

| Field | Description |
| --- | --- |
| [Separate](#Separate) | An image in separate file. |
| [Embedded](#Embedded) | An image embedded in another document. |
| [ContainerItem](#ContainerItem) | An image that is an element in a container file. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


An image in separate file.

### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


An image embedded in another document.

### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


An image that is an element in a container file.

### values() {#values--}
```
public static ImageLocation[] values()
```




**Returns:**
com.groupdocs.search.options.ImageLocation[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ImageLocation valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
