---
title: "SearchReport"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa información detallada sobre una operación de búsqueda."
type: docs
weight: 30
url: /es/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Representa información detallada sobre una operación de búsqueda.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos de la carpeta especificada
index.add(documentsFolder);
// Buscando en el índice
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Obteniendo informes de búsqueda
SearchReport[] reports = index.getSearchReports();
// Imprimiendo informes en la consola
for (SearchReport report : reports) {
System.out.println("Consulta: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duración: " + report.getSearchDuration());
System.out.println("Documentos: " + report.getDocumentCount());
System.out.println("Ocurrencias: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Obtiene la hora de inicio de la búsqueda. |
|
|  | [getEndTime()](#getEndTime--) | Obtiene la hora de finalización de la búsqueda. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Obtiene la duración de la búsqueda en segundos. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Obtiene el número de documentos encontrados. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtiene el número total de ocurrencias encontradas. |
|
|  | [getTextQuery()](#getTextQuery--) | Obtiene la consulta de búsqueda en forma de texto. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Obtiene la consulta de búsqueda en forma de objeto. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Obtiene las opciones de búsqueda. |
|
|  | [toString()](#toString--) | Devuelve una cadena que representa el SearchReport actual. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Obtiene la consulta de búsqueda en forma de texto.


**Returns:**
java.lang.String - La consulta de búsqueda en forma de texto.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Obtiene la consulta de búsqueda en forma de objeto.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Obtiene las opciones de búsqueda.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Devuelve una cadena que representa el SearchReport actual.


**Returns:**
java.lang.String - Una cadena que representa el SearchReport actual.

