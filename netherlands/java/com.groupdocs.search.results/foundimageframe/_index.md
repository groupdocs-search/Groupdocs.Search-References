---
title: "FoundImageFrame"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een gevonden afbeeldingsframe voor."
type: docs
weight: 16
url: /nl/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

Stelt een gevonden afbeeldingsframe voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Haalt de documentinformatie op. |
|
|  | [getImageIndex()](#getImageIndex--) | Haalt het ordinale nummer van de afbeelding in het document op. |
|
|  | [getFrameIndex()](#getFrameIndex--) | Haalt de index van het frame in de afbeelding op. |
|
|  | [getHashDifferences()](#getHashDifferences--) | Haalt het aantal niet‑overeenkomende bits in de afbeeldingshash op. |
|
|  | [toString()](#toString--) | Retourneert een  System.String  die het huidige  FoundImageFrame  vertegenwoordigt. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Haalt de documentinformatie op.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


Haalt het ordinale nummer van de afbeelding in het document op.


**Returns:**
int - Het ordinale nummer van de afbeelding in het document.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


Haalt de index van het frame in de afbeelding op.


**Returns:**
int - De index van het frame in de afbeelding.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


Haalt het aantal niet‑overeenkomende bits in de afbeeldingshash op.


**Returns:**
int - Het aantal niet‑overeenkomende bits in de afbeeldingshash.

### toString() {#toString--}
```
public abstract String toString()
```


Retourneert een  System.String  die het huidige  FoundImageFrame  vertegenwoordigt.


**Returns:**
java.lang.String - Een  System.String  die het huidige  FoundImageFrame  vertegenwoordigt.

