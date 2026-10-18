---
title: "FoundDocument"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein gefundenes Dokument dar."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Stellt ein gefundenes Dokument dar.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Liefert die Dokumentinformationen. |
|
|  | [getRelevance()](#getRelevance--) | Ermittelt die Relevanz des Suchergebnisses. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Liefert die Anzahl der gefundenen Vorkommen. |
|
|  | [getFoundFields()](#getFoundFields--) | Ermittelt die gefundenen Dokumentfelder. |
|
|  | [getTerms()](#getTerms--) | Liefert die gefundenen Begriffe. |
|
|  | [getTermSequences()](#getTermSequences--) | Liefert die gefundenen Begriffsequenzen. |
|
|  | [getAttributes()](#getAttributes--) | Ermittelt die mit dem gefundenen Dokument verbundenen Attribute. |
|
|  | [toString()](#toString--) | Gibt die String-Darstellung des gefundenen Dokuments zurück. |
|
|  | [serialize()](#serialize--) | Serialisiert die aktuelle Instanz in ein Byte-Array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialisiert eine Instanz aus einem Byte-Array. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Liefert die Dokumentinformationen.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Ermittelt die Relevanz des Suchergebnisses.


**Returns:**
double - Die Relevanz des Suchergebnisses.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Liefert die Anzahl der gefundenen Vorkommen.


**Returns:**
int - Die Anzahl der gefundenen Vorkommen.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Ermittelt die gefundenen Dokumentfelder.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Die gefundenen Dokumentfelder.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Ermittelt die gefundenen Begriffe. Der Wert wird bei jedem Zugriff auf die Eigenschaft ausgewertet.


**Returns:**
java.lang.String[] - Die gefundenen Begriffe.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Liefert die gefundenen Begriffsequenzen.


**Returns:**
java.lang.String[][] - Die gefundenen Begriffsequenzen.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Ermittelt die mit dem gefundenen Dokument verbundenen Attribute. Die entsprechende Option muss in den Suchoptionen aktiviert sein, um Attribute abzurufen.


**Returns:**
java.lang.String[] - Die mit dem gefundenen Dokument verbundenen Attribute.

### toString() {#toString--}
```
public abstract String toString()
```


Gibt die String-Darstellung des gefundenen Dokuments zurück.


**Returns:**
java.lang.String - Ein String, der das gefundene Dokument darstellt.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serialisiert die aktuelle Instanz in ein Byte-Array.


**Returns:**
byte[] – Ein Byte-Array, das die aktuelle Instanz darstellt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Deserialisiert eine Instanz aus einem Byte-Array.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Array | byte[] | Ein Byte-Array, aus dem deserialisiert werden soll. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

