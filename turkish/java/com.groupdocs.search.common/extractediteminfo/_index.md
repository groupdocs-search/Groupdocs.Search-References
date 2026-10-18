---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Kapsayıcı öğe bilgisini temsil eder."
type: docs
weight: 18
url: /tr/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Kapsayıcı öğe bilgisini temsil eder.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | ExtractedItemInfo sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Bir belge türü alır. |
|
|  | [getFields()](#getFields--) | Çıkarılan alanları alır. |
|
|  | [getItemInfo()](#getItemInfo--) | Bir öğe bilgisini alır. |
|
|  | [getInnerPath()](#getInnerPath--) | İç bir yolu alır. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


ExtractedItemInfo sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | Belge formatı ailesi. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Çıkarılan alanlar. |
|
|  | itemInfo | java.lang.String | Öğe bilgisi. |
|
|  | innerPath | java.lang.String | Konteyner içindeki öğenin yolu. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Bir belge türü alır.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Çıkarılan alanları alır.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Çıkarılan alanlar.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Bir öğe bilgisini alır.


**Returns:**
java.lang.String - Öğenin bilgisi.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


İç bir yolu alır.


**Returns:**
java.lang.String - İç yol.

