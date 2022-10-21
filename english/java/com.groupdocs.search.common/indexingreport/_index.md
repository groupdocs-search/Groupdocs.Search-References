---
title: IndexingReport
second_title: GroupDocs.Search for Java API Reference
description: Represents a detailed information on an indexing operation.
type: docs
weight: 27
url: /java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public class IndexingReport
```

Represents a detailed information on an indexing operation.

**Learn more**

 *  [Indexing reports][]

The example demonstrates a typical usage of the class.

```
String indexFolder = "c:\\MyIndex\\";
 String documentsFolder1 = "c:\\MyDocuments1\\";
 String documentsFolder2 = "c:\\MyDocuments2\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents
 index.add(documentsFolder1);
 index.add(documentsFolder2);
 // Getting indexing reports
 IndexingReport[] reports = index.getIndexingReports();
 // Printing reports to the console
 for (IndexingReport report : reports)
 {
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


[Indexing reports]: https://docs.groupdocs.com/display/searchjava/Indexing+reports
## Methods

| Method | Description |
| --- | --- |
| [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Gets the total number of documents in the index. |
| [getTotalTermCount()](#getTotalTermCount--) | Gets the total number of terms in index. |
| [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Gets the total length of indexed documents in MB. |
| [getSegmentCount()](#getSegmentCount--) | Gets the number of index segments. |
| [getTotalIndexSize()](#getTotalIndexSize--) | Gets the total index size in bytes. |
| [getStartTime()](#getStartTime--) | Gets the indexing start time. |
| [getEndTime()](#getEndTime--) | Gets the indexing end time. |
| [getIndexingTime()](#getIndexingTime--) | Gets the indexing duration in seconds. |
| [getErrors()](#getErrors--) | Gets the list of errors. |
| [getIndexedDocuments()](#getIndexedDocuments--) | Gets the list of indexed documents. |
| [getUpdatedDocuments()](#getUpdatedDocuments--) | Gets the list of updated documents. |
| [getRemovedDocuments()](#getRemovedDocuments--) | Gets the list of removed from index documents. |
### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public final int getTotalDocumentsInIndex()
```


Gets the total number of documents in the index.

**Returns:**
int - The total number of documents in the index.
### getTotalTermCount() {#getTotalTermCount--}
```
public final int getTotalTermCount()
```


Gets the total number of terms in index.

**Returns:**
int - The total number of terms in index.
### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public final double getIndexedDocumentsSize()
```


Gets the total length of indexed documents in MB.

**Returns:**
double - The total length of indexed documents in MB.
### getSegmentCount() {#getSegmentCount--}
```
public final int getSegmentCount()
```


Gets the number of index segments.

**Returns:**
int - The number of index segments.
### getTotalIndexSize() {#getTotalIndexSize--}
```
public final long getTotalIndexSize()
```


Gets the total index size in bytes.

**Returns:**
long - The total index size in bytes.
### getStartTime() {#getStartTime--}
```
public final Date getStartTime()
```


Gets the indexing start time.

**Returns:**
java.util.Date - The indexing start time.
### getEndTime() {#getEndTime--}
```
public final Date getEndTime()
```


Gets the indexing end time.

**Returns:**
java.util.Date - The indexing end time.
### getIndexingTime() {#getIndexingTime--}
```
public final double getIndexingTime()
```


Gets the indexing duration in seconds.

**Returns:**
double - The indexing duration in seconds.
### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Gets the list of errors.

**Returns:**
java.lang.String[] - The list of errors.
### getIndexedDocuments() {#getIndexedDocuments--}
```
public final String[] getIndexedDocuments()
```


Gets the list of indexed documents.

**Returns:**
java.lang.String[] - The list of indexed documents.
### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public final String[] getUpdatedDocuments()
```


Gets the list of updated documents.

**Returns:**
java.lang.String[] - The list of updated documents.
### getRemovedDocuments() {#getRemovedDocuments--}
```
public final String[] getRemovedDocuments()
```


Gets the list of removed from index documents.

**Returns:**
java.lang.String[] - The list of removed from index documents.
