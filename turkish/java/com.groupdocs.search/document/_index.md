---
title: "Belge"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Dosya sistemi akışı veya yapısından bir indekse eklenen belgeler için temel sınıfı temsil eder."
type: docs
weight: 13
url: /tr/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Dosya sistemi, akış veya yapıdan bir indekse eklenen belgeler için temel sınıfı temsil eder. Farklı kaynak türlerinden belge oluşturmak için statik yöntemler içerir.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | Belge kaynağı türünü alır. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Bir dizinde belgeyi tanımlamak için kullanılan belge anahtarını alır. |
|
|  | [isLazy()](#isLazy--) | Belgenin gerektiği gibi yüklenip yüklenmediğini gösteren bir değeri alır. |
|
|  | [getModificationDate()](#getModificationDate--) | Belgenin son değiştirilme tarihini alır. |
|
|  | [getExtension()](#getExtension--) | Bu belge türü için kullanılan uzantıyı alır. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Belge için ek alanları alır. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Belge için ek alanları ayarlar. |
|
|  | [getAttributes()](#getAttributes--) | Belgenin özniteliklerini alır. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Belgenin özniteliklerini ayarlar. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Bir dosyadan belge oluşturur. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Bir akıştan belge oluşturur. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Metin alanlarından oluşan bir dizi olan bir yapıyı kullanarak belge oluşturur. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Tembel yüklemeli bir belge oluşturur. |
|
|  | [toString()](#toString--) | Geçerli  Document  nesnesini temsil eden bir  java.lang.String  döndürür. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Belge kaynağı türünü alır.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Bir dizinde belgeyi tanımlamak için kullanılan belge anahtarını alır.


**Returns:**
java.lang.String - Bir dizinde belgeyi tanımlamak için kullanılan belge anahtarı.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Belgenin gerektiği gibi yüklenip yüklenmediğini gösteren bir değeri alır.


**Returns:**
boolean - Belgenin gerektiği gibi yüklenip yüklenmediğini gösteren bir değer.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Belgenin son değiştirilme tarihini alır.


**Returns:**
java.util.Date - Belgenin son değiştirilme tarihi.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Bu belge türü için kullanılan uzantıyı alır.


**Returns:**
java.lang.String - Bu belge türü için kullanılan uzantı.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Belge için ek alanları alır.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Belge için ek alanlar.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Belge için ek alanları ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Belge için ek alanlar. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Belgenin özniteliklerini alır.


**Returns:**
java.lang.String[] - Belgenin öznitelikleri.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Belgenin özniteliklerini ayarlar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | java.lang.String[] | Belgenin öznitelikleri. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Bir dosyadan belge oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | filePath | java.lang.String | Belgenin dosya yolu. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Bir akıştan belge oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentKey | java.lang.String | Belgenin anahtarı. |
|
|  | modificationDate | java.util.Date | Belgenin değiştirilme tarihi. |
|
|  | extension | java.lang.String | Belgenin uzantısı. |
|
|  | stream | java.io.InputStream | Belgenin akışı. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Metin alanlarından oluşan bir dizi olan bir yapıyı kullanarak belge oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentKey | java.lang.String | Belgenin anahtarı. |
|
|  | modificationDate | java.util.Date | Belgenin değiştirilme tarihi. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Belgenin alanları. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Tembel yüklemeli bir belge oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | Belgenin kaynak türü. Bu değer, yüklenen belgenin türüyle eşleşmelidir. |
|
|  | documentKey | java.lang.String | Belgenin anahtarı. Bu değer, yüklenen belgenin anahtarıyla eşleşmelidir. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | Belge yükleyicisi. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


Geçerli  Document  nesnesini temsil eden bir  java.lang.String  döndürür.


**Returns:**
java.lang.String - Mevcut Document'ı temsil eden bir java.lang.String.

