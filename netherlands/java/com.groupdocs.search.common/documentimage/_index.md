---
title: "DocumentImage"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt documentafbeeldingsgegevens voor."
type: docs
weight: 16
url: /nl/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Stelt documentafbeeldingsgegevens voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Haalt het ordinale nummer van de afbeelding in het document op. |
|
|  | [getFields()](#getFields--) | Haalt de geëxtraheerde velden op. |
|
|  | [getFrames()](#getFrames--) | Haalt de afbeeldingsframes op. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Haalt het ordinale nummer van de afbeelding in het document op.


**Returns:**
int - Het ordinale nummer van de afbeelding in het document.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Haalt de geëxtraheerde velden op.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De geëxtraheerde velden.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Haalt de afbeeldingsframes op.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - De afbeeldingsframes.

