---
title: "FoundDocument"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett hittat dokument."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Representerar ett hittat dokument.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Hämtar dokumentinformationen. |
|
|  | [getRelevance()](#getRelevance--) | Hämtar relevansen för sökresultatet. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Hämtar antalet förekomster som hittades. |
|
|  | [getFoundFields()](#getFoundFields--) | Hämtar de hittade dokumentfälten. |
|
|  | [getTerms()](#getTerms--) | Hämtar de hittade termerna. |
|
|  | [getTermSequences()](#getTermSequences--) | Hämtar de hittade termsekvenserna. |
|
|  | [getAttributes()](#getAttributes--) | Hämtar attributen som är associerade med det hittade dokumentet. |
|
|  | [toString()](#toString--) | Returnerar strängrepresentation av det hittade dokumentet. |
|
|  | [serialize()](#serialize--) | Serialiserar den aktuella instansen till en bytearray. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiserar en instans från en bytearray. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Hämtar dokumentinformationen.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Hämtar relevansen för sökresultatet.


**Returns:**
double - Relevansen för sökresultatet.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Hämtar antalet förekomster som hittades.


**Returns:**
int - Antalet förekomster som hittades.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Hämtar de hittade dokumentfälten.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - De hittade dokumentfälten.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Hämtar de hittade termerna. Värdet utvärderas varje gång egenskapen nås.


**Returns:**
java.lang.String[] - De hittade termerna.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Hämtar de hittade termsekvenserna.


**Returns:**
java.lang.String[][] - De hittade termsekvenserna.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Hämtar attributen som är associerade med det hittade dokumentet. Det motsvarande alternativet måste vara aktiverat i sökalternativen för att hämta attribut.


**Returns:**
java.lang.String[] - Attributen som är associerade med det hittade dokumentet.

### toString() {#toString--}
```
public abstract String toString()
```


Returnerar strängrepresentation av det hittade dokumentet.


**Returns:**
java.lang.String - En sträng som representerar det hittade dokumentet.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialiserar den aktuella instansen till en bytearray.


**Returns:**
byte[] - En bytearray som representerar den aktuella instansen.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Deserialiserar en instans från en bytearray.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | array | byte[] | En bytearray att deserialisera från. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

