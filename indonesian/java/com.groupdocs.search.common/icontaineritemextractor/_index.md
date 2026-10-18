---
title: "IContainerItemExtractor"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan metode untuk mengekstrak item dari dokumen kontainer."
type: docs
weight: 35
url: /id/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Menyediakan metode untuk mengekstrak item dari dokumen kontainer.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Mendapatkan keluarga format dokumen. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Mengekstrak item dari dokumen kontainer. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Mengekstrak item dari dokumen kontainer. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Mendapatkan keluarga format dokumen.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Mengekstrak item dari dokumen kontainer.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | filePath | java.lang.String | Path file. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Sebuah array dari item yang diekstrak.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Mengekstrak item dari dokumen kontainer.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | stream | java.io.InputStream | Stream dokumen. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Sebuah array dari item yang diekstrak.

