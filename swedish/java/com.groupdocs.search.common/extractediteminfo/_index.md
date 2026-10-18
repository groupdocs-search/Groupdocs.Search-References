---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar information om ett containerobjekt."
type: docs
weight: 18
url: /sv/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Representerar information om ett containerobjekt.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Initierar en ny instans av klassen  ExtractedItemInfo  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Hämtar en dokumenttyp. |
|
|  | [getFields()](#getFields--) | Hämtar extraherade fält. |
|
|  | [getItemInfo()](#getItemInfo--) | Hämtar information om ett objekt. |
|
|  | [getInnerPath()](#getInnerPath--) | Hämtar en intern sökväg. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Initierar en ny instans av klassen  ExtractedItemInfo  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | Dokumentformatfamiljen. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | De extraherade fälten. |
|
|  | itemInfo | java.lang.String | Objektinformationen. |
|
|  | innerPath | java.lang.String | Sökvägen till objektet i behållaren. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Hämtar en dokumenttyp.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Hämtar extraherade fält.


**Returns:**
com.groupdocs.search.common.DocumentField[] - De extraherade fälten.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Hämtar information om ett objekt.


**Returns:**
java.lang.String - Objektinformationen.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Hämtar en intern sökväg.


**Returns:**
java.lang.String - Den interna sökvägen.

