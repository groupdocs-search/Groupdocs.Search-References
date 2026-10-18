---
title: "TextStorageSettings"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Metin depolama ayarlarını temsil eder."
type: docs
weight: 42
url: /tr/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Metin depolama ayarlarını temsil eder.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | TextStorageSettings sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getCompression()](#getCompression--) | Metin depolamanın sıkıştırmasını alır. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Metin depolamanın sıkıştırmasını ayarlar. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


TextStorageSettings sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Metin depolamanın sıkıştırması. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Metin depolamanın sıkıştırmasını alır. Varsayılan değer Compression.Normal'dır.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Metin depolamanın sıkıştırmasını ayarlar. Varsayılan değer Compression.Normal'dur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | Metin depolamanın sıkıştırması. |
|

