---
title: "SearchResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un resultado de búsqueda que coincide con una consulta de búsqueda."
type: docs
weight: 19
url: /es/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Representa un resultado de búsqueda que coincide con una consulta de búsqueda.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Creando un índice
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentFolder);
// Configurando opciones de búsqueda
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Habilitando la búsqueda difusa
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Configurando el número máximo de diferencias a 3
// Buscar documentos que contengan la palabra 'Einstein' o la frase 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Imprimiendo el resultado
System.out.println("Documentos: " + result.getDocumentCount());
System.out.println("Ocurrencias totales: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocumento: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOcurrencias: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tCampo: " + field.getFieldName());
System.out.println("\t\tOcurrencias: " + document.getOccurrenceCount());
// Imprimiendo términos encontrados
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Imprimiendo frases encontradas
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Obtiene el número de documentos encontrados. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtiene el número total de ocurrencias encontradas. |
|
|  | [getTruncated()](#getTruncated--) | Obtiene un valor que indica que el resultado está truncado. |
|
|  | [getWarnings()](#getWarnings--) | Obtiene una advertencia que describe el resultado. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Obtiene un token de búsqueda de fragmento para buscar el siguiente fragmento. |
|
|  | [getStartTime()](#getStartTime--) | Obtiene la hora de inicio de la búsqueda. |
|
|  | [getEndTime()](#getEndTime--) | Obtiene la hora de finalización de la búsqueda. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Obtiene la duración de la búsqueda en segundos. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Obtiene el documento encontrado por índice. |
|
|  | [iterator()](#iterator--) | Devuelve un iterador que recorre la colección de los documentos encontrados. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Obtiene el número de documentos encontrados.


**Returns:**
int - El número de documentos encontrados.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtiene el número total de ocurrencias encontradas.


**Returns:**
int - El número total de ocurrencias encontradas.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Obtiene un valor que indica que el resultado está truncado.


**Returns:**
boolean - Un valor que indica que el resultado está truncado.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Obtiene una advertencia que describe el resultado.


**Returns:**
java.lang.String - Una advertencia que describe el resultado.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Obtiene un token de búsqueda de fragmento para buscar el siguiente fragmento.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Obtiene la hora de inicio de la búsqueda.


**Returns:**
java.util.Date - La hora de inicio de la búsqueda.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Obtiene la hora de finalización de la búsqueda.


**Returns:**
java.util.Date - La hora de finalización de la búsqueda.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Obtiene la duración de la búsqueda en segundos.


**Returns:**
double - La duración de la búsqueda en segundos.

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Obtiene el documento encontrado por índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | índice | int | El índice de un documento encontrado. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Devuelve un iterador que recorre la colección de los documentos encontrados.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Un iterador que puede usarse para iterar a través de la colección de los documentos encontrados.

