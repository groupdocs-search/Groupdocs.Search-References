---
title: FoundDocumentField
second_title: GroupDocs.Search for Java API Reference
description: Represents a found document field.
type: docs
weight: 15
url: /java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public class FoundDocumentField
```

Represents a found document field.

**Learn more**

 *  [Search results][]


[Search results]: https://docs.groupdocs.com/display/searchjava/Search+results
## Methods

| Method | Description |
| --- | --- |
| [getFieldName()](#getFieldName--) | Gets the field name. |
| [getOccurrenceCount()](#getOccurrenceCount--) | Gets the number of occurrences found. |
| [getTerms()](#getTerms--) | Gets the terms found. |
| [getTermsOccurrences()](#getTermsOccurrences--) | Gets the occurrences of the found terms. |
| [getTermSequences()](#getTermSequences--) | Gets the term sequences found. |
| [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Gets the occurrences of the found term sequences. |
| [toString()](#toString--) | Returns string representation of the found document field. |
| [getTermSequencePositions()](#getTermSequencePositions--) | Gets the found term sequence positions. |
| [serialize()](#serialize--) | Serializes the current instance to a byte array. |
| [deserialize(byte[] array)](#deserialize-byte---) | Deserializes an instance from a byte array. |
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the field name.

**Returns:**
java.lang.String - The field name.
### getOccurrenceCount() {#getOccurrenceCount--}
```
public final int getOccurrenceCount()
```


Gets the number of occurrences found.

**Returns:**
int - The number of occurrences found.
### getTerms() {#getTerms--}
```
public final String[] getTerms()
```


Gets the terms found.

**Returns:**
java.lang.String[] - The terms found.
### getTermsOccurrences() {#getTermsOccurrences--}
```
public final int[] getTermsOccurrences()
```


Gets the occurrences of the found terms.

**Returns:**
int[] - The occurrences of the found terms.
### getTermSequences() {#getTermSequences--}
```
public final String[][] getTermSequences()
```


Gets the term sequences found.

**Returns:**
java.lang.String[][] - The term sequences found.
### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public final int[] getTermSequencesOccurrences()
```


Gets the occurrences of the found term sequences.

**Returns:**
int[] - The occurrences of the found term sequences.
### toString() {#toString--}
```
public String toString()
```


Returns string representation of the found document field.

**Returns:**
java.lang.String - A string that represents the found document field.
### getTermSequencePositions() {#getTermSequencePositions--}
```
public final int[][] getTermSequencePositions()
```


Gets the found term sequence positions.

**Returns:**
int[][] - The found term sequence positions.
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serializes the current instance to a byte array.

**Returns:**
byte[] - A byte array representing the current instance.
### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Deserializes an instance from a byte array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | byte[] | A byte array to deserialize from. |

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.
