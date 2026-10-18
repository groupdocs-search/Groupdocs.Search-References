---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Bietet Optionen für die umgekehrte Bildsuche‑Operation."
type: docs
weight: 24
url: /de/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Bietet Optionen für die umgekehrte Bildsuche‑Operation.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Initialisiert eine neue Instanz der Klasse ImageSearchOptions. |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Initialisiert eine neue Instanz der Klasse ImageSearchOptions. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Ermittelt die maximale Anzahl von nicht übereinstimmenden Bits im Bild-Hash. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Setzt die maximale Anzahl von nicht übereinstimmenden Bits im Bild-Hash. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Ermittelt die maximale Anzahl gefundener Bilder für eine umgekehrte Bildsuche. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Setzt die maximale Anzahl gefundener Bilder für eine umgekehrte Bildsuche. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Ermittelt den Suchdokumentfilter. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Ermittelt oder setzt den Suchdokumentfilter. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Initialisiert eine neue Instanz der Klasse ImageSearchOptions.


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Initialisiert eine neue Instanz der Klasse ImageSearchOptions.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Ermittelt die maximale Anzahl von nicht übereinstimmenden Bits im Bild-Hash. Der Standardwert ist 5.


**Returns:**
int - Die maximale Anzahl von nicht übereinstimmenden Bits im Bild-Hash.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Legt die maximale Anzahl von nicht übereinstimmenden Bits im Bild-Hash fest. Der Standardwert ist 5.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl von nicht übereinstimmenden Bits im Bild-Hash. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Ruft die maximale Anzahl gefundener Bilder für eine umgekehrte Bildsuche ab. Der Standardwert ist 1000.


**Returns:**
int - Die maximale Anzahl gefundener Bilder für eine umgekehrte Bildsuche.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Legt die maximale Anzahl gefundener Bilder für eine umgekehrte Bildsuche fest. Der Standardwert ist 1000.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl gefundener Bilder für eine umgekehrte Bildsuche. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Ruft den Suchdokumentfilter ab.  SearchDocumentFilter  arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse  GroupDocs.Search.Options.SearchDocumentFilter  zur Erstellung von Instanzen des Suchdokumentfilters. Der Standardwert ist null, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Ruft den Suchdokumentfilter ab oder legt ihn fest.  SearchDocumentFilter  arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse  GroupDocs.Search.Options.SearchDocumentFilter  zur Erstellung von Instanzen des Suchdokumentfilters. Der Standardwert ist null, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Der Suchdokumentfilter. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
