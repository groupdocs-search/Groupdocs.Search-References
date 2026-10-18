---
title: "SearchOptions"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt opties voor de zoekbewerking."
type: docs
weight: 34
url: /nl/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Biedt opties voor de zoekbewerking.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Initialiseert een nieuw exemplaar van de SearchOptions-klasse. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Initialiseert een nieuw exemplaar van de SearchOptions-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Haalt de vlag op voor het gebruik van synoniemen bij zoeken. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Stelt de vlag in voor het gebruik van synoniemen bij zoeken. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Haalt de vlag op voor het gebruik van homofonen bij zoeken. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Stelt de vlag in voor het gebruik van homofonen bij zoeken. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Haalt de vlag op voor het gebruik van verschillende woordvormen bij zoeken. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Stelt de vlag in voor het gebruik van verschillende woordvormen bij zoeken. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Haalt de vlag op voor het ophalen van attributen die bij gevonden documenten horen. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Stelt de vlag in voor het ophalen van attributen die aan gevonden documenten zijn gekoppeld. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Haalt de opties voor fuzzy zoeken op. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Haalt de opties voor de spellingscorrector op. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Haalt de opties voor de toetsenbordindelingcorrector op. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Haalt de vlag op voor hoofdlettergevoelig zoeken. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Stelt de vlag in voor hoofdlettergevoelig zoeken. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Haalt het maximale totale aantal voorkomens van alle termen in een zoekopdracht op. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Stelt het maximale totale aantal voorkomens van alle termen in een zoekopdracht in. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Haalt het maximale aantal voorkomens van elke term in een zoekopdracht op. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Stelt het maximale aantal voorkomens van elke term in een zoekopdracht in. |
|
|  | [getDateFormats()](#getDateFormats--) | Haalt de collectie datumformaten op voor datumbereik zoeken. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Haalt de vlag op voor zoeken per fragmenten. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Stelt de vlag in voor zoeken per fragmenten. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Haalt het zoekdocumentfilter op. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Stelt het zoekdocumentfilter in. |
|
|  | [getCancellation()](#getCancellation--) | Haalt het annuleringsobject van de bewerking op. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Stelt het annuleringsobject van de bewerking in. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initialiseert een nieuw exemplaar van de SearchOptions-klasse.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Initialiseert een nieuw exemplaar van de SearchOptions-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Haalt de vlag op voor het gebruik van synoniemen in zoeken. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor het gebruik van synoniemen in zoeken.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Stelt de vlag in voor het gebruik van synoniemen in zoeken. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor het gebruik van synoniemen in zoeken. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Haalt de vlag op voor het gebruik van homofonen in zoeken. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor het gebruik van homofonen in zoeken.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Stelt de vlag in voor het gebruik van homofonen in zoeken. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor het gebruik van homofonen in zoeken. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Haalt de vlag op voor het gebruik van verschillende woordvormen in zoeken. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor het gebruik van verschillende woordvormen in zoeken.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Stelt de vlag in voor het gebruik van verschillende woordvormen in zoeken. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor het gebruiken van verschillende woordvormen bij zoeken. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Haalt de vlag op voor het ophalen van attributen die bij gevonden documenten horen. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor het ophalen van attributen die bij gevonden documenten horen.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Stelt de vlag in voor het ophalen van attributen die bij gevonden documenten horen. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor het ophalen van attributen die bij gevonden documenten horen. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Haalt de opties voor fuzzy zoeken op.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Haalt de opties voor de spellingscorrector op.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Haalt de opties voor de toetsenbordindelingcorrector op.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Haalt de vlag op voor hoofdlettergevoelig zoeken. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor hoofdlettergevoelig zoeken.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Stelt de vlag in voor hoofdlettergevoelig zoeken. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor hoofdlettergevoelig zoeken. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Haalt het maximale totale aantal voorkomens van alle termen in een zoekopdracht op. De standaardwaarde is 500000.


**Returns:**
int - Het maximale totale aantal voorkomens.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Stelt het maximale totale aantal voorkomens van alle termen in een zoekopdracht in. De standaardwaarde is 500000.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale totale aantal voorkomens. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Haalt het maximale aantal voorkomens van elke term in een zoekopdracht op. De standaardwaarde is 100000.


**Returns:**
int - Het maximale aantal voorkomens van elke term in een zoekopdracht.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Stelt het maximale aantal voorkomens van elke term in een zoekopdracht in. De standaardwaarde is 100000.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | int | Het maximale aantal voorkomens van elke term in een zoekopdracht. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Haalt de collectie datumformaten op voor datumreeks zoeken. De standaard datumformaten zijn 'dd.MM.yyyy', 'MM/dd/yyyy' en 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Het voorbeeld toont hoe de datumformaten voor de zoekopdracht in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Een index maken in de opgegeven map
index.add(documentsFolder); // Documenten indexeren vanuit de opgegeven map
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Verwijdert standaard datumformaten
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Een datumformaatpatroon maken 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Zoeken in index
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Haalt de vlag op voor zoeken in delen. De standaardwaarde is false.


**Returns:**
boolean - De vlag voor zoeken in delen.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Stelt de vlag in voor zoeken in delen. De standaardwaarde is false.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | boolean | De vlag voor zoeken in delen. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Haalt de zoekdocumentfilter op.  SearchDocumentFilter  werkt op basis van de inclusielogica. Gebruik de  SearchDocumentFilter  klasse voor het maken van zoekdocumentfilter‑instanties. De standaardwaarde is null, wat betekent dat alle gevonden documenten worden geretourneerd.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Het voorbeeld toont hoe het documentfilter in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren
index.add(documentsFolder);
// Een zoekdocumentfilter maken dat documenten met extensies '.doc', '.docx', '.rtf' overslaat
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Een filter voor bestandsextensies maken
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Het filter voor bestandsextensies omkeren
options.setSearchDocumentFilter(invertedFilter);
// Zoeken in index
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Stelt het zoekdocumentfilter in. SearchDocumentFilter werkt op de inclusielogica. Gebruik de SearchDocumentFilter-klasse voor het maken van instanties van een zoekdocumentfilter. De standaardwaarde is null, wat betekent dat alle gevonden documenten worden geretourneerd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | De zoekdocumentfilter. |


Het voorbeeld toont hoe het documentfilter in te stellen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren
index.add(documentsFolder);
// Een zoekdocumentfilter maken dat documenten met extensies '.doc', '.docx', '.rtf' overslaat
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Een filter voor bestandsextensies maken
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Het filter voor bestandsextensies omkeren
options.setSearchDocumentFilter(invertedFilter);
// Zoeken in index
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Haalt het annuleringsobject van de bewerking op. De standaardwaarde is null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Stelt het annuleringsobject van de bewerking in. De standaardwaarde is null.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Het annuleringsobject van de bewerking. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
