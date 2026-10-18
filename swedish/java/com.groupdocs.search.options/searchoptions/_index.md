---
title: "SearchOptions"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller alternativ för sökoperationen."
type: docs
weight: 34
url: /sv/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Tillhandahåller alternativ för sökoperationen.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Initierar en ny instans av  SearchOptions  -klassen. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Initierar en ny instans av  SearchOptions  -klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Hämtar flaggan för att använda synonymer i sökning. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Ställer in flaggan för att använda synonymer i sökning. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Hämtar flaggan för att använda homofoner i sökning. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Ställer in flaggan för att använda homofoner i sökning. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Hämtar flaggan för att använda olika ordformer i sökning. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Ställer in flaggan för att använda olika ordformer i sökning. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Hämtar flaggan för att hämta attribut som är associerade med hittade dokument. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Ställer in flaggan för att hämta attribut som är associerade med hittade dokument. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Hämtar alternativen för fuzzy-sökning. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Hämtar alternativen för stavningskorrigering. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Hämtar alternativen för tangentbordslayoutkorrigering. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Hämtar flaggan för skiftlägeskänslig sökning. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Ställer in flaggan för skiftlägeskänslig sökning. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Hämtar det maximala totala antalet förekomster av alla termer i en sökfråga. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Ställer in det maximala totala antalet förekomster av alla termer i en sökfråga. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Hämtar det maximala antalet förekomster av varje term i en sökfråga. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Ställer in det maximala antalet förekomster av varje term i en sökfråga. |
|
|  | [getDateFormats()](#getDateFormats--) | Hämtar samlingen av datumformat för datumintervallsökning. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Hämtar flaggan för sökning i delar. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Ställer in flaggan för sökning i delar. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Hämtar sökdokumentfiltret. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Ställer in filtret för sökdokument. |
|
|  | [getCancellation()](#getCancellation--) | Hämtar objektet för avbrytning av operationen. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ställer in objektet för avbrytning av operationen. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initierar en ny instans av  SearchOptions  -klassen.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Initierar en ny instans av  SearchOptions  -klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Hämtar flaggan för att använda synonymer i sökning. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för att använda synonymer i sökning.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Ställer in flaggan för att använda synonymer i sökning. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för att använda synonymer i sökning. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Hämtar flaggan för att använda homofoner i sökning. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för att använda homofoner i sökning.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Ställer in flaggan för att använda homofoner i sökning. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för att använda homofoner i sökning. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Hämtar flaggan för att använda olika ordformer i sökning. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för att använda olika ordformer i sökning.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Ställer in flaggan för att använda olika ordformer i sökning. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för att använda olika ordformer i sökningen. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Hämtar flaggan för att hämta attribut som är associerade med hittade dokument. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för att hämta attribut som är associerade med hittade dokument.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Ställer in flaggan för att hämta attribut som är associerade med hittade dokument. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för att hämta attribut som är associerade med hittade dokument. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Hämtar alternativen för fuzzy-sökning.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Hämtar alternativen för stavningskorrigering.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Hämtar alternativen för tangentbordslayoutkorrigering.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Hämtar flaggan för skiftlägeskänslig sökning. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för skiftlägeskänslig sökning.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Ställer in flaggan för skiftlägeskänslig sökning. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för skiftlägeskänslig sökning. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Hämtar det maximala totala antalet förekomster av alla termer i en sökfråga. Standardvärdet är  500000 .


**Returns:**
int - Det maximala totala antalet förekomster.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Ställer in det maximala totala antalet förekomster av alla termer i en sökfråga. Standardvärdet är  500000 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala totala antalet förekomster. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Hämtar det maximala antalet förekomster för varje term i en sökfråga. Standardvärdet är  100000 .


**Returns:**
int - Det maximala antalet förekomster för varje term i en sökfråga.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Ställer in det maximala antalet förekomster för varje term i en sökfråga. Standardvärdet är  100000 .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | int | Det maximala antalet förekomster för varje term i en sökfråga. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Hämtar samlingen av datumformat för datumintervallsökning. Standarddatumformaten är 'dd.MM.yyyy', 'MM/dd/yyyy' och 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Exemplet visar hur man ställer in datumformaten för sökningen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Skapar ett index i den angivna mappen
index.add(documentsFolder); // Indexerar dokument från den angivna mappen
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Tar bort standarddatumformat
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Skapar ett datumformatmönster 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Sök i index
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Hämtar flaggan för sökning i delar. Standardvärdet är  false .


**Returns:**
boolean - Flaggan för sökning i delar.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Ställer in flaggan för sökning i delar. Standardvärdet är  false .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | boolean | Flaggan för sökning i delar. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Hämtar sökdokumentfiltret.  SearchDocumentFilter  fungerar enligt inklusionslogik. Använd  SearchDocumentFilter  -klassen för att skapa instanser av ett sökdokumentfilter. Standardvärdet är  null , vilket betyder att alla hittade dokument kommer att returneras.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Exemplet visar hur man ställer in dokumentfiltret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument
index.add(documentsFolder);
// Skapar ett sökdokumentfilter som hoppar över dokument med filändelserna '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Skapar filter för filändelser
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inverterar filter för filändelser
options.setSearchDocumentFilter(invertedFilter);
// Sök i indexet
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Ställer in sökdokumentfiltret.  SearchDocumentFilter  fungerar med inklusionslogiken. Använd  SearchDocumentFilter  klass för att skapa instanser av ett sökdokumentfilter. Standardvärdet är  null , vilket betyder att alla hittade dokument kommer att returneras.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Sökdokumentfiltret. |


Exemplet visar hur man ställer in dokumentfiltret.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument
index.add(documentsFolder);
// Skapar ett sökdokumentfilter som hoppar över dokument med filändelserna '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Skapar filter för filändelser
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inverterar filter för filändelser
options.setSearchDocumentFilter(invertedFilter);
// Sök i indexet
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Hämtar objektet för avbrytning av operationen. Standardvärdet är  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Ställer in objektet för avbrytning av operationen. Standardvärdet är  null .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objektet för avbrytning av operationen. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
