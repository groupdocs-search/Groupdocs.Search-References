---
title: "OperationProgressEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de actualización del progreso de la operación de indexado."
type: docs
weight: 18
url: /es/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento de actualización del progreso de la operación de indexado.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Obtiene el número total de documentos para procesar. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Obtiene el número de documentos procesados con éxito. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Obtiene el número de documentos omitidos. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Obtiene el porcentaje del progreso. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Obtiene la clave del último documento procesado. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Obtiene la ruta del último documento procesado. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Obtiene el estado del último documento procesado. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Obtiene el número total de documentos para procesar.


**Returns:**
int - El número total de documentos para procesar.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Obtiene el número de documentos procesados con éxito.


**Returns:**
int - El número de documentos procesados con éxito.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Obtiene el número de documentos omitidos.


**Returns:**
int - El número de documentos omitidos.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Obtiene el porcentaje del progreso.


**Returns:**
double - El porcentaje del progreso.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Obtiene la clave del último documento procesado.


**Returns:**
java.lang.String - La clave del último documento procesado.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Obtiene la ruta del último documento procesado.


**Returns:**
java.lang.String - La ruta del último documento procesado.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Obtiene el estado del último documento procesado.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

