---
title: "FoundDocumentField"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un campo di documento trovato."
type: docs
weight: 15
url: /it/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Rappresenta un campo di documento trovato.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Restituisce il nome del campo. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ottiene il numero di occorrenze trovate. |
|
|  | [getTerms()](#getTerms--) | Ottiene i termini trovati. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Ottiene le occorrenze dei termini trovati. |
|
|  | [getTermSequences()](#getTermSequences--) | Ottiene le sequenze di termini trovate. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Ottiene le occorrenze delle sequenze di termini trovate. |
|
|  | [toString()](#toString--) | Restituisce la rappresentazione stringa del campo del documento trovato. |
|
|  | [serialize()](#serialize--) | Serializza l'istanza corrente in un array di byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializza un'istanza da un array di byte. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Restituisce il nome del campo.


**Returns:**
java.lang.String - Il nome del campo.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Ottiene il numero di occorrenze trovate.


**Returns:**
int - Il numero di occorrenze trovate.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Ottiene i termini trovati.


**Returns:**
java.lang.String[] - I termini trovati.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Ottiene le occorrenze dei termini trovati.


**Returns:**
int[] - Le occorrenze dei termini trovati.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Ottiene le sequenze di termini trovate.


**Returns:**
java.lang.String[][] - Le sequenze di termini trovate.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Ottiene le occorrenze delle sequenze di termini trovate.


**Returns:**
int[] - Le occorrenze delle sequenze di termini trovate.

### toString() {#toString--}
```
public abstract String toString()
```


Restituisce la rappresentazione stringa del campo del documento trovato.


**Returns:**
java.lang.String - Una stringa che rappresenta il campo del documento trovato.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serializza l'istanza corrente in un array di byte.


**Returns:**
byte[] - Un array di byte che rappresenta l'istanza corrente.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Deserializza un'istanza da un array di byte.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | array | byte[] | Un array di byte da cui deserializzare. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

