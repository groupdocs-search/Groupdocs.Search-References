---
title: "FoundDocumentField"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een gevonden documentveld voor."
type: docs
weight: 15
url: /nl/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Stelt een gevonden documentveld voor.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Haalt de veldnaam op. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Haalt het aantal gevonden voorkomens op. |
|
|  | [getTerms()](#getTerms--) | Haalt de gevonden termen op. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Haalt de voorkomens van de gevonden termen op. |
|
|  | [getTermSequences()](#getTermSequences--) | Haalt de gevonden termreeksen op. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Haalt de voorkomens van de gevonden termreeksen op. |
|
|  | [toString()](#toString--) | Retourneert de tekenreeksrepresentatie van het gevonden documentveld. |
|
|  | [serialize()](#serialize--) | Serialiseert de huidige instantie naar een byte-array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiseert een instantie vanuit een byte-array. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Haalt de veldnaam op.


**Returns:**
java.lang.String - De veldnaam.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Haalt het aantal gevonden voorkomens op.


**Returns:**
int - Het aantal gevonden voorkomens.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Haalt de gevonden termen op.


**Returns:**
java.lang.String[] - De gevonden termen.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Haalt de voorkomens van de gevonden termen op.


**Returns:**
int[] - De voorkomens van de gevonden termen.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Haalt de gevonden termreeksen op.


**Returns:**
java.lang.String[][] - De gevonden termreeksen.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Haalt de voorkomens van de gevonden termreeksen op.


**Returns:**
int[] - De voorkomens van de gevonden termreeksen.

### toString() {#toString--}
```
public abstract String toString()
```


Retourneert de tekenreeksrepresentatie van het gevonden documentveld.


**Returns:**
java.lang.String - Een tekenreeks die het gevonden documentveld vertegenwoordigt.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialiseert de huidige instantie naar een byte-array.


**Returns:**
byte[] - Een byte-array die de huidige instantie vertegenwoordigt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Deserialiseert een instantie vanuit een byte-array.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | array | byte[] | Een byte-array om van te deserialiseren. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

