---
title: "IndexType"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Gibt einen Indextyp an."
type: docs
weight: 49
url: /de/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Gibt einen Indextyp an.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Normaler Index mit Dokumenten-Metadaten und Dokumenteninhalt, der alle Suchfunktionen unterstützt. |
|
|  | [MetadataIndex](#MetadataIndex) | Index, der nur Metadaten von Dokumenten enthält, ohne Inhalt. |
|
|  | [CompactIndex](#CompactIndex) | Indextyp, der deutlich weniger Speicherplatz benötigt, aber keine Phrasensuche und keine Datumsbereichssuche unterstützt. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Normaler Index mit Dokumenten-Metadaten und Dokumenteninhalt, der alle Suchfunktionen unterstützt.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Index, der nur Metadaten von Dokumenten enthält, ohne Inhalt.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Indextyp, der deutlich weniger Speicherplatz benötigt, aber keine Phrasensuche und keine Datumsbereichssuche unterstützt.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
