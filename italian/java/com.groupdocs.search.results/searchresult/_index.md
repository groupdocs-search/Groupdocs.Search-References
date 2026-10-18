---
title: "SearchResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un risultato di ricerca corrispondente a una query di ricerca."
type: docs
weight: 19
url: /it/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Rappresenta un risultato di ricerca corrispondente a una query di ricerca.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Creazione di un indice
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentFolder);
// Impostazione delle opzioni di ricerca
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Impostazione del numero massimo di differenze a 3
// Ricerca di documenti contenenti la parola 'Einstein' o la frase 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Stampa del risultato
System.out.println("Documenti: " + result.getDocumentCount());
System.out.println("Totale occorrenze: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocumento: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOccorrenze: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tCampo: " + field.getFieldName());
System.out.println("\t\tOccorrenze: " + document.getOccurrenceCount());
// Stampa dei termini trovati
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Stampa delle frasi trovate
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


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Ottiene il numero di documenti trovati. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ottiene il numero totale di occorrenze trovate. |
|
|  | [getTruncated()](#getTruncated--) | Restituisce un valore che indica che il risultato è troncato. |
|
|  | [getWarnings()](#getWarnings--) | Restituisce avvisi che descrivono il risultato. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Restituisce un token di ricerca a blocchi per cercare il blocco successivo. |
|
|  | [getStartTime()](#getStartTime--) | Ottiene l'ora di inizio della ricerca. |
|
|  | [getEndTime()](#getEndTime--) | Ottiene l'ora di fine della ricerca. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Ottiene la durata della ricerca in secondi. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Restituisce il documento trovato per indice. |
|
|  | [iterator()](#iterator--) | Restituisce un iteratore che scorre la collezione dei documenti trovati. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Ottiene il numero di documenti trovati.


**Returns:**
int - Il numero di documenti trovati.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Ottiene il numero totale di occorrenze trovate.


**Returns:**
int - Il numero totale di occorrenze trovate.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Restituisce un valore che indica che il risultato è troncato.


**Returns:**
boolean - Un valore che indica che il risultato è troncato.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Restituisce avvisi che descrivono il risultato.


**Returns:**
java.lang.String - Avvisi che descrivono il risultato.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Restituisce un token di ricerca a blocchi per cercare il blocco successivo.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Ottiene l'ora di inizio della ricerca.


**Returns:**
java.util.Date - L'ora di inizio della ricerca.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Ottiene l'ora di fine della ricerca.


**Returns:**
java.util.Date - L'ora di fine della ricerca.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Ottiene la durata della ricerca in secondi.


**Returns:**
double - La durata della ricerca in secondi.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Restituisce il documento trovato per indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indice | int | L'indice di un documento trovato. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Restituisce un iteratore che scorre la collezione dei documenti trovati.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Un iteratore che può essere usato per iterare attraverso la collezione dei documenti trovati.

