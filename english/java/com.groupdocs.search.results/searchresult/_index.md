---
title: SearchResult
second_title: GroupDocs.Search for Java API Reference
description: Represents a search result matching a search query.
type: docs
weight: 19
url: /java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class SearchResult implements Iterable<FoundDocument>
```

Represents a search result matching a search query.

**Learn more**

 *  [Searching][]
 *  [Search results][]

The example demonstrates a typical usage of the class.

```
String indexFolder = "c:\\MyIndex\\";
 String documentFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentFolder);
 // Setting search options
 SearchOptions options = new SearchOptions();
 options.getFuzzySearch().setEnabled(true); // Enabling the fuzzy search
 options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Setting the maximum number of differences to 3
 // Search for documents containing the word 'Einstein' or the phrase 'Theory of Relativity'
 SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
 // Printing the result
 System.out.println("Documents: " + result.getDocumentCount());
 System.out.println("Total occurrences: " + result.getOccurrenceCount());
 for (int i = 0; i < result.getDocumentCount(); i++)
 {
     FoundDocument document = result.getFoundDocument(i);
     System.out.println("\tDocument: " + document.getDocumentInfo().getFilePath());
     System.out.println("\tOccurrences: " + document.getOccurrenceCount());
     for (int j = 0; j < document.getFoundFields().length; j++)
     {
         FoundDocumentField field = document.getFoundFields()[j];
         System.out.println("\t\tField: " + field.getFieldName());
         System.out.println("\t\tOccurrences: " + document.getOccurrenceCount());
         // Printing found terms
         if (field.getTerms() != null)
         {
             for (int k = 0; k < field.getTerms().length; k++)
             {
                 System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
             }
         }
         // Printing found phrases
         if (field.getTermSequences() != null)
         {
             for (int k = 0; k < field.getTermSequences().length; k++)
             {
                 String[] terms = field.getTermSequences()[k];
                 String sequence = "";
                 for (int m = 0; m < terms.length; m++)
                 {
                     sequence += terms[m] + " ";
                 }
                 System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
             }
         }
     }
 }
```


[Searching]: https://docs.groupdocs.com/display/searchjava/Searching
[Search results]: https://docs.groupdocs.com/display/searchjava/Search+results
## Methods

| Method | Description |
| --- | --- |
| [getDocumentCount()](#getDocumentCount--) | Gets the number of documents found. |
| [getOccurrenceCount()](#getOccurrenceCount--) | Gets the total number of occurrences found. |
| [getTruncated()](#getTruncated--) | Gets a value indicating that the result is truncated. |
| [getWarnings()](#getWarnings--) | Gets a warnings describing the result. |
| [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Gets a chunk search token for searching the next chunk. |
| [getStartTime()](#getStartTime--) | Gets the start time of the search. |
| [getEndTime()](#getEndTime--) | Gets the end time of the search. |
| [getSearchDuration()](#getSearchDuration--) | Gets the search duration in seconds. |
| [getFoundDocument(int index)](#getFoundDocument-int-) | Gets the found document by index. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection of the documents found. |
### getDocumentCount() {#getDocumentCount--}
```
public final int getDocumentCount()
```


Gets the number of documents found.

**Returns:**
int - The number of documents found.
### getOccurrenceCount() {#getOccurrenceCount--}
```
public final int getOccurrenceCount()
```


Gets the total number of occurrences found.

**Returns:**
int - The total number of occurrences found.
### getTruncated() {#getTruncated--}
```
public final boolean getTruncated()
```


Gets a value indicating that the result is truncated.

**Returns:**
boolean - A value indicating that the result is truncated.
### getWarnings() {#getWarnings--}
```
public final String getWarnings()
```


Gets a warnings describing the result.

**Returns:**
java.lang.String - A warnings describing the result.
### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public final ChunkSearchToken getNextChunkSearchToken()
```


Gets a chunk search token for searching the next chunk.

**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.
### getStartTime() {#getStartTime--}
```
public final Date getStartTime()
```


Gets the start time of the search.

**Returns:**
java.util.Date - The start time of the search.
### getEndTime() {#getEndTime--}
```
public final Date getEndTime()
```


Gets the end time of the search.

**Returns:**
java.util.Date - The end time of the search.
### getSearchDuration() {#getSearchDuration--}
```
public final double getSearchDuration()
```


Gets the search duration in seconds.

**Returns:**
double - The search duration in seconds.
### getFoundDocument(int index) {#getFoundDocument-int-}
```
public final FoundDocument getFoundDocument(int index)
```


Gets the found document by index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of a found document. |

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.
### iterator() {#iterator--}
```
public final Iterator<FoundDocument> iterator()
```


Returns an iterator that iterates through the collection of the documents found.

**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - An iterator that can be used to iterate through the collection of the found documents.
