---
title: "FoundDocumentField"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un campo de documento encontrado."
type: docs
weight: 15
url: /es/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Representa un campo de documento encontrado.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Obtiene el nombre del campo. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtiene el número de ocurrencias encontradas. |
|
|  | [getTerms()](#getTerms--) | Obtiene los términos encontrados. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Obtiene las ocurrencias de los términos encontrados. |
|
|  | [getTermSequences()](#getTermSequences--) | Obtiene las secuencias de términos encontradas. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Obtiene las ocurrencias de las secuencias de términos encontradas. |
|
|  | [toString()](#toString--) | Devuelve la representación en cadena del campo de documento encontrado. |
|
|  | [serialize()](#serialize--) | Serializa la instancia actual a una matriz de bytes. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializa una instancia a partir de una matriz de bytes. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Obtiene el nombre del campo.


**Returns:**
java.lang.String - El nombre del campo.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtiene el número de ocurrencias encontradas.


**Returns:**
int - El número de ocurrencias encontradas.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Obtiene los términos encontrados.


**Returns:**
java.lang.String[] - Los términos encontrados.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Obtiene las ocurrencias de los términos encontrados.


**Returns:**
int[] - Las ocurrencias de los términos encontrados.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Obtiene las secuencias de términos encontradas.


**Returns:**
java.lang.String[][] - Las secuencias de términos encontradas.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Obtiene las ocurrencias de las secuencias de términos encontradas.


**Returns:**
int[] - Las ocurrencias de las secuencias de términos encontradas.

### toString() {#toString--}
```
public abstract String toString()
```


Devuelve la representación en cadena del campo de documento encontrado.


**Returns:**
java.lang.String - Una cadena que representa el campo de documento encontrado.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serializa la instancia actual a una matriz de bytes.


**Returns:**
byte[] - Una matriz de bytes que representa la instancia actual.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Deserializa una instancia a partir de una matriz de bytes.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matriz | byte[] | Una matriz de bytes desde la cual deserializar. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

