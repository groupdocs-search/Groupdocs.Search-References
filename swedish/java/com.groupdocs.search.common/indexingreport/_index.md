---
title: "IndexingReport"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar detaljerad information om en indexeringsoperation."
type: docs
weight: 25
url: /sv/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Representerar detaljerad information om en indexeringsoperation.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument
index.add(documentsFolder1);
index.add(documentsFolder2);
// Hämtar indexeringsrapporter
IndexingReport[] reports = index.getIndexingReports();
// Skriver ut rapporter till konsolen
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


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Hämtar det totala antalet dokument i indexet. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Hämtar det totala antalet termer i indexet. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Hämtar den totala längden på indexerade dokument i MB. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Hämtar antalet indexsegment. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Hämtar den totala indexstorleken i byte. |
|
|  | [getStartTime()](#getStartTime--) | Hämtar indexeringens starttid. |
|
|  | [getEndTime()](#getEndTime--) | Hämtar indexeringens sluttid. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Hämtar indexeringens varaktighet i sekunder. |
|
|  | [getErrors()](#getErrors--) | Hämtar listan över fel. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Hämtar listan över indexerade dokument. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Hämtar listan över uppdaterade dokument. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Hämtar listan över dokument som tagits bort från indexet. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Hämtar det totala antalet dokument i indexet.


**Returns:**
int - Det totala antalet dokument i indexet.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Hämtar det totala antalet termer i indexet.


**Returns:**
int - Det totala antalet termer i indexet.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Hämtar den totala längden på indexerade dokument i MB.


**Returns:**
double - Den totala längden på indexerade dokument i MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Hämtar antalet indexsegment.


**Returns:**
int - Antalet indexsegment.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Hämtar den totala indexstorleken i byte.


**Returns:**
long - Den totala indexstorleken i byte.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Hämtar indexeringens starttid.


**Returns:**
java.util.Date - Indexeringens starttid.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Hämtar indexeringens sluttid.


**Returns:**
java.util.Date - Indexeringens sluttid.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Hämtar indexeringens varaktighet i sekunder.


**Returns:**
double - Indexeringens varaktighet i sekunder.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Hämtar listan över fel.


**Returns:**
java.lang.String[] - Listan över fel.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Hämtar listan över indexerade dokument.


**Returns:**
java.lang.String[] - Listan över indexerade dokument.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Hämtar listan över uppdaterade dokument.


**Returns:**
java.lang.String[] - Listan över uppdaterade dokument.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Hämtar listan över dokument som tagits bort från indexet.


**Returns:**
java.lang.String[] - Listan över dokument som tagits bort från indexet.

