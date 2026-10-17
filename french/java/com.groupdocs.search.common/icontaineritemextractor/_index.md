---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Fournit des méthodes pour extraire des éléments de documents conteneurs."
type: docs
weight: 35
url: /fr/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Fournit des méthodes pour extraire des éléments de documents conteneurs.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Obtient la famille de formats de document. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Extrait les éléments du document conteneur. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Extrait les éléments du document conteneur. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Obtient la famille de formats de document.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Extrait les éléments du document conteneur.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Un tableau d'éléments extraits.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Extrait les éléments du document conteneur.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | stream | java.io.InputStream | Le flux du document. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Un tableau d'éléments extraits.

