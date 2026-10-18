---
title: "IndexType"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir indeks türü belirtir."
type: docs
weight: 49
url: /tr/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Bir indeks türü belirtir.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Tüm arama özelliklerini destekleyen, belge meta verileri ve belge içeriği içeren normal indeks. |
|
|  | [MetadataIndex](#MetadataIndex) | İçerik olmadan yalnızca belgelerin meta verilerini içeren indeks. |
|
|  | [CompactIndex](#CompactIndex) | Daha az disk alanı kullanan ancak ifade araması ve tarih aralığı arama özelliklerini desteklemeyen indeks türü. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Tüm arama özelliklerini destekleyen, belge meta verileri ve belge içeriği içeren normal indeks.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


İçerik olmadan yalnızca belgelerin meta verilerini içeren indeks.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Daha az disk alanı kullanan ancak ifade araması ve tarih aralığı arama özelliklerini desteklemeyen indeks türü.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
