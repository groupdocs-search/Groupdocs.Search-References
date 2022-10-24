---
title: FoundDocument
second_title: GroupDocs.Search for Java API Reference
description: Represents a found document.
type: docs
weight: 14
url: /java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public class FoundDocument
```

Represents a found document.

**Learn more**

 *  [Search results][]


[Search results]: https://docs.groupdocs.com/display/searchjava/Search+results
## Methods

| Method | Description |
| --- | --- |
| [getDocumentInfo()](#getDocumentInfo--) | Gets the document info. |
| [getRelevance()](#getRelevance--) | Gets the relevance of search result. |
| [getOccurrenceCount()](#getOccurrenceCount--) | Gets the number of occurrences found. |
| [getFoundFields()](#getFoundFields--) | Gets the document fields found. |
| [getTerms()](#getTerms--) | Gets the terms found. |
| [getTermSequences()](#getTermSequences--) | Gets the term sequences found. |
| [toString()](#toString--) | Returns string representation of the found document. |
| [serialize()](#serialize--) | Serializes the current instance to a byte array. |
| [deserialize(byte[] array)](#deserialize-byte---) | Deserializes an instance from a byte array. |
### getDocumentInfo() {#getDocumentInfo--}
```
public final DocumentInfo getDocumentInfo()
```


Gets the document info.

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.
### getRelevance() {#getRelevance--}
```
public final double getRelevance()
```


Gets the relevance of search result.

**Returns:**
double - The relevance of search result.
### getOccurrenceCount() {#getOccurrenceCount--}
```
public final int getOccurrenceCount()
```


Gets the number of occurrences found.

**Returns:**
int - The number of occurrences found.
### getFoundFields() {#getFoundFields--}
```
public final FoundDocumentField[] getFoundFields()
```


Gets the document fields found.

**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - The document fields found.
### getTerms() {#getTerms--}
```
public final String[] getTerms()
```


Gets the terms found. The value is evaluated each time the property is accessed.

**Returns:**
java.lang.String[] - The terms found.
### getTermSequences() {#getTermSequences--}
```
public final String[][] getTermSequences()
```


Gets the term sequences found.

**Returns:**
java.lang.String[][] - The term sequences found.
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the found document.

**Returns:**
java.lang.String - A string that represents the found document.
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serializes the current instance to a byte array.

**Returns:**
byte[] - A byte array representing the current instance.
### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Deserializes an instance from a byte array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | byte[] | A byte array to deserialize from. |

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.
