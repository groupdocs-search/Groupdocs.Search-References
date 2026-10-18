---
title: "DocumentImage"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Dokumentbilddaten dar."
type: docs
weight: 16
url: /de/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

Stellt Dokumentbilddaten dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | Gibt die Ordnungszahl des Bildes im Dokument zurück. |
|
|  | [getFields()](#getFields--) | Ruft die extrahierten Felder ab. |
|
|  | [getFrames()](#getFrames--) | Gibt die Bildrahmen zurück. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Gibt die Ordnungszahl des Bildes im Dokument zurück.


**Returns:**
int - Die Ordnungszahl des Bildes im Dokument.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


Ruft die extrahierten Felder ab.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Die extrahierten Felder.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


Gibt die Bildrahmen zurück.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Die Bildrahmen.

