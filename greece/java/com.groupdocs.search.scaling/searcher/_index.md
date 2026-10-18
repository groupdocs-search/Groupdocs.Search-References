---
title: "Searcher"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει μια υπηρεσία που διαχειρίζεται ερωτήματα αναζήτησης προς τα τμήματα του δικτύου αναζήτησης."
type: docs
weight: 12
url: /el/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Αντιπροσωπεύει μια υπηρεσία που διαχειρίζεται ερωτήματα αναζήτησης προς τα τμήματα του δικτύου αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Ξεκινά μια αναζήτηση με ένα ερώτημα σε μορφή κειμένου στον κατανεμημένο ευρετήριο αναζήτησης. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Ξεκινά μια αναζήτηση στον κατανεμημένο ευρετήριο αναζήτησης. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Εκτελεί αντίστροφη αναζήτηση εικόνας στον κατανεμημένο ευρετήριο αναζήτησης. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Συνεχίζει μια αναζήτηση στον κατανεμημένο ευρετήριο αναζήτησης. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Συνεχίζει μια αντίστροφη αναζήτηση εικόνας στον κατανεμημένο ευρετήριο αναζήτησης. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Λαμβάνει έναν πίνακα με όλα τα ευρετηριασμένα έγγραφα. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Λαμβάνει έναν πίνακα με τα ένθετα στοιχεία του καθορισμένου εγγράφου (για έγγραφα κοντέινερ όπως ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Δημιουργεί το κείμενο ενός ευρετηριασμένου εγγράφου και το περνά μέσω ενός προσαρμογέα εξόδου. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Ξεκινά μια αναζήτηση με ένα ερώτημα σε μορφή κειμένου στον κατανεμημένο ευρετήριο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | java.lang.String | Το ερώτημα αναζήτησης. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Ξεκινά μια αναζήτηση στον κατανεμημένο ευρετήριο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Το ερώτημα αναζήτησης. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Οι επιλογές αναζήτησης. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Εκτελεί αντίστροφη αναζήτηση εικόνας στον κατανεμημένο ευρετήριο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Η εικόνα για αναζήτηση. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Οι επιλογές αναζήτησης εικόνας. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Συνεχίζει μια αναζήτηση στον κατανεμημένο ευρετήριο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Το διακριτικό αναζήτησης δικτύου. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Συνεχίζει μια αντίστροφη αναζήτηση εικόνας στον κατανεμημένο ευρετήριο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Το διακριτικό αναζήτησης εικόνας δικτύου. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Το ευρεθέν έγγραφο. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Ο επισημαστής αποτελεσμάτων αναζήτησης. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Οι επιλογές επισήμανσης. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Λαμβάνει έναν πίνακα με όλα τα ευρετηριασμένα έγγραφα.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | shardIndex | int | Ο δείκτης τμήματος. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Ένας πίνακας όλων των ευρετηριασμένων εγγράφων.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Λαμβάνει έναν πίνακα με τα ένθετα στοιχεία του καθορισμένου εγγράφου (για έγγραφα κοντέινερ όπως ZIP, OST, PST).


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Η πληροφορία εγγράφου. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Ένας πίνακας στοιχείων εγγράφου.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Δημιουργεί το κείμενο ενός ευρετηριασμένου εγγράφου και το περνά μέσω ενός προσαρμογέα εξόδου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Οι πληροφορίες του ευρετηριασμένου εγγράφου. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Ο προσαρμογέας εξόδου. |
|

