---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen när en bildförberedelse startar."
type: docs
weight: 15
url: /sv/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen när en bildförberedelse startar.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Hämtar dokumentnyckeln. |
|
|  | [getInnerPath()](#getInnerPath--) | Hämtar den inre sökvägen för ett inbäddat dokument. |
|
|  | [getImageIndex()](#getImageIndex--) | Hämtar ordningsnumret för bilden i dokumentet. |
|
|  | [getImageFrames()](#getImageFrames--) | Hämtar bildramarna. |
|
|  | [getImageStream()](#getImageStream--) | Hämtar bildströmmen. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Hämtar dokumentnyckeln.


**Returns:**
java.lang.String - Dokumentnyckeln.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Hämtar den inre sökvägen för ett inbäddat dokument.


**Returns:**
java.lang.String[] - Den inre sökvägen för ett inbäddat dokument.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Hämtar ordningsnumret för bilden i dokumentet.


**Returns:**
int - Ordningsnumret för bilden i dokumentet.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Hämtar bildramarna.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Bildramarna.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Hämtar bildströmmen.


**Returns:**
java.io.InputStream - Bildströmmen.

