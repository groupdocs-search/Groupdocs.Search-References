---
title: "ExtractorSettings"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Bevat instellingen voor de documentgegevens‑extractor."
type: docs
weight: 19
url: /nl/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Bevat instellingen voor de documentgegevens‑extractor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Haalt het indextype op waarvoor de extractor wordt gebruikt. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Stelt het indextype in waarvoor de extractor wordt gebruikt. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Haalt het indextype op waarvoor de extractor wordt gebruikt. De standaardwaarde is  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Stelt het indextype in waarvoor de extractor wordt gebruikt. De standaardwaarde is  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Het indextype waarvoor de extractor wordt gebruikt. |
|

