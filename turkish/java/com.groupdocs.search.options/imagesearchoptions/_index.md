---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Ters görüntü arama işlemi için seçenekler sağlar."
type: docs
weight: 24
url: /tr/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Ters görüntü arama işlemi için seçenekler sağlar.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | ImageSearchOptions sınıfının yeni bir örneğini başlatır. |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | ImageSearchOptions sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Görüntü karmasındaki eşleşmeyen bitlerin maksimum sayısını alır. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Görüntü karmasındaki eşleşmeyen bitlerin maksimum sayısını ayarlar. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Görüntü ters arama isteği için bulunan görüntülerin maksimum sayısını alır. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Görüntü ters arama isteği için bulunan görüntülerin maksimum sayısını ayarlar. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Arama belge filtresini alır. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Arama belge filtresini alır veya ayarlar. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


ImageSearchOptions sınıfının yeni bir örneğini başlatır.


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


ImageSearchOptions sınıfının yeni bir örneğini başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | veri | java.lang.Object | Serileştirilmiş veri. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Görüntü karmasındaki eşleşmeyen bitlerin maksimum sayısını alır. Varsayılan değer 5'tir.


**Returns:**
int - Görüntü karmasındaki eşleşmeyen bitlerin maksimum sayısı.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Görüntü karmasındaki eşleşmeyen bitlerin maksimum sayısını ayarlar. Varsayılan değer 5'tir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Görüntü karmasındaki eşleşmeyen bitlerin maksimum sayısı. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Görüntü ters arama isteği için bulunan görüntülerin maksimum sayısını alır. Varsayılan değer 1000'dir.


**Returns:**
int - Görüntü ters arama isteği için bulunan görüntülerin maksimum sayısı.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Görüntü ters arama isteği için bulunan görüntülerin maksimum sayısını ayarlar. Varsayılan değer 1000'dir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | değer | int | Görüntü ters arama isteği için bulunan görüntülerin maksimum sayısı. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Arama belge filtresini alır. SearchDocumentFilter dahil etme mantığı üzerinde çalışır. Arama belge filtresi örnekleri oluşturmak için GroupDocs.Search.Options.SearchDocumentFilter sınıfını kullanın. Varsayılan değer null'dur, bu da bulunan tüm belgelerin döndürüleceği anlamına gelir.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Arama belge filtresini alır veya ayarlar. SearchDocumentFilter dahil etme mantığı üzerinde çalışır. Arama belge filtresi örnekleri oluşturmak için GroupDocs.Search.Options.SearchDocumentFilter sınıfını kullanın. Varsayılan değer null'dur, bu da bulunan tüm belgelerin döndürüleceği anlamına gelir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Arama belge filtresi. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
