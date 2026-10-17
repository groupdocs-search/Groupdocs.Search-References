---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les informations d'un élément de conteneur."
type: docs
weight: 18
url: /fr/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Représente les informations d'un élément de conteneur.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Initialise une nouvelle instance de la classe ExtractedItemInfo. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Obtient un type de document. |
|
|  | [getFields()](#getFields--) | Obtient des champs extraits. |
|
|  | [getItemInfo()](#getItemInfo--) | Obtient les informations d'un élément. |
|
|  | [getInnerPath()](#getInnerPath--) | Obtient un chemin interne. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Initialise une nouvelle instance de la classe ExtractedItemInfo.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | La famille de formats de document. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Les champs extraits. |
|
|  | itemInfo | java.lang.String | Les informations de l'élément. |
|
|  | innerPath | java.lang.String | Le chemin vers l'élément dans le conteneur. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Obtient un type de document.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Obtient des champs extraits.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Les champs extraits.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Obtient les informations d'un élément.


**Returns:**
java.lang.String - Les informations de l'élément.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Obtient un chemin interne.


**Returns:**
java.lang.String - Le chemin interne.

