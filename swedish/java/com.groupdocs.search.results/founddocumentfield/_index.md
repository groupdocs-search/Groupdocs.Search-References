---
title: "FoundDocumentField"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett hittat dokumentfält."
type: docs
weight: 15
url: /sv/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Representerar ett hittat dokumentfält.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Hämtar fältnamnet. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Hämtar antalet förekomster som hittades. |
|
|  | [getTerms()](#getTerms--) | Hämtar de hittade termerna. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Hämtar förekomsterna av de hittade termerna. |
|
|  | [getTermSequences()](#getTermSequences--) | Hämtar de hittade termsekvenserna. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Hämtar förekomsterna av de hittade termsekvenserna. |
|
|  | [toString()](#toString--) | Returnerar en strängrepresentation av det hittade dokumentfältet. |
|
|  | [serialize()](#serialize--) | Serialiserar den aktuella instansen till en bytearray. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiserar en instans från en bytearray. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Hämtar fältnamnet.


**Returns:**
java.lang.String - Fältnamnet.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Hämtar antalet förekomster som hittades.


**Returns:**
int - Antalet förekomster som hittades.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Hämtar de hittade termerna.


**Returns:**
java.lang.String[] - De hittade termerna.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Hämtar förekomsterna av de hittade termerna.


**Returns:**
int[] - Förekomsterna av de hittade termerna.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Hämtar de hittade termsekvenserna.


**Returns:**
java.lang.String[][] - De hittade termsekvenserna.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Hämtar förekomsterna av de hittade termsekvenserna.


**Returns:**
int[] - Förekomsterna av de hittade termsekvenserna.

### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en strängrepresentation av det hittade dokumentfältet.


**Returns:**
java.lang.String - En sträng som representerar det hittade dokumentfältet.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialiserar den aktuella instansen till en bytearray.


**Returns:**
byte[] - En bytearray som representerar den aktuella instansen.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Deserialiserar en instans från en bytearray.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | array | byte[] | En bytearray att deserialisera från. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

