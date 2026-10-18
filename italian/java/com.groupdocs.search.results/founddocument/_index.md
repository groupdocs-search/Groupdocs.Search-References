---
title: "FoundDocument"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un documento trovato."
type: docs
weight: 14
url: /it/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Rappresenta un documento trovato.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Ottiene le informazioni del documento. |
|
|  | [getRelevance()](#getRelevance--) | Ottiene la rilevanza del risultato della ricerca. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Ottiene il numero di occorrenze trovate. |
|
|  | [getFoundFields()](#getFoundFields--) | Ottiene i campi del documento trovati. |
|
|  | [getTerms()](#getTerms--) | Ottiene i termini trovati. |
|
|  | [getTermSequences()](#getTermSequences--) | Ottiene le sequenze di termini trovate. |
|
|  | [getAttributes()](#getAttributes--) | Ottiene gli attributi associati al documento trovato. |
|
|  | [toString()](#toString--) | Restituisce la rappresentazione stringa del documento trovato. |
|
|  | [serialize()](#serialize--) | Serializza l'istanza corrente in un array di byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializza un'istanza da un array di byte. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Ottiene le informazioni del documento.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Ottiene la rilevanza del risultato della ricerca.


**Returns:**
double - La rilevanza del risultato della ricerca.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Ottiene il numero di occorrenze trovate.


**Returns:**
int - Il numero di occorrenze trovate.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Ottiene i campi del documento trovati.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - I campi del documento trovati.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Ottiene i termini trovati. Il valore è valutato ogni volta che la proprietà viene acceduta.


**Returns:**
java.lang.String[] - I termini trovati.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Ottiene le sequenze di termini trovate.


**Returns:**
java.lang.String[][] - Le sequenze di termini trovate.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Ottiene gli attributi associati al documento trovato. L'opzione corrispondente deve essere abilitata nelle opzioni di ricerca per recuperare gli attributi.


**Returns:**
java.lang.String[] - Gli attributi associati al documento trovato.

### toString() {#toString--}
```
public abstract String toString()
```


Restituisce la rappresentazione stringa del documento trovato.


**Returns:**
java.lang.String - Una stringa che rappresenta il documento trovato.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serializza l'istanza corrente in un array di byte.


**Returns:**
byte[] - Un array di byte che rappresenta l'istanza corrente.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Deserializza un'istanza da un array di byte.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | array | byte[] | Un array di byte da cui deserializzare. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

