---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer de voorbereiding van een afbeelding start."
type: docs
weight: 15
url: /nl/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer de voorbereiding van een afbeelding start.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Haalt de document-sleutel op. |
|
|  | [getInnerPath()](#getInnerPath--) | Haalt het interne pad van een genesteld document op. |
|
|  | [getImageIndex()](#getImageIndex--) | Haalt het ordinale nummer van de afbeelding in het document op. |
|
|  | [getImageFrames()](#getImageFrames--) | Haalt de afbeeldingsframes op. |
|
|  | [getImageStream()](#getImageStream--) | Haalt de afbeeldingsstroom op. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Haalt de document-sleutel op.


**Returns:**
java.lang.String - De document-sleutel.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Haalt het interne pad van een genesteld document op.


**Returns:**
java.lang.String[] - Het interne pad van een genesteld document.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Haalt het ordinale nummer van de afbeelding in het document op.


**Returns:**
int - Het ordinale nummer van de afbeelding in het document.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Haalt de afbeeldingsframes op.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - De afbeeldingsframes.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Haalt de afbeeldingsstroom op.


**Returns:**
java.io.InputStream - De afbeeldingsstroom.

