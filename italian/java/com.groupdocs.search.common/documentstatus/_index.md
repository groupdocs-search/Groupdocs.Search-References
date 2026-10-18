---
title: "DocumentStatus"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta lo stato di elaborazione di un documento."
type: docs
weight: 40
url: /it/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Rappresenta lo stato di elaborazione di un documento.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Documento indicizzato con successo. |
|
|  | [Skipped](#Skipped) | Documento saltato. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Si è verificato un errore durante l'indicizzazione del documento. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Documento indicizzato con successo.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Documento saltato.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Si è verificato un errore durante l'indicizzazione del documento.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
