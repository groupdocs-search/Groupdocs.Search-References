---
title: "SearchReport"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt gedetailleerde informatie over een zoekoperatie voor."
type: docs
weight: 30
url: /nl/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Stelt gedetailleerde informatie over een zoekoperatie voor.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Het voorbeeld toont een typisch gebruik van de klasse.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Een index maken in de opgegeven map
Index index = new Index(indexFolder);
// Documenten indexeren vanuit de opgegeven map
index.add(documentsFolder);
// Zoeken in index
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Ophalen van zoekrapporten
SearchReport[] reports = index.getSearchReports();
// Rapporten afdrukken naar de console
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Haalt de starttijd van de zoekopdracht op. |
|
|  | [getEndTime()](#getEndTime--) | Haalt de eindtijd van de zoekopdracht op. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Haalt de zoekduur in seconden op. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Haalt het aantal gevonden documenten op. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Haalt het totale aantal gevonden voorkomens op. |
|
|  | [getTextQuery()](#getTextQuery--) | Haalt de zoekopdracht op in tekstvorm. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Haalt de zoekopdracht op in objectvorm. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Haalt de zoekopties op. |
|
|  | [toString()](#toString--) | Retourneert een String die de huidige SearchReport vertegenwoordigt. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Haalt de zoekopdracht op in tekstvorm.


**Returns:**
java.lang.String - De zoekopdracht in tekstvorm.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Haalt de zoekopdracht op in objectvorm.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Haalt de zoekopties op.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Retourneert een String die de huidige SearchReport vertegenwoordigt.


**Returns:**
java.lang.String - Een string die de huidige SearchReport vertegenwoordigt.

