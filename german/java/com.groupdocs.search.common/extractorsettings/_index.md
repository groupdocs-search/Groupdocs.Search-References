---
title: "ExtractorSettings"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Enthält Einstellungen für den Dokumentdatenextraktor."
type: docs
weight: 19
url: /de/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Enthält Einstellungen für den Dokumentdatenextraktor.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Liefert den Indextyp, für den der Extraktor verwendet wird. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Legt den Indextyp fest, für den der Extraktor verwendet wird. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Liefert den Indextyp, für den der Extraktor verwendet wird. Der Standardwert ist  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Legt den Indextyp fest, für den der Extraktor verwendet wird. Der Standardwert ist  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Der Indextyp, für den der Extraktor verwendet wird. |
|

