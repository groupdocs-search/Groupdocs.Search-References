---
title: "DocumentStatus"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een documentverwerkingsstatus voor."
type: docs
weight: 40
url: /nl/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Stelt een documentverwerkingsstatus voor.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Document succesvol geïndexeerd. |
|
|  | [Skipped](#Skipped) | Document overgeslagen. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Fout opgetreden tijdens het indexeren van het document. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Document succesvol geïndexeerd.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Document overgeslagen.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Fout opgetreden tijdens het indexeren van het document.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
