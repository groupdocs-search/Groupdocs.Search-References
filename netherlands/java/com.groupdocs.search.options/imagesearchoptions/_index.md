---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor de bewerking omgekeerd zoeken naar afbeeldingen."
type: docs
weight: 24
url: /nl/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Biedt opties voor de bewerking omgekeerd zoeken naar afbeeldingen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Initialiseert een nieuw exemplaar van de  ImageSearchOptions  klasse. |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Initialiseert een nieuw exemplaar van de  ImageSearchOptions  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Haalt het maximale aantal niet-overeenkomende bits in de afbeeldinghash op. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Stelt het maximale aantal niet-overeenkomende bits in de afbeeldinghash in. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Haalt het maximale aantal gevonden afbeeldingen op voor een omgekeerde afbeeldingzoekopdracht. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Stelt het maximale aantal gevonden afbeeldingen in voor een omgekeerde afbeeldingzoekopdracht. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Haalt het zoekdocumentfilter op. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Haalt het zoekdocumentfilter op of stelt het in. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Initialiseert een nieuw exemplaar van de  ImageSearchOptions  klasse.


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Initialiseert een nieuw exemplaar van de  ImageSearchOptions  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Haalt het maximale aantal niet-overeenkomende bits in de afbeeldinghash op. De standaardwaarde is  5 .


**Returns:**
int - Het maximale aantal niet-overeenkomende bits in de afbeeldinghash.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Stelt het maximale aantal niet-overeenkomende bits in de afbeeldinghash in. De standaardwaarde is 5.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal niet-overeenkomende bits in de afbeeldinghash. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Haalt het maximale aantal gevonden afbeeldingen op voor een omgekeerd afbeeldingzoekverzoek. De standaardwaarde is 1000.


**Returns:**
int - Het maximale aantal gevonden afbeeldingen voor een omgekeerd afbeeldingzoekverzoek.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Stelt het maximale aantal gevonden afbeeldingen in voor een omgekeerd afbeeldingzoekverzoek. De standaardwaarde is 1000.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal gevonden afbeeldingen voor een omgekeerd afbeeldingzoekverzoek. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Haalt de zoekdocumentfilter op. SearchDocumentFilter werkt volgens de inclusielogica. Gebruik de class GroupDocs.Search.Options.SearchDocumentFilter voor het maken van zoekdocumentfilter‑instanties. De standaardwaarde is null, wat betekent dat alle gevonden documenten worden geretourneerd.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Haalt de zoekdocumentfilter op of stelt deze in. SearchDocumentFilter werkt volgens de inclusielogica. Gebruik de class GroupDocs.Search.Options.SearchDocumentFilter voor het maken van zoekdocumentfilter‑instanties. De standaardwaarde is null, wat betekent dat alle gevonden documenten worden geretourneerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | De zoekdocumentfilter. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
