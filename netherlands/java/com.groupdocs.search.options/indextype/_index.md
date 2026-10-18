---
title: "IndexType"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Specificeert een indextype."
type: docs
weight: 49
url: /nl/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Specificeert een indextype.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Normale index met documentmetadata en documentinhoud die alle zoekfuncties ondersteunt. |
|
|  | [MetadataIndex](#MetadataIndex) | Index die alleen metadata van documenten bevat, zonder inhoud. |
|
|  | [CompactIndex](#CompactIndex) | Indextype dat veel minder schijfruimte inneemt maar geen ondersteuning biedt voor frase‑zoekopdrachten en datumreeks‑zoekfuncties. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Normale index met documentmetadata en documentinhoud die alle zoekfuncties ondersteunt.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Index die alleen metadata van documenten bevat, zonder inhoud.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Indextype dat veel minder schijfruimte inneemt maar geen ondersteuning biedt voor frase‑zoekopdrachten en datumreeks‑zoekfuncties.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
