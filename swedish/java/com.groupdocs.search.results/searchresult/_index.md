---
title: "SearchResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett sökresultat som matchar en sökfråga."
type: docs
weight: 19
url: /sv/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Representerar ett sökresultat som matchar en sökfråga.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Skapar ett index
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentFolder);
// Ställer in sökalternativ
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktiverar fuzzy-sökning
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Ställer in maximalt antal skillnader till 3
// Sök efter dokument som innehåller ordet 'Einstein' eller frasen 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Skriver ut resultatet
System.out.println("Dokument: " + result.getDocumentCount());
System.out.println("Totalt antal förekomster: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDokument: " + document.getDocumentInfo().getFilePath());
System.out.println("\tFörekomster: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tFält: " + field.getFieldName());
System.out.println("\t\tFörekomster: " + document.getOccurrenceCount());
// Skriver ut hittade termer
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Skriver ut hittade fraser
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


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Hämtar antalet hittade dokument. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Hämtar det totala antalet hittade förekomster. |
|
|  | [getTruncated()](#getTruncated--) | Hämtar ett värde som indikerar att resultatet är avkortat. |
|
|  | [getWarnings()](#getWarnings--) | Hämtar en varning som beskriver resultatet. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Hämtar en token för segment-sökning för att söka nästa segment. |
|
|  | [getStartTime()](#getStartTime--) | Hämtar starttiden för sökningen. |
|
|  | [getEndTime()](#getEndTime--) | Hämtar sluttiden för sökningen. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Hämtar sökvaraktigheten i sekunder. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Hämtar det hittade dokumentet efter index. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen av de hittade dokumenten. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Hämtar antalet hittade dokument.


**Returns:**
int - Antalet hittade dokument.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Hämtar det totala antalet hittade förekomster.


**Returns:**
int - Det totala antalet hittade förekomster.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Hämtar ett värde som indikerar att resultatet är avkortat.


**Returns:**
boolean - Ett värde som indikerar att resultatet är avkortat.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Hämtar en varning som beskriver resultatet.


**Returns:**
java.lang.String - En varning som beskriver resultatet.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Hämtar en token för segment-sökning för att söka nästa segment.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Hämtar starttiden för sökningen.


**Returns:**
java.util.Date - Starttiden för sökningen.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Hämtar sluttiden för sökningen.


**Returns:**
java.util.Date - Sluttiden för sökningen.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Hämtar sökvaraktigheten i sekunder.


**Returns:**
double - Sökvaraktigheten i sekunder.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Hämtar det hittade dokumentet efter index.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | index | int | Indexet för ett hittat dokument. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Returnerar en iterator som itererar genom samlingen av de hittade dokumenten.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - En iterator som kan användas för att iterera genom samlingen av de hittade dokumenten.

