---
title: "FoundImageFrame"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen gefundenen Bildrahmen dar."
type: docs
weight: 16
url: /de/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Stellt einen gefundenen Bildrahmen dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Liefert die Dokumentinformationen. |
|
|  | [getImageIndex()](#getImageIndex--) | Gibt die Ordnungszahl des Bildes im Dokument zurück. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Liefert den Index des Frames im Bild. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Liefert die Anzahl der nicht übereinstimmenden Bits im Bild‑Hash. |
|
|  | [toString()](#toString--) | Gibt einen  System.String  zurück, der das aktuelle  FoundImageFrame  repräsentiert. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Liefert die Dokumentinformationen.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Gibt die Ordnungszahl des Bildes im Dokument zurück.


**Returns:**
int - Die Ordnungszahl des Bildes im Dokument.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Liefert den Index des Frames im Bild.


**Returns:**
int - Der Index des Frames im Bild.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Liefert die Anzahl der nicht übereinstimmenden Bits im Bild‑Hash.


**Returns:**
int - Die Anzahl der nicht übereinstimmenden Bits im Bild‑Hash.

### toString() {#toString--}
```
public abstract String toString()
```


Gibt einen  System.String  zurück, der das aktuelle  FoundImageFrame  repräsentiert.


**Returns:**
java.lang.String - Ein  System.String  der das aktuelle  FoundImageFrame  repräsentiert.

