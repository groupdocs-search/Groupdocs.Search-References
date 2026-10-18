---
title: "ExtractorSettings"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge veri çıkarıcısı için ayarları içerir."
type: docs
weight: 19
url: /tr/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Belge veri çıkarıcısı için ayarları içerir.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | Çıkarıcının kullanıldığı indeks tipini alır. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Çıkarıcının kullanıldığı indeks tipini ayarlar. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Çıkarıcının kullanıldığı indeks tipini alır. Varsayılan değer  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Çıkarıcının kullanıldığı indeks tipini ayarlar. Varsayılan değer  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | Çıkarıcının kullanıldığı indeks tipi. |
|

