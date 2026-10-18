---
title: "SearchReport"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar detaljerad information om en sökoperation."
type: docs
weight: 30
url: /sv/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Representerar detaljerad information om en sökoperation.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Exemplet demonstrerar ett typiskt användningssätt av klassen.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Skapar ett index i den angivna mappen
Index index = new Index(indexFolder);
// Indexerar dokument från den angivna mappen
index.add(documentsFolder);
// Söker i indexet
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Hämtar sökrapporter
SearchReport[] reports = index.getSearchReports();
// Skriver ut rapporter till konsolen
for (SearchReport report : reports) {
System.out.println("Fråga: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Varaktighet: " + report.getSearchDuration());
System.out.println("Dokument: " + report.getDocumentCount());
System.out.println("Förekomster: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Hämtar starttiden för sökningen. |
|
|  | [getEndTime()](#getEndTime--) | Hämtar sluttiden för sökningen. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Hämtar sökvaraktigheten i sekunder. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Hämtar antalet hittade dokument. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Hämtar det totala antalet hittade förekomster. |
|
|  | [getTextQuery()](#getTextQuery--) | Hämtar sökfrågan i textform. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Hämtar sökfrågan i objektform. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Hämtar sökalternativen. |
|
|  | [toString()](#toString--) | Returnerar en String som representerar den aktuella SearchReport. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Hämtar sökfrågan i textform.


**Returns:**
java.lang.String - Sökfrågan i textform.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Hämtar sökfrågan i objektform.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Hämtar sökalternativen.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en String som representerar den aktuella SearchReport.


**Returns:**
java.lang.String - En sträng som representerar den aktuella SearchReport.

