---
title: "DocumentStatus"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el estado de procesamiento de un documento."
type: docs
weight: 40
url: /es/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Representa el estado de procesamiento de un documento.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Documento indexado con éxito. |
|
|  | [Skipped](#Skipped) | Documento omitido. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Se produjo un error durante la indexación del documento. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Documento indexado con éxito.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Documento omitido.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Se produjo un error durante la indexación del documento.


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
