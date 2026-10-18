---
title: "DocumentStatus"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett dokumentbearbetningsstatus."
type: docs
weight: 40
url: /sv/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Representerar ett dokumentbearbetningsstatus.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Dokumentet har indexerats framgångsrikt. |
|
|  | [Skipped](#Skipped) | Dokumentet har hoppats över. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Ett fel inträffade under dokumentindexering. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Dokumentet har indexerats framgångsrikt.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Dokumentet har hoppats över.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Ett fel inträffade under dokumentindexering.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
