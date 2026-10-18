---
title: "SearchOptions"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Fornisce opzioni per l'operazione di ricerca."
type: docs
weight: 34
url: /it/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Fornisce opzioni per l'operazione di ricerca.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Inizializza una nuova istanza della classe SearchOptions. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Inizializza una nuova istanza della classe SearchOptions. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Restituisce il flag per l'uso dei sinonimi nella ricerca. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Imposta il flag per l'uso dei sinonimi nella ricerca. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Restituisce il flag per l'uso di omofoni nella ricerca. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Imposta il flag per l'uso di omofoni nella ricerca. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Restituisce il flag per l'uso di forme diverse delle parole nella ricerca. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Imposta il flag per l'uso di forme diverse delle parole nella ricerca. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Restituisce il flag per il recupero degli attributi associati ai documenti trovati. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Imposta il flag per il recupero degli attributi associati ai documenti trovati. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Restituisce le opzioni di ricerca fuzzy. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Restituisce le opzioni del correttore ortografico. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Restituisce le opzioni del correttore di layout della tastiera. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Restituisce il flag della ricerca sensibile al maiuscolo/minuscolo. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Imposta il flag della ricerca sensibile al maiuscolo/minuscolo. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Restituisce il numero totale massimo di occorrenze di tutti i termini in una query di ricerca. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Imposta il numero totale massimo di occorrenze di tutti i termini in una query di ricerca. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Restituisce il numero massimo di occorrenze di ciascun termine in una query di ricerca. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Imposta il numero massimo di occorrenze di ciascun termine in una query di ricerca. |
|
|  | [getDateFormats()](#getDateFormats--) | Restituisce la collezione di formati data per la ricerca per intervallo di date. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Restituisce il flag della ricerca per blocchi. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Imposta il flag della ricerca per blocchi. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Ottiene il filtro del documento di ricerca. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Imposta il filtro dei documenti di ricerca. |
|
|  | [getCancellation()](#getCancellation--) | Restituisce l'oggetto di annullamento dell'operazione. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Imposta l'oggetto di annullamento dell'operazione. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Inizializza una nuova istanza della classe SearchOptions.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Inizializza una nuova istanza della classe SearchOptions.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Restituisce il flag dell'uso dei sinonimi nella ricerca. Il valore predefinito è false.


**Returns:**
boolean - Il flag dell'uso dei sinonimi nella ricerca.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Imposta il flag dell'uso dei sinonimi nella ricerca. Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag dell'uso dei sinonimi nella ricerca. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Restituisce il flag dell'uso di omofoni nella ricerca. Il valore predefinito è false.


**Returns:**
boolean - Il flag dell'uso di omofoni nella ricerca.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Imposta il flag dell'uso di omofoni nella ricerca. Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag dell'uso di omofoni nella ricerca. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Restituisce il flag dell'uso di forme diverse delle parole nella ricerca. Il valore predefinito è false.


**Returns:**
boolean - Il flag dell'uso di forme diverse delle parole nella ricerca.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Imposta il flag dell'uso di forme diverse delle parole nella ricerca. Il valore predefinito è false.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag per utilizzare forme diverse di parole nella ricerca. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Ottiene il flag per il recupero degli attributi associati ai documenti trovati. Il valore predefinito è  false .


**Returns:**
boolean - Il flag per il recupero degli attributi associati ai documenti trovati.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Imposta il flag per il recupero degli attributi associati ai documenti trovati. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag per il recupero degli attributi associati ai documenti trovati. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Restituisce le opzioni di ricerca fuzzy.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Restituisce le opzioni del correttore ortografico.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Restituisce le opzioni del correttore di layout della tastiera.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Ottiene il flag per la ricerca sensibile alle maiuscole. Il valore predefinito è  false .


**Returns:**
boolean - Il flag per la ricerca sensibile alle maiuscole.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Imposta il flag per la ricerca sensibile alle maiuscole. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag per la ricerca sensibile alle maiuscole. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Ottiene il numero totale massimo di occorrenze di tutti i termini in una query di ricerca. Il valore predefinito è  500000 .


**Returns:**
int - Il numero totale massimo di occorrenze.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Imposta il numero totale massimo di occorrenze di tutti i termini in una query di ricerca. Il valore predefinito è  500000 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero totale massimo di occorrenze. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Ottiene il numero massimo di occorrenze di ciascun termine in una query di ricerca. Il valore predefinito è  100000 .


**Returns:**
int - Il numero massimo di occorrenze di ciascun termine in una query di ricerca.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Imposta il numero massimo di occorrenze di ciascun termine in una query di ricerca. Il valore predefinito è  100000 .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | int | Il numero massimo di occorrenze di ciascun termine in una query di ricerca. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Ottiene la raccolta di formati data per la ricerca per intervallo di date. I formati data predefiniti sono 'dd.MM.yyyy', 'MM/dd/yyyy' e 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


L'esempio dimostra come impostare i formati data per la ricerca.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Rimozione dei formati data predefiniti
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Creazione di un modello di formato data 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Cerca nell'indice
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Ottiene il flag per la ricerca per blocchi. Il valore predefinito è  false .


**Returns:**
boolean - Il flag per la ricerca per blocchi.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Imposta il flag per la ricerca per blocchi. Il valore predefinito è  false .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | valore | boolean | Il flag per la ricerca per blocchi. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Ottiene il filtro dei documenti di ricerca.  SearchDocumentFilter  funziona con la logica di inclusione. Utilizzare la classe  SearchDocumentFilter  per creare istanze di filtro dei documenti di ricerca. Il valore predefinito è  null , il che significa che tutti i documenti trovati saranno restituiti.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


L'esempio dimostra come impostare il filtro documento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti
index.add(documentsFolder);
// Creazione di un filtro di documenti di ricerca che ignora i documenti con estensioni '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creazione del filtro di estensione file
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inversione del filtro di estensione file
options.setSearchDocumentFilter(invertedFilter);
// Ricerca nell'indice
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Imposta il filtro di documenti di ricerca.  SearchDocumentFilter  funziona sulla logica di inclusione. Usa la classe  SearchDocumentFilter  per creare istanze di filtri di documenti di ricerca. Il valore predefinito è  null , il che significa che tutti i documenti trovati saranno restituiti.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Il filtro dei documenti di ricerca. |


L'esempio dimostra come impostare il filtro documento.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti
index.add(documentsFolder);
// Creazione di un filtro di documenti di ricerca che ignora i documenti con estensioni '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creazione del filtro di estensione file
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inversione del filtro di estensione file
options.setSearchDocumentFilter(invertedFilter);
// Ricerca nell'indice
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Ottiene l'oggetto di annullamento dell'operazione. Il valore predefinito è  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è  null .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | L'oggetto di annullamento dell'operazione. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
