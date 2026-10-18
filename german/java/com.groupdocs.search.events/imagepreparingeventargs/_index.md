---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, wenn die Vorbereitung eines Bildes startet."
type: docs
weight: 15
url: /de/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, wenn die Vorbereitung eines Bildes startet.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Ermittelt den Dokumentenschlüssel. |
|
|  | [getInnerPath()](#getInnerPath--) | Gibt den inneren Pfad eines verschachtelten Dokuments zurück. |
|
|  | [getImageIndex()](#getImageIndex--) | Gibt die Ordnungszahl des Bildes im Dokument zurück. |
|
|  | [getImageFrames()](#getImageFrames--) | Gibt die Bildrahmen zurück. |
|
|  | [getImageStream()](#getImageStream--) | Gibt den Bild-Stream zurück. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Ermittelt den Dokumentenschlüssel.


**Returns:**
java.lang.String - Der Dokumentenschlüssel.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Gibt den inneren Pfad eines verschachtelten Dokuments zurück.


**Returns:**
java.lang.String[] - Der innere Pfad eines verschachtelten Dokuments.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Gibt die Ordnungszahl des Bildes im Dokument zurück.


**Returns:**
int - Die Ordnungszahl des Bildes im Dokument.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Gibt die Bildrahmen zurück.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Die Bildrahmen.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Gibt den Bild-Stream zurück.


**Returns:**
java.io.InputStream - Der Bild-Stream.

