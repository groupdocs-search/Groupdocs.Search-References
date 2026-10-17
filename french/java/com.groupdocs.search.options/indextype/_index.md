---
title: "IndexType"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Spécifie un type d'index."
type: docs
weight: 49
url: /fr/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Spécifie un type d'index.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | Description |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Index normal avec les métadonnées et le contenu des documents, qui prend en charge toutes les fonctionnalités de recherche. |
|
|  | [MetadataIndex](#MetadataIndex) | Index contenant uniquement les métadonnées des documents, sans le contenu. |
|
|  | [CompactIndex](#CompactIndex) | Type d'index qui occupe beaucoup moins d'espace disque mais ne prend pas en charge la recherche de phrases et les fonctionnalités de recherche par intervalle de dates. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Index normal avec les métadonnées et le contenu des documents, qui prend en charge toutes les fonctionnalités de recherche.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Index contenant uniquement les métadonnées des documents, sans le contenu.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Type d'index qui occupe beaucoup moins d'espace disque mais ne prend pas en charge la recherche de phrases et les fonctionnalités de recherche par intervalle de dates.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
