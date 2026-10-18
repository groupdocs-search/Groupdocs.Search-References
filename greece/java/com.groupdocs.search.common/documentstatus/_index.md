---
title: "DocumentStatus"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει την κατάσταση επεξεργασίας εγγράφου."
type: docs
weight: 40
url: /el/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Αντιπροσωπεύει την κατάσταση επεξεργασίας εγγράφου.

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Το έγγραφο ευρετηριάστηκε επιτυχώς. |
|
|  | [Skipped](#Skipped) | Το έγγραφο παραλείφθηκε. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Παρουσιάστηκε σφάλμα κατά την ευρετηρίαση του εγγράφου. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Το έγγραφο ευρετηριάστηκε επιτυχώς.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Το έγγραφο παραλείφθηκε.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Παρουσιάστηκε σφάλμα κατά την ευρετηρίαση του εγγράφου.


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
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
