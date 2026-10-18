---
title: "IndexingReport"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta informazioni dettagliate su un'operazione di indicizzazione."
type: docs
weight: 25
url: /it/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Rappresenta informazioni dettagliate su un'operazione di indicizzazione.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
// Indicizzazione dei documenti
index.add(documentsFolder1);
index.add(documentsFolder2);
// Ottenere i report di indicizzazione
IndexingReport[] reports = index.getIndexingReports();
// Stampa i report sulla console
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println(\"Tempo: \" + df.format(report.getStartTime()));
System.out.println(\"Durata: \" + report.getIndexingTime());
System.out.println(\"Documenti totali: \" + report.getTotalDocumentsInIndex());
System.out.println(\"Termini totali: \" + report.getTotalTermCount());
System.out.println(\"Dimensione dei documenti indicizzati (MB): \" + report.getIndexedDocumentsSize());
System.out.println(\"Dimensione indice (MB): \" + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Restituisce il numero totale di documenti nell'indice. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Restituisce il numero totale di termini nell'indice. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Restituisce la lunghezza totale dei documenti indicizzati in MB. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Restituisce il numero di segmenti dell'indice. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Restituisce la dimensione totale dell'indice in byte. |
|
|  | [getStartTime()](#getStartTime--) | Restituisce l'ora di inizio dell'indicizzazione. |
|
|  | [getEndTime()](#getEndTime--) | Restituisce l'ora di fine dell'indicizzazione. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Restituisce la durata dell'indicizzazione in secondi. |
|
|  | [getErrors()](#getErrors--) | Restituisce l'elenco degli errori. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Restituisce l'elenco dei documenti indicizzati. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Restituisce l'elenco dei documenti aggiornati. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Restituisce l'elenco dei documenti rimossi dall'indice. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Restituisce il numero totale di documenti nell'indice.


**Returns:**
int - Il numero totale di documenti nell'indice.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Restituisce il numero totale di termini nell'indice.


**Returns:**
int - Il numero totale di termini nell'indice.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Restituisce la lunghezza totale dei documenti indicizzati in MB.


**Returns:**
double - La lunghezza totale dei documenti indicizzati in MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Restituisce il numero di segmenti dell'indice.


**Returns:**
int - Il numero di segmenti dell'indice.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Restituisce la dimensione totale dell'indice in byte.


**Returns:**
long - La dimensione totale dell'indice in byte.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Restituisce l'ora di inizio dell'indicizzazione.


**Returns:**
java.util.Date - L'ora di inizio dell'indicizzazione.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Restituisce l'ora di fine dell'indicizzazione.


**Returns:**
java.util.Date - L'ora di fine dell'indicizzazione.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Restituisce la durata dell'indicizzazione in secondi.


**Returns:**
double - La durata dell'indicizzazione in secondi.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Restituisce l'elenco degli errori.


**Returns:**
java.lang.String[] - L'elenco degli errori.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Restituisce l'elenco dei documenti indicizzati.


**Returns:**
java.lang.String[] - L'elenco dei documenti indicizzati.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Restituisce l'elenco dei documenti aggiornati.


**Returns:**
java.lang.String[] - L'elenco dei documenti aggiornati.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Restituisce l'elenco dei documenti rimossi dall'indice.


**Returns:**
java.lang.String[] - L'elenco dei documenti rimossi dall'indice.

