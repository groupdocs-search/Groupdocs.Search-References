---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Kapsayıcı belgelerden öğeleri çıkarmak için yöntemler sağlar."
type: docs
weight: 35
url: /tr/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Kapsayıcı belgelerden öğeleri çıkarmak için yöntemler sağlar.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Belge formatı ailesini alır. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Kapsayıcı belgelerden öğeleri çıkarır. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Kapsayıcı belgelerden öğeleri çıkarır. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Belge formatı ailesini alır.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Kapsayıcı belgelerden öğeleri çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Dosya yolu. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Çıkarılan öğelerin bir dizisi.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Kapsayıcı belgelerden öğeleri çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | stream | java.io.InputStream | Belgenin akışı. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Çıkarılan öğelerin bir dizisi.

