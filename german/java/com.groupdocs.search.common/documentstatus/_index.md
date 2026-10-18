---
title: "DocumentStatus"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Dokumentverarbeitungsstatus dar."
type: docs
weight: 40
url: /de/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Stellt einen Dokumentverarbeitungsstatus dar.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Dokument erfolgreich indiziert. |
|
|  | [Skipped](#Skipped) | Dokument übersprungen. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Fehler beim Indizieren des Dokuments aufgetreten. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Dokument erfolgreich indiziert.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Dokument übersprungen.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Fehler beim Indizieren des Dokuments aufgetreten.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
