---
title: "SearchOptions"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Optionen für den Suchvorgang bereit."
type: docs
weight: 34
url: /de/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Stellt Optionen für den Suchvorgang bereit.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | Initialisiert eine neue Instanz der SearchOptions-Klasse. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | Initialisiert eine neue Instanz der SearchOptions-Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | Liefert das Flag zur Verwendung von Synonymen bei der Suche. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Setzt das Flag zur Verwendung von Synonymen bei der Suche. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Liefert das Flag zur Verwendung von Homophonen bei der Suche. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Setzt das Flag zur Verwendung von Homophonen bei der Suche. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Liefert das Flag zur Verwendung verschiedener Wortformen bei der Suche. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Setzt das Flag zur Verwendung verschiedener Wortformen bei der Suche. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | Liefert das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verknüpft sind. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | Setzt das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verknüpft sind. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | Liest die Optionen für die unscharfe Suche. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | Liest die Optionen für die Rechtschreibkorrektur. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Liest die Optionen für die Korrektur des Tastaturlayouts. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Liest das Flag für die Groß-/Kleinschreibungssuche. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Setzt das Flag für die Groß-/Kleinschreibungssuche. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Liest die maximale Gesamtanzahl der Vorkommen aller Begriffe in einer Suchanfrage. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Setzt die maximale Gesamtanzahl der Vorkommen aller Begriffe in einer Suchanfrage. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Liest die maximale Anzahl der Vorkommen jedes Begriffs in einer Suchanfrage. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Setzt die maximale Anzahl der Vorkommen jedes Begriffs in einer Suchanfrage. |
|
|  | [getDateFormats()](#getDateFormats--) | Liest die Sammlung von Datumsformaten für die Datumsspannen‑Suche. |
|
|  | [isChunkSearch()](#isChunkSearch--) | Liest das Flag für die Suche nach Chunks. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Setzt das Flag für die Suche nach Chunks. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Ermittelt den Suchdokumentfilter. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Setzt den Suchdokumentfilter. |
|
|  | [getCancellation()](#getCancellation--) | Liest das Abbruchobjekt der Operation. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Setzt das Abbruchobjekt der Operation. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initialisiert eine neue Instanz der SearchOptions-Klasse.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


Initialisiert eine neue Instanz der SearchOptions-Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Daten | java.lang.Object | Die serialisierten Daten. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


Liest das Flag für die Verwendung von Synonymen in der Suche. Der Standardwert ist  false .


**Returns:**
boolean - Das Flag für die Verwendung von Synonymen in der Suche.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


Setzt das Flag für die Verwendung von Synonymen in der Suche. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag für die Verwendung von Synonymen in der Suche. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


Liest das Flag für die Verwendung von Homophonen in der Suche. Der Standardwert ist  false .


**Returns:**
boolean - Das Flag für die Verwendung von Homophonen in der Suche.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


Setzt das Flag für die Verwendung von Homophonen in der Suche. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag für die Verwendung von Homophonen in der Suche. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


Liest das Flag für die Verwendung verschiedener Wortformen in der Suche. Der Standardwert ist  false .


**Returns:**
boolean - Das Flag für die Verwendung verschiedener Wortformen in der Suche.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


Setzt das Flag für die Verwendung verschiedener Wortformen in der Suche. Der Standardwert ist  false .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag zur Verwendung unterschiedlicher Wortformen bei der Suche. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


Liest das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verbunden sind. Der Standardwert ist false.


**Returns:**
boolean - Das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verbunden sind.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


Setzt das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verbunden sind. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag zum Abrufen von Attributen, die mit gefundenen Dokumenten verbunden sind. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


Liest die Optionen für die unscharfe Suche.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


Liest die Optionen für die Rechtschreibkorrektur.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Liest die Optionen für die Korrektur des Tastaturlayouts.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


Liest das Flag für die Groß-/Kleinschreibungssuche. Der Standardwert ist false.


**Returns:**
boolean - Das Flag für die Groß-/Kleinschreibungssuche.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


Setzt das Flag für die Groß-/Kleinschreibungssuche. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag für die Groß-/Kleinschreibungssuche. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


Liest die maximale Gesamtanzahl der Vorkommen aller Begriffe in einer Suchanfrage. Der Standardwert ist 500000.


**Returns:**
int - Die maximale Gesamtanzahl der Vorkommen.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


Setzt die maximale Gesamtanzahl der Vorkommen aller Begriffe in einer Suchanfrage. Der Standardwert ist 500000.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Gesamtanzahl der Vorkommen. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


Liest die maximale Anzahl der Vorkommen jedes Begriffs in einer Suchanfrage. Der Standardwert ist 100000.


**Returns:**
int - Die maximale Anzahl der Vorkommen jedes Begriffs in einer Suchanfrage.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


Setzt die maximale Anzahl der Vorkommen jedes Begriffs in einer Suchanfrage. Der Standardwert ist 100000.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | int | Die maximale Anzahl der Vorkommen jedes Begriffs in einer Suchanfrage. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


Liest die Sammlung von Datumsformaten für die Datumsspanne-Suche. Die Standard-Datumsformate sind 'dd.MM.yyyy', 'MM/dd/yyyy' und 'yyyy-MM-dd'.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


Das Beispiel zeigt, wie die Datumsformate für die Suche festgelegt werden.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Erstellen eines Index im angegebenen Ordner
index.add(documentsFolder); // Indizieren von Dokumenten aus dem angegebenen Ordner
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // Entfernt Standard-Datumsformate
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// Erstellen eines Datumsformatmusters 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // Suche im Index
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


Liest das Flag für die Suche in Teilen. Der Standardwert ist false.


**Returns:**
boolean - Das Flag für die Suche in Teilen.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


Setzt das Flag für die Suche in Teilen. Der Standardwert ist false.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | boolean | Das Flag für die Suche in Teilen. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Liest den Suchdokumentfilter.  SearchDocumentFilter  arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse  SearchDocumentFilter  zur Erstellung von Instanzen des Suchdokumentfilters. Der Standardwert ist null, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


Das Beispiel zeigt, wie man den DocumentFilter festlegt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten
index.add(documentsFolder);
// Erstellen eines Suchdokumentfilters, der Dokumente mit den Erweiterungen '.doc', '.docx', '.rtf' überspringt
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(\".doc\", \".docx\", \".rtf\"); // Erstellen eines Dateierweiterungsfilters
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Invertieren des Dateierweiterungsfilters
options.setSearchDocumentFilter(invertedFilter);
// Suche im Index
SearchResult result = index.search(\"Einstein\", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Legt den Suchdokumentfilter fest.  SearchDocumentFilter  arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse  SearchDocumentFilter  zur Erstellung von Instanzen eines Suchdokumentfilters. Der Standardwert ist  null , was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Der Suchdokumentfilter. |


Das Beispiel zeigt, wie man den DocumentFilter festlegt.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten
index.add(documentsFolder);
// Erstellen eines Suchdokumentfilters, der Dokumente mit den Erweiterungen '.doc', '.docx', '.rtf' überspringt
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(\".doc\", \".docx\", \".rtf\"); // Erstellen eines Dateierweiterungsfilters
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Invertieren des Dateierweiterungsfilters
options.setSearchDocumentFilter(invertedFilter);
// Suche im Index
SearchResult result = index.search(\"Einstein\", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Gibt das Abbruchobjekt der Operation zurück. Der Standardwert ist  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Legt das Abbruchobjekt der Operation fest. Der Standardwert ist  null .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Das Abbruchobjekt der Operation. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
