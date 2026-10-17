---
title: "ExtractorSettings"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Contient les paramètres de l'extracteur de données de document."
type: docs
weight: 19
url: /fr/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Contient les paramètres de l'extracteur de données de document.

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Obtient le type d'index pour lequel l'extracteur est utilisé. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Définit le type d'index pour lequel l'extracteur est utilisé. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Obtient le type d'index pour lequel l'extracteur est utilisé. La valeur par défaut est  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Définit le type d'index pour lequel l'extracteur est utilisé. La valeur par défaut est  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Le type d'index pour lequel l'extracteur est utilisé. |
|

