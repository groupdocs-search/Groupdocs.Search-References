---
title: "IndexType"
second_title: "GroupDocs.Search för Java API-referens"
description: "Specificerar en indextyp."
type: docs
weight: 49
url: /sv/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Specificerar en indextyp.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Normalt index med dokumentmetadata och dokumentinnehåll som stödjer alla sökfunktioner. |
|
|  | [MetadataIndex](#MetadataIndex) | Index som endast innehåller metadata för dokument, utan innehåll. |
|
|  | [CompactIndex](#CompactIndex) | Indextyp som tar mycket mindre diskutrymme men inte stödjer frasökning och datumintervallssökning. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Normalt index med dokumentmetadata och dokumentinnehåll som stödjer alla sökfunktioner.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Index som endast innehåller metadata för dokument, utan innehåll.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Indextyp som tar mycket mindre diskutrymme men inte stödjer frasökning och datumintervallssökning.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
