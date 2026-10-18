---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά πληροφορίες στοιχείου δοχείου."
type: docs
weight: 18
url: /el/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Αναπαριστά πληροφορίες στοιχείου δοχείου.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExtractedItemInfo. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Λαμβάνει έναν τύπο εγγράφου. |
|
|  | [getFields()](#getFields--) | Λαμβάνει εξαγόμενα πεδία. |
|
|  | [getItemInfo()](#getItemInfo--) | Λαμβάνει πληροφορίες στοιχείου. |
|
|  | [getInnerPath()](#getInnerPath--) | Λαμβάνει εσωτερική διαδρομή. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης ExtractedItemInfo.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | Η οικογένεια μορφής εγγράφου. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Τα εξαγόμενα πεδία. |
|
|  | itemInfo | java.lang.String | Οι πληροφορίες του στοιχείου. |
|
|  | innerPath | java.lang.String | Η διαδρομή προς το στοιχείο στο δοχείο. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Λαμβάνει έναν τύπο εγγράφου.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Λαμβάνει εξαγόμενα πεδία.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Τα εξαγόμενα πεδία.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Λαμβάνει πληροφορίες στοιχείου.


**Returns:**
java.lang.String - Οι πληροφορίες του στοιχείου.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Λαμβάνει εσωτερική διαδρομή.


**Returns:**
java.lang.String - Η εσωτερική διαδρομή.

