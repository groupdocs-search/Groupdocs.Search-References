---
title: "SearchReport"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt detaillierte Informationen zu einem Suchvorgang dar."
type: docs
weight: 30
url: /de/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Stellt detaillierte Informationen zu einem Suchvorgang dar.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Das Beispiel demonstriert eine typische Verwendung der Klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Erstellen eines Index im angegebenen Ordner
Index index = new Index(indexFolder);
// Indizieren von Dokumenten aus dem angegebenen Ordner
index.add(documentsFolder);
// Durchsuchen des Index
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Abrufen von Suchberichten
SearchReport[] reports = index.getSearchReports();
// Ausgeben der Berichte in die Konsole
for (SearchReport report : reports) {
System.out.println("Abfrage: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Dauer: " + report.getSearchDuration());
System.out.println("Dokumente: " + report.getDocumentCount());
System.out.println("Vorkommen: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Ermittelt die Startzeit der Suche. |
|
|  | [getEndTime()](#getEndTime--) | Ermittelt die Endzeit der Suche. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Ermittelt die Suchdauer in Sekunden. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Ermittelt die Anzahl gefundener Dokumente. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ermittelt die Gesamtzahl gefundener Vorkommen. |
|
|  | [getTextQuery()](#getTextQuery--) | Ermittelt die Suchabfrage in Textform. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Ermittelt die Suchabfrage in Objektform. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Ermittelt die Suchoptionen. |
|
|  | [toString()](#toString--) | Gibt einen String zurück, der das aktuelle  SearchReport  darstellt. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Ermittelt die Suchabfrage in Textform.


**Returns:**
java.lang.String - Die Suchanfrage in Textform.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Ermittelt die Suchabfrage in Objektform.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Ermittelt die Suchoptionen.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Gibt einen String zurück, der das aktuelle  SearchReport  darstellt.


**Returns:**
java.lang.String - Ein String, der den aktuellen SearchReport darstellt.

