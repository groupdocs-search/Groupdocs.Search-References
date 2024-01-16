---
title: SearchReport
second_title: GroupDocs.Search for Java API Reference
description: Represents a detailed information on a search operation.
type: docs
weight: 30
url: /java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Represents a detailed information on a search operation.

**Learn more**

 *  [Search reports][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Searching in index
 SearchResult result1 = index.search("Einstein");
 SearchResult result2 = index.search("\"Theory of Relativity\"");
 // Getting search reports
 SearchReport[] reports = index.getSearchReports();
 // Printing reports to the console
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


[Search reports]: https://docs.groupdocs.com/display/searchjava/Search+reports
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getStartTime()](#getStartTime--) | Gets the start time of the search. |
| [getEndTime()](#getEndTime--) | Gets the end time of the search. |
| [getSearchDuration()](#getSearchDuration--) | Gets the search duration in seconds. |
| [getDocumentCount()](#getDocumentCount--) | Gets the number of documents found. |
| [getOccurrenceCount()](#getOccurrenceCount--) | Gets the total number of occurrences found. |
| [getTextQuery()](#getTextQuery--) | Gets the search query in text form. |
| [getObjectQuery()](#getObjectQuery--) | Gets the search query in object form. |
| [getSearchOptions()](#getSearchOptions--) | Gets the search options. |
| [toString()](#toString--) | Returns a String that represents the current  SearchReport . |
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Gets the start time of the search.

**Returns:**
java.util.Date - The start time of the search.
### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Gets the end time of the search.

**Returns:**
java.util.Date - The end time of the search.
### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Gets the search duration in seconds.

**Returns:**
double - The search duration in seconds.
### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Gets the number of documents found.

**Returns:**
int - The number of documents found.
### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Gets the total number of occurrences found.

**Returns:**
int - The total number of occurrences found.
### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Gets the search query in text form.

**Returns:**
java.lang.String - The search query in text form.
### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Gets the search query in object form.

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.
### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Gets the search options.

**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.
### toString() {#toString--}
```
public abstract String toString()
```


Returns a String that represents the current  SearchReport .

**Returns:**
java.lang.String - A String that represents the current  SearchReport .
