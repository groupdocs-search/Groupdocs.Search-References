---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt containeriteminformatie voor."
type: docs
weight: 18
url: /nl/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Stelt containeriteminformatie voor.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Initialiseert een nieuw exemplaar van de  ExtractedItemInfo  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Haalt een documenttype op. |
|
|  | [getFields()](#getFields--) | Haalt geëxtraheerde velden op. |
|
|  | [getItemInfo()](#getItemInfo--) | Haalt een iteminformatie op. |
|
|  | [getInnerPath()](#getInnerPath--) | Haalt een intern pad op. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Initialiseert een nieuw exemplaar van de  ExtractedItemInfo  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | De documentformaatfamilie. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De geëxtraheerde velden. |
|
|  | itemInfo | java.lang.String | De iteminformatie. |
|
|  | innerPath | java.lang.String | Het pad naar het item in de container. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Haalt een documenttype op.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Haalt geëxtraheerde velden op.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De geëxtraheerde velden.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Haalt een iteminformatie op.


**Returns:**
java.lang.String - De iteminformatie.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Haalt een intern pad op.


**Returns:**
java.lang.String - Het interne pad.

