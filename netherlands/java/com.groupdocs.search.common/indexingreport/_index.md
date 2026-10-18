---
title: "IndexingReport"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt gedetailleerde informatie over een indexeerbewerking voor."
type: docs
weight: 25
url: /nl/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Stelt gedetailleerde informatie over een indexeerbewerking voor.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren
index.add(documentsFolder1);
index.add(documentsFolder2);
// Ophalen van indexeer-rapporten
IndexingReport[] reports = index.getIndexingReports();
// Rapporten afdrukken naar de console
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Haalt het totale aantal documenten in de index op. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Haalt het totale aantal termen in de index op. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Haalt de totale lengte van geïndexeerde documenten in MB op. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Haalt het aantal indexsegmenten op. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Haalt de totale indexgrootte in bytes op. |
|
|  | [getStartTime()](#getStartTime--) | Haalt de starttijd van het indexeren op. |
|
|  | [getEndTime()](#getEndTime--) | Haalt de eindtijd van het indexeren op. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Haalt de duur van het indexeren in seconden op. |
|
|  | [getErrors()](#getErrors--) | Haalt de lijst met fouten op. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Haalt de lijst met geïndexeerde documenten op. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Haalt de lijst met bijgewerkte documenten op. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Haalt de lijst met uit de index verwijderde documenten op. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Haalt het totale aantal documenten in de index op.


**Returns:**
int - Het totale aantal documenten in de index.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Haalt het totale aantal termen in de index op.


**Returns:**
int - Het totale aantal termen in de index.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Haalt de totale lengte van geïndexeerde documenten in MB op.


**Returns:**
double - De totale lengte van geïndexeerde documenten in MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Haalt het aantal indexsegmenten op.


**Returns:**
int - Het aantal indexsegmenten.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Haalt de totale indexgrootte in bytes op.


**Returns:**
long - De totale indexgrootte in bytes.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Haalt de starttijd van het indexeren op.


**Returns:**
java.util.Date - De starttijd van het indexeren.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Haalt de eindtijd van het indexeren op.


**Returns:**
java.util.Date - De eindtijd van het indexeren.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Haalt de duur van het indexeren in seconden op.


**Returns:**
double - De duur van het indexeren in seconden.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Haalt de lijst met fouten op.


**Returns:**
java.lang.String[] - De lijst met fouten.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Haalt de lijst met geïndexeerde documenten op.


**Returns:**
java.lang.String[] - De lijst met geïndexeerde documenten.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Haalt de lijst met bijgewerkte documenten op.


**Returns:**
java.lang.String[] - De lijst met bijgewerkte documenten.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Haalt de lijst met uit de index verwijderde documenten op.


**Returns:**
java.lang.String[] - De lijst met uit de index verwijderde documenten.

