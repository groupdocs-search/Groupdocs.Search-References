---
title: "ExtractorSettings"
second_title: "GroupDocs.Search för Java API-referens"
description: "Innehåller inställningar för dokumentdataextraheraren."
type: docs
weight: 19
url: /sv/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Innehåller inställningar för dokumentdataextraheraren.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Hämtar indextypen som extrahören används för. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Ställer in indextypen som extrahören används för. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Hämtar indextypen som extrahören används för. Standardvärdet är  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Ställer in indextypen som extrahören används för. Standardvärdet är  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Indextypen som extrahören används för. |
|

