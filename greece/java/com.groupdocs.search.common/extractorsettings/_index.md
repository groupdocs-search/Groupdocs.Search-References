---
title: "ExtractorSettings"
second_title: "GroupDocs.Search για Java API Reference"
description: "Περιέχει ρυθμίσεις για τον εξαγωγέα δεδομένων εγγράφου."
type: docs
weight: 19
url: /el/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Περιέχει ρυθμίσεις για τον εξαγωγέα δεδομένων εγγράφου.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Λαμβάνει τον τύπο ευρετηρίου για τον οποίο χρησιμοποιείται ο εξαγωγέας. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Ορίζει τον τύπο ευρετηρίου για τον οποίο χρησιμοποιείται ο εξαγωγέας. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Λαμβάνει τον τύπο ευρετηρίου για τον οποίο χρησιμοποιείται ο εξαγωγέας. Η προεπιλεγμένη τιμή είναι  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Ορίζει τον τύπο ευρετηρίου για τον οποίο χρησιμοποιείται ο εξαγωγέας. Η προεπιλεγμένη τιμή είναι  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Ο τύπος ευρετηρίου για τον οποίο χρησιμοποιείται ο εξαγωγέας. |
|

