---
title: "FoundDocument"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een gevonden document voor."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Stelt een gevonden document voor.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Haalt de documentinformatie op. |
|
|  | [getRelevance()](#getRelevance--) | Haalt de relevantie van het zoekresultaat op. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Haalt het aantal gevonden voorkomens op. |
|
|  | [getFoundFields()](#getFoundFields--) | Haalt de gevonden documentvelden op. |
|
|  | [getTerms()](#getTerms--) | Haalt de gevonden termen op. |
|
|  | [getTermSequences()](#getTermSequences--) | Haalt de gevonden termreeksen op. |
|
|  | [getAttributes()](#getAttributes--) | Haalt de attributen op die aan het gevonden document zijn gekoppeld. |
|
|  | [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van het gevonden document. |
|
|  | [serialize()](#serialize--) | Serialiseert de huidige instantie naar een byte-array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiseert een instantie vanuit een byte-array. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Haalt de documentinformatie op.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Haalt de relevantie van het zoekresultaat op.


**Returns:**
double - De relevantie van het zoekresultaat.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Haalt het aantal gevonden voorkomens op.


**Returns:**
int - Het aantal gevonden voorkomens.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Haalt de gevonden documentvelden op.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - De gevonden documentvelden.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Haalt de gevonden termen op. De waarde wordt elke keer geëvalueerd wanneer de eigenschap wordt benaderd.


**Returns:**
java.lang.String[] - De gevonden termen.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Haalt de gevonden termreeksen op.


**Returns:**
java.lang.String[][] - De gevonden termreeksen.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Haalt de attributen op die aan het gevonden document zijn gekoppeld. De overeenkomstige optie moet ingeschakeld zijn in de zoekopties om attributen op te halen.


**Returns:**
java.lang.String[] - De attributen die aan het gevonden document zijn gekoppeld.

### toString() {#toString--}
```
public abstract String toString()
```


Retourneert de tekenreeksrepresentatie van het gevonden document.


**Returns:**
java.lang.String - Een tekenreeks die het gevonden document weergeeft.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialiseert de huidige instantie naar een byte-array.


**Returns:**
byte[] - Een byte-array die de huidige instantie vertegenwoordigt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Deserialiseert een instantie vanuit een byte-array.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | array | byte[] | Een byte-array om van te deserialiseren. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

