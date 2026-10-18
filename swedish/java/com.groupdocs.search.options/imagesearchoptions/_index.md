---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för operationen omvänd bildsökning."
type: docs
weight: 24
url: /sv/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Tillhandahåller alternativ för operationen omvänd bildsökning.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Initierar en ny instans av klassen  ImageSearchOptions  . |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Initierar en ny instans av klassen  ImageSearchOptions  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Hämtar det maximala antalet mismatcherade bitar i bildhashen. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Ställer in det maximala antalet mismatcherade bitar i bildhashen. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Hämtar det maximala antalet hittade bilder för en omvänd bildsökning. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Ställer in det maximala antalet hittade bilder för en omvänd bildsökning. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Hämtar sökdokumentfiltret. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Hämtar eller ställer in sökdokumentfiltret. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Initierar en ny instans av klassen  ImageSearchOptions  .


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Initierar en ny instans av klassen  ImageSearchOptions  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Hämtar det maximala antalet mismatcherade bitar i bildhashen. Standardvärdet är  5 .


**Returns:**
int - Det maximala antalet felmatchande bitar i bildens hash.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Ställer in det maximala antalet felmatchande bitar i bildens hash. Standardvärdet är 5.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet felmatchande bitar i bildens hash. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Hämtar det maximala antalet hittade bilder för en omvänd bildsökning. Standardvärdet är 1000.


**Returns:**
int - Det maximala antalet hittade bilder för en omvänd bildsökning.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Ställer in det maximala antalet hittade bilder för en omvänd bildsökning. Standardvärdet är 1000.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet hittade bilder för en omvänd bildsökning. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Hämtar sökdokumentfiltret. SearchDocumentFilter fungerar med inklusionslogik. Använd GroupDocs.Search.Options.SearchDocumentFilter-klassen för att skapa instanser av ett sökdokumentfilter. Standardvärdet är null, vilket betyder att alla hittade dokument kommer att returneras.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Hämtar eller anger sökdokumentfiltret. SearchDocumentFilter fungerar med inklusionslogik. Använd GroupDocs.Search.Options.SearchDocumentFilter-klassen för att skapa instanser av ett sökdokumentfilter. Standardvärdet är null, vilket betyder att alla hittade dokument kommer att returneras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Sökdokumentfiltret. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
