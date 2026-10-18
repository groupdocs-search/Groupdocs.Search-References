---
title: "FoundDocument"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un documento encontrado."
type: docs
weight: 14
url: /es/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Representa un documento encontrado.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtiene la información del documento. |
|
|  | [getRelevance()](#getRelevance--) | Obtiene la relevancia del resultado de búsqueda. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtiene el número de ocurrencias encontradas. |
|
|  | [getFoundFields()](#getFoundFields--) | Obtiene los campos del documento encontrados. |
|
|  | [getTerms()](#getTerms--) | Obtiene los términos encontrados. |
|
|  | [getTermSequences()](#getTermSequences--) | Obtiene las secuencias de términos encontradas. |
|
|  | [getAttributes()](#getAttributes--) | Obtiene los atributos asociados al documento encontrado. |
|
|  | [toString()](#toString--) | Devuelve la representación en cadena del documento encontrado. |
|
|  | [serialize()](#serialize--) | Serializa la instancia actual a una matriz de bytes. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializa una instancia a partir de una matriz de bytes. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Obtiene la información del documento.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Obtiene la relevancia del resultado de búsqueda.


**Returns:**
double - La relevancia del resultado de búsqueda.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtiene el número de ocurrencias encontradas.


**Returns:**
int - El número de ocurrencias encontradas.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Obtiene los campos del documento encontrados.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Los campos del documento encontrados.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Obtiene los términos encontrados. El valor se evalúa cada vez que se accede a la propiedad.


**Returns:**
java.lang.String[] - Los términos encontrados.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Obtiene las secuencias de términos encontradas.


**Returns:**
java.lang.String[][] - Las secuencias de términos encontradas.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Obtiene los atributos asociados al documento encontrado. La opción correspondiente debe estar habilitada en las opciones de búsqueda para recuperar los atributos.


**Returns:**
java.lang.String[] - Los atributos asociados al documento encontrado.

### toString() {#toString--}
```
public abstract String toString()
```


Devuelve la representación en cadena del documento encontrado.


**Returns:**
java.lang.String - Una cadena que representa el documento encontrado.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Serializa la instancia actual a una matriz de bytes.


**Returns:**
byte[] - Una matriz de bytes que representa la instancia actual.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Deserializa una instancia a partir de una matriz de bytes.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matriz | byte[] | Una matriz de bytes desde la cual deserializar. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

