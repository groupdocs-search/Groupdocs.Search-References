---
title: "IndexingReport"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt detaillierte Informationen zu einem Indexierungsvorgang dar."
type: docs
weight: 25
url: /de/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Stellt detaillierte Informationen zu einem Indexierungsvorgang dar.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten
index.add(documentsFolder1);
index.add(documentsFolder2);
// Abrufen von Indexierungsberichten
IndexingReport[] reports = index.getIndexingReports();
// Ausgeben der Berichte in die Konsole
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


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Gibt die Gesamtzahl der Dokumente im Index zurück. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Gibt die Gesamtzahl der Begriffe im Index zurück. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Gibt die Gesamtlänge der indizierten Dokumente in MB zurück. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Liefert die Anzahl der Indexsegmente. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Gibt die Gesamtgröße des Index in Bytes zurück. |
|
|  | [getStartTime()](#getStartTime--) | Gibt den Startzeitpunkt der Indexierung zurück. |
|
|  | [getEndTime()](#getEndTime--) | Gibt den Endzeitpunkt der Indexierung zurück. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Gibt die Dauer der Indexierung in Sekunden zurück. |
|
|  | [getErrors()](#getErrors--) | Gibt die Liste der Fehler zurück. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Gibt die Liste der indizierten Dokumente zurück. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Liefert die Liste der aktualisierten Dokumente. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Liefert die Liste der aus dem Index entfernten Dokumente. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Gibt die Gesamtzahl der Dokumente im Index zurück.


**Returns:**
int - Die Gesamtzahl der Dokumente im Index.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Gibt die Gesamtzahl der Begriffe im Index zurück.


**Returns:**
int - Die Gesamtzahl der Terme im Index.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Gibt die Gesamtlänge der indizierten Dokumente in MB zurück.


**Returns:**
double - Die Gesamtlänge der indizierten Dokumente in MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Liefert die Anzahl der Indexsegmente.


**Returns:**
int - Die Anzahl der Indexsegmente.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Gibt die Gesamtgröße des Index in Bytes zurück.


**Returns:**
long - Die gesamte Indexgröße in Bytes.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Gibt den Startzeitpunkt der Indexierung zurück.


**Returns:**
java.util.Date - Der Startzeitpunkt der Indizierung.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Gibt den Endzeitpunkt der Indexierung zurück.


**Returns:**
java.util.Date - Der Endzeitpunkt der Indizierung.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Gibt die Dauer der Indexierung in Sekunden zurück.


**Returns:**
double - Die Dauer der Indizierung in Sekunden.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Gibt die Liste der Fehler zurück.


**Returns:**
java.lang.String[] - Die Liste der Fehler.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Gibt die Liste der indizierten Dokumente zurück.


**Returns:**
java.lang.String[] - Die Liste der indizierten Dokumente.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Liefert die Liste der aktualisierten Dokumente.


**Returns:**
java.lang.String[] - Die Liste der aktualisierten Dokumente.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Liefert die Liste der aus dem Index entfernten Dokumente.


**Returns:**
java.lang.String[] - Die Liste der aus dem Index entfernten Dokumente.

