---
title: "IndexingReport"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa información detallada sobre una operación de indexación."
type: docs
weight: 25
url: /es/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Representa información detallada sobre una operación de indexación.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


El ejemplo muestra un uso típico de la clase.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Creando un índice en la carpeta especificada
Index index = new Index(indexFolder);
// Indexando documentos
index.add(documentsFolder1);
index.add(documentsFolder2);
// Obtención de informes de indexación
IndexingReport[] reports = index.getIndexingReports();
// Imprimiendo informes en la consola
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Constructores

| Constructor | Descripción |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Obtiene el número total de documentos en el índice. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Obtiene el número total de términos en el índice. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Obtiene la longitud total de los documentos indexados en MB. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Obtiene el número de segmentos del índice. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Obtiene el tamaño total del índice en bytes. |
|
|  | [getStartTime()](#getStartTime--) | Obtiene la hora de inicio de la indexación. |
|
|  | [getEndTime()](#getEndTime--) | Obtiene la hora de finalización de la indexación. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Obtiene la duración de la indexación en segundos. |
|
|  | [getErrors()](#getErrors--) | Obtiene la lista de errores. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Obtiene la lista de documentos indexados. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Obtiene la lista de documentos actualizados. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Obtiene la lista de documentos eliminados del índice. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Obtiene el número total de documentos en el índice.


**Returns:**
int - El número total de documentos en el índice.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Obtiene el número total de términos en el índice.


**Returns:**
int - El número total de términos en el índice.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Obtiene la longitud total de los documentos indexados en MB.


**Returns:**
double - La longitud total de los documentos indexados en MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Obtiene el número de segmentos del índice.


**Returns:**
int - El número de segmentos del índice.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Obtiene el tamaño total del índice en bytes.


**Returns:**
long - El tamaño total del índice en bytes.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Obtiene la hora de inicio de la indexación.


**Returns:**
java.util.Date - La hora de inicio de la indexación.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Obtiene la hora de finalización de la indexación.


**Returns:**
java.util.Date - La hora de finalización de la indexación.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Obtiene la duración de la indexación en segundos.


**Returns:**
double - La duración de la indexación en segundos.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Obtiene la lista de errores.


**Returns:**
java.lang.String[] - La lista de errores.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Obtiene la lista de documentos indexados.


**Returns:**
java.lang.String[] - La lista de documentos indexados.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Obtiene la lista de documentos actualizados.


**Returns:**
java.lang.String[] - La lista de documentos actualizados.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Obtiene la lista de documentos eliminados del índice.


**Returns:**
java.lang.String[] - La lista de documentos eliminados del índice.

