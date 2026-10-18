---
title: "SearchReport"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta informazioni dettagliate su un'operazione di ricerca."
type: docs
weight: 30
url: /it/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Rappresenta informazioni dettagliate su un'operazione di ricerca.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti dalla cartella specificata
index.add(documentsFolder);
// Ricerca nell'indice
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Ottenere i report di ricerca
SearchReport[] reports = index.getSearchReports();
// Stampa i report sulla console
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println(\"Tempo: \" + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Ottiene l'ora di inizio della ricerca. |
|
|  | [getEndTime()](#getEndTime--) | Ottiene l'ora di fine della ricerca. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Ottiene la durata della ricerca in secondi. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Ottiene il numero di documenti trovati. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ottiene il numero totale di occorrenze trovate. |
|
|  | [getTextQuery()](#getTextQuery--) | Ottiene la query di ricerca in forma testuale. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Ottiene la query di ricerca in forma di oggetto. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Ottiene le opzioni di ricerca. |
|
|  | [toString()](#toString--) | Restituisce una Stringa che rappresenta l'attuale SearchReport. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Ottiene la query di ricerca in forma testuale.


**Returns:**
java.lang.String - La query di ricerca in forma testuale.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Ottiene la query di ricerca in forma di oggetto.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Ottiene le opzioni di ricerca.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Restituisce una Stringa che rappresenta l'attuale SearchReport.


**Returns:**
java.lang.String - Una stringa che rappresenta il corrente SearchReport.

