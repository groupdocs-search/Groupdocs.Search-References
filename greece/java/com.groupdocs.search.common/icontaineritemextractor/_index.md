---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει μεθόδους για την εξαγωγή στοιχείων από έγγραφα περιέκτη."
type: docs
weight: 35
url: /el/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Παρέχει μεθόδους για την εξαγωγή στοιχείων από έγγραφα περιέκτη.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Λαμβάνει την οικογένεια μορφής του εγγράφου. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Εξάγει στοιχεία από το έγγραφο container. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Εξάγει στοιχεία από το έγγραφο container. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Λαμβάνει την οικογένεια μορφής του εγγράφου.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Εξάγει στοιχεία από το έγγραφο container.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή του αρχείου. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Ένας πίνακας εξαγόμενων στοιχείων.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Εξάγει στοιχεία από το έγγραφο container.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ροή | java.io.InputStream | Η ροή του εγγράφου. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Ένας πίνακας εξαγόμενων στοιχείων.

