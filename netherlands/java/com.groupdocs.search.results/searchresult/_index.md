---
title: "SearchResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een zoekresultaat voor dat overeenkomt met een zoekopdracht."
type: docs
weight: 19
url: /nl/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Stelt een zoekresultaat voor dat overeenkomt met een zoekopdracht.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Een index maken
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentFolder);
// Instellen van zoekopties
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Fuzzy-zoekopdracht inschakelen
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Instellen van het maximale aantal verschillen op 3
// Zoeken naar documenten die het woord 'Einstein' of de zin 'Theory of Relativity' bevatten
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Het resultaat afdrukken
System.out.println("Documents: " + result.getDocumentCount());
System.out.println("Total occurrences: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocument: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOccurrences: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tField: " + field.getFieldName());
System.out.println("\t\tOccurrences: " + document.getOccurrenceCount());
// Afdrukken gevonden termen
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Afdrukken gevonden zinnen
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Haalt het aantal gevonden documenten op. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Haalt het totale aantal gevonden voorkomens op. |
|
|  | [getTruncated()](#getTruncated--) | Haalt een waarde op die aangeeft dat het resultaat is afgekapt. |
|
|  | [getWarnings()](#getWarnings--) | Haalt een waarschuwing op die het resultaat beschrijft. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Haalt een chunk-zoektoken op voor het zoeken naar de volgende chunk. |
|
|  | [getStartTime()](#getStartTime--) | Haalt de starttijd van de zoekopdracht op. |
|
|  | [getEndTime()](#getEndTime--) | Haalt de eindtijd van de zoekopdracht op. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Haalt de zoekduur in seconden op. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Haalt het gevonden document op via index. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de verzameling van de gevonden documenten iterereert. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Haalt het aantal gevonden documenten op.


**Returns:**
int - Het aantal gevonden documenten.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Haalt het totale aantal gevonden voorkomens op.


**Returns:**
int - Het totale aantal gevonden voorkomens.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Haalt een waarde op die aangeeft dat het resultaat is afgekapt.


**Returns:**
boolean - Een waarde die aangeeft dat het resultaat is afgekapt.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Haalt een waarschuwing op die het resultaat beschrijft.


**Returns:**
java.lang.String - Een waarschuwing die het resultaat beschrijft.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Haalt een chunk-zoektoken op voor het zoeken naar de volgende chunk.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Haalt de starttijd van de zoekopdracht op.


**Returns:**
java.util.Date - De starttijd van de zoekopdracht.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Haalt de eindtijd van de zoekopdracht op.


**Returns:**
java.util.Date - De eindtijd van de zoekopdracht.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Haalt de zoekduur in seconden op.


**Returns:**
double - De zoekduur in seconden.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Haalt het gevonden document op via index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | index | int | De index van een gevonden document. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Retourneert een iterator die door de verzameling van de gevonden documenten iterereert.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Een iterator die kan worden gebruikt om door de collectie van de gevonden documenten te itereren.

