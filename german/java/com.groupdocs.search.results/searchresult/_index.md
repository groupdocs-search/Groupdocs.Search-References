---
title: "SearchResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt."
type: docs
weight: 19
url: /de/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Stellt ein Suchergebnis dar, das zu einer Suchanfrage passt.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Erstellen eines Index
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentFolder);
// Festlegen der Suchoptionen
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Aktivieren der unscharfen Suche
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Festlegen der maximalen Anzahl von Unterschieden auf 3
// Suche nach Dokumenten, die das Wort 'Einstein' oder die Phrase 'Theory of Relativity' enthalten
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Ausgeben des Ergebnisses
System.out.println("Dokumente: " + result.getDocumentCount());
System.out.println("Gesamte Vorkommen: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDokument: " + document.getDocumentInfo().getFilePath());
System.out.println("\tVorkommen: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tFeld: " + field.getFieldName());
System.out.println("\t\tVorkommen: " + document.getOccurrenceCount());
// Ausgabe gefundener Begriffe
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Ausgabe gefundener Phrasen
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


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Ermittelt die Anzahl gefundener Dokumente. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ermittelt die Gesamtzahl gefundener Vorkommen. |
|
|  | [getTruncated()](#getTruncated--) | Gibt einen Wert zurück, der anzeigt, dass das Ergebnis abgeschnitten ist. |
|
|  | [getWarnings()](#getWarnings--) | Gibt eine Warnung zurück, die das Ergebnis beschreibt. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Gibt ein Chunk-Such-Token für die Suche nach dem nächsten Chunk zurück. |
|
|  | [getStartTime()](#getStartTime--) | Ermittelt die Startzeit der Suche. |
|
|  | [getEndTime()](#getEndTime--) | Ermittelt die Endzeit der Suche. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Ermittelt die Suchdauer in Sekunden. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Gibt das gefundene Dokument nach Index zurück. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung der gefundenen Dokumente iteriert. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Ermittelt die Anzahl gefundener Dokumente.


**Returns:**
int - Die Anzahl gefundener Dokumente.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Ermittelt die Gesamtzahl gefundener Vorkommen.


**Returns:**
int - Die Gesamtzahl gefundener Vorkommen.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Gibt einen Wert zurück, der anzeigt, dass das Ergebnis abgeschnitten ist.


**Returns:**
boolean - Ein Wert, der anzeigt, dass das Ergebnis abgeschnitten ist.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Gibt eine Warnung zurück, die das Ergebnis beschreibt.


**Returns:**
java.lang.String - Eine Warnung, die das Ergebnis beschreibt.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Gibt ein Chunk-Such-Token für die Suche nach dem nächsten Chunk zurück.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Ermittelt die Startzeit der Suche.


**Returns:**
java.util.Date - Die Startzeit der Suche.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Ermittelt die Endzeit der Suche.


**Returns:**
java.util.Date - Die Endzeit der Suche.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Ermittelt die Suchdauer in Sekunden.


**Returns:**
double - Die Suchdauer in Sekunden.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Gibt das gefundene Dokument nach Index zurück.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Index | int | Der Index eines gefundenen Dokuments. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung der gefundenen Dokumente iteriert.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Ein Iterator, der verwendet werden kann, um durch die Sammlung der gefundenen Dokumente zu iterieren.

