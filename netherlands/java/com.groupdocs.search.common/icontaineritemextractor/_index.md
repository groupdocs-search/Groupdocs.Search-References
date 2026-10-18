---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Biedt methoden voor het extraheren van items uit containerdocumenten."
type: docs
weight: 35
url: /nl/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Biedt methoden voor het extraheren van items uit containerdocumenten.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Haalt de documentformaatfamilie op. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Extraheert items uit een containerdocument. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Extraheert items uit een containerdocument. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Haalt de documentformaatfamilie op.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Extraheert items uit een containerdocument.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestandspad. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Een array van geëxtraheerde items.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Extraheert items uit een containerdocument.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | stream | java.io.InputStream | De documentstroom. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Een array van geëxtraheerde items.

