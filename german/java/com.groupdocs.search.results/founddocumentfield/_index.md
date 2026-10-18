---
title: "FoundDocumentField"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein gefundenes Dokumentsfeld dar."
type: docs
weight: 15
url: /de/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Stellt ein gefundenes Dokumentsfeld dar.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Liefert den Feldnamen. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Liefert die Anzahl der gefundenen Vorkommen. |
|
|  | [getTerms()](#getTerms--) | Liefert die gefundenen Begriffe. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Liefert die Vorkommen der gefundenen Begriffe. |
|
|  | [getTermSequences()](#getTermSequences--) | Liefert die gefundenen Begriffsequenzen. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Liefert die Vorkommen der gefundenen Begriffsequenzen. |
|
|  | [toString()](#toString--) | Gibt die String‑Repräsentation des gefundenen Dokumentfeldes zurück. |
|
|  | [serialize()](#serialize--) | Serialisiert die aktuelle Instanz in ein Byte-Array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialisiert eine Instanz aus einem Byte-Array. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Liefert den Feldnamen.


**Returns:**
java.lang.String - Der Feldname.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Liefert die Anzahl der gefundenen Vorkommen.


**Returns:**
int - Die Anzahl der gefundenen Vorkommen.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Liefert die gefundenen Begriffe.


**Returns:**
java.lang.String[] - Die gefundenen Begriffe.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Liefert die Vorkommen der gefundenen Begriffe.


**Returns:**
int[] - Die Vorkommen der gefundenen Begriffe.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Liefert die gefundenen Begriffsequenzen.


**Returns:**
java.lang.String[][] - Die gefundenen Begriffsequenzen.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Liefert die Vorkommen der gefundenen Begriffsequenzen.


**Returns:**
int[] - Die Vorkommen der gefundenen Begriffsequenzen.

### toString() {#toString--}
```
public abstract String toString()
```


Gibt die String‑Repräsentation des gefundenen Dokumentfeldes zurück.


**Returns:**
java.lang.String - Ein String, der das gefundene Dokumentfeld repräsentiert.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialisiert die aktuelle Instanz in ein Byte-Array.


**Returns:**
byte[] – Ein Byte-Array, das die aktuelle Instanz darstellt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Deserialisiert eine Instanz aus einem Byte-Array.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Array | byte[] | Ein Byte-Array, aus dem deserialisiert werden soll. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

