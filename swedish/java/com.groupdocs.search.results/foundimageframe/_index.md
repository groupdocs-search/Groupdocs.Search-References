---
title: "FoundImageFrame"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en hittad bildram."
type: docs
weight: 16
url: /sv/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Representerar en hittad bildram.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Hämtar dokumentinformationen. |
|
|  | [getImageIndex()](#getImageIndex--) | Hämtar ordningsnumret för bilden i dokumentet. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Hämtar indexet för ramen i bilden. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Hämtar antalet felmatchade bitar i bildhashen. |
|
|  | [toString()](#toString--) | Returnerar en  System.String  som representerar den aktuella  FoundImageFrame . |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Hämtar dokumentinformationen.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Hämtar ordningsnumret för bilden i dokumentet.


**Returns:**
int - Ordningsnumret för bilden i dokumentet.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Hämtar indexet för ramen i bilden.


**Returns:**
int - Indexet för ramen i bilden.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Hämtar antalet felmatchade bitar i bildhashen.


**Returns:**
int - Antalet felmatchade bitar i bildhashen.

### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en  System.String  som representerar den aktuella  FoundImageFrame .


**Returns:**
java.lang.String - En  System.String  som representerar den aktuella  FoundImageFrame .

