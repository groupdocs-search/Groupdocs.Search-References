---
title: "DocumentStatus"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un statut de traitement de document."
type: docs
weight: 40
url: /fr/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Représente un statut de traitement de document.

## Fields

| Field | Description |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Document indexé avec succès. |
|
|  | [Skipped](#Skipped) | Document ignoré. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Une erreur s'est produite lors de l'indexation du document. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Document indexé avec succès.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Document ignoré.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Une erreur s'est produite lors de l'indexation du document.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
