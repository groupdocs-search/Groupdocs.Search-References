---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Bietet Bildindizierungsoptionen für die umgekehrte Bildsuche."
type: docs
weight: 23
url: /de/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

Bietet Bildindizierungsoptionen für die umgekehrte Bildsuche.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Liest einen Wert, der angibt, ob separate Bilddateien indiziert werden sollen. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Setzt einen Wert, der angibt, ob separate Bilddateien indiziert werden sollen. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Liest einen Wert, der angibt, ob Bilder, die Elemente in einem Container sind (z. B. Bilder in einem ZIP‑Archiv), indiziert werden sollen. |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Setzt einen Wert, der angibt, ob Bilder, die Elemente in einem Container sind (z. B. Bilder in einem ZIP‑Archiv), indiziert werden sollen. |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Liest einen Wert, der angibt, ob eingebettete Bilder (z. B. Bilder in einem DOCX‑Dokument) indiziert werden sollen. |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Setzt einen Wert, der angibt, ob eingebettete Bilder (z. B. Bilder in einem DOCX‑Dokument) indiziert werden sollen. |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Liest einen Wert, der angibt, ob separate Bilddateien indiziert werden sollen. Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob separate Bilddateien indiziert werden sollen.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Setzt einen Wert, der angibt, ob separate Bilddateien indiziert werden sollen. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob separate Bilddateien indiziert werden sollen. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Liest einen Wert, der angibt, ob Bilder, die Elemente in einem Container sind (z. B. Bilder in einem ZIP‑Archiv), indiziert werden sollen. Der Standardwert ist  false .


**Returns:**
boolean - Ein Wert, der angibt, ob Bilder, die Elemente in einem Container sind, indiziert werden sollen.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Setzt einen Wert, der angibt, ob Bilder, die Elemente in einem Container sind (z. B. Bilder in einem ZIP-Archiv), indiziert werden sollen. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob Bilder, die Elemente in einem Container sind, indiziert werden sollen. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Liefert einen Wert, der angibt, ob eingebettete Bilder (z. B. Bilder in einem DOCX-Dokument) indiziert werden sollen. Der Standardwert ist false.


**Returns:**
boolean - Ein Wert, der angibt, ob eingebettete Bilder indiziert werden sollen.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Setzt einen Wert, der angibt, ob eingebettete Bilder (z. B. Bilder in einem DOCX-Dokument) indiziert werden sollen. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Ein Wert, der angibt, ob eingebettete Bilder indiziert werden sollen. |
|

