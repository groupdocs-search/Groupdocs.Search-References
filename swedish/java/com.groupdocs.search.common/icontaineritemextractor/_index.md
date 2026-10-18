---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search för Java API-referens"
description: "Tillhandahåller metoder för att extrahera objekt från behållardokument."
type: docs
weight: 35
url: /sv/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Tillhandahåller metoder för att extrahera objekt från behållardokument.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Hämtar dokumentformatfamiljen. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Extraherar objekt från containerdokumentet. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Extraherar objekt från containerdokumentet. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Hämtar dokumentformatfamiljen.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Extraherar objekt från containerdokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | filePath | java.lang.String | Filens sökväg. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - En array av extraherade objekt.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Extraherar objekt från containerdokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ström | java.io.InputStream | Dokumentströmmen. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - En array av extraherade objekt.

