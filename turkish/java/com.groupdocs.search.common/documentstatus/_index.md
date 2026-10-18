---
title: "DocumentStatus"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir belge işleme durumunu temsil eder."
type: docs
weight: 40
url: /tr/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Bir belge işleme durumunu temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Belge başarıyla indekslendi. |
|
|  | [Skipped](#Skipped) | Belge atlandı. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Belge indeksleme sırasında hata oluştu. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Belge başarıyla indekslendi.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Belge atlandı.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Belge indeksleme sırasında hata oluştu.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
