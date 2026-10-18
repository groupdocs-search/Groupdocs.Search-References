---
title: "DocumentInfo"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Dizinlenmiş bir belge için bir tanımlayıcıyı temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

Dizinlenmiş bir belge için bir tanımlayıcıyı temsil eder.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [toString()](#toString--) | Geçerli  DocumentInfo  nesnesini temsil eden bir  System.String  döndürür. |
|
|  | [getFilePath()](#getFilePath--) | Dosyadan indekslenen dosya yolu veya akıştan/struktürden indekslenen belge anahtarını alır. |
|
|  | [getFileType()](#getFileType--) | Dosya türünü alır. |
|
|  | [getFormatFamily()](#getFormatFamily--) | Belge formatı ailesini alır. |
|
|  | [getInnerPath()](#getInnerPath--) | Kapsayıcı belge öğesinin iç yolunu alır. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | Kapsayıcı belge öğesinin iç yol bölümlerini alır. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Belge kaynağı türünü alır. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | İndeksleme hatası göstergesini alır. |
|
|  | [serialize()](#serialize--) | Geçerli örneği bir bayt dizisine serileştirir. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Bir örneği bayt dizisinden seriden çıkarır. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


Geçerli  DocumentInfo  nesnesini temsil eden bir  System.String  döndürür.


**Returns:**
java.lang.String - Geçerli  DocumentInfo  nesnesini temsil eden bir  System.String .

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


Dosyadan indekslenen dosya yolu veya akıştan/struktürden indekslenen belge anahtarını alır.


**Returns:**
java.lang.String - Dosya yolu veya belge anahtarı.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


Dosya türünü alır.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Belge formatı ailesini alır.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


Kapsayıcı belge öğesinin iç yolunu alır.


**Returns:**
java.lang.String - İç yol.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


Kapsayıcı belge öğesinin iç yol bölümlerini alır.


**Returns:**
java.lang.String[] - İç yol bölümleri.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Belge kaynağı türünü alır.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


İndeksleme hatası göstergesini alır.


**Returns:**
boolean - İndeksleme hatası göstergesi.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Geçerli örneği bir bayt dizisine serileştirir.


**Returns:**
byte[] - Geçerli örneği temsil eden bir bayt dizisi.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Bir örneği bayt dizisinden seriden çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dizi | byte[] | Serileştirilecek bir bayt dizisi. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

