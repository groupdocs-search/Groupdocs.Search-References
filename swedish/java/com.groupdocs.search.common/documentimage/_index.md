---
title: "DocumentImage"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar dokumentbilddata."
type: docs
weight: 16
url: /sv/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Representerar dokumentbilddata.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Hämtar ordningsnumret för bilden i dokumentet. |
|
|  | [getFields()](#getFields--) | Hämtar de extraherade fälten. |
|
|  | [getFrames()](#getFrames--) | Hämtar bildramarna. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Hämtar ordningsnumret för bilden i dokumentet.


**Returns:**
int - Ordningsnumret för bilden i dokumentet.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Hämtar de extraherade fälten.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De extraherade fälten.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Hämtar bildramarna.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Bildramarna.

