---
title: "Arayıcı"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağının parçalarına yapılan arama sorgularını yöneten bir hizmeti temsil eder."
type: docs
weight: 12
url: /tr/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Arama ağının parçalarına yapılan arama sorgularını yöneten bir hizmeti temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Dağıtık arama indeksinde metin biçiminde bir sorgu ile arama başlatır. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Dağıtık arama indeksinde arama başlatır. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Dağıtık arama indeksinde ters görüntü araması gerçekleştirir. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Dağıtık arama indeksinde aramayı sürdürür. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Dağıtık arama indeksinde ters görüntü aramasını sürdürür. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Bulunan terimleri vurgulayan HTML biçimlendirilmiş metin oluşturur. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Tüm indekslenmiş belgelerin bir dizisini alır. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Belirtilen belgenin iç içe öğelerinin bir dizisini alır (ZIP, OST, PST gibi kapsayıcı belgeler için). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | İndekslenmiş bir belgenin metnini oluşturur ve bir çıktı adaptörü aracılığıyla iletir. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Dağıtık arama indeksinde metin biçiminde bir sorgu ile arama başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | java.lang.String | Arama sorgusu. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Dağıtık arama indeksinde arama başlatır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Arama sorgusu. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Arama seçenekleri. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Dağıtık arama indeksinde ters görüntü araması gerçekleştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Aranacak görüntü. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Görüntü arama seçenekleri. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Dağıtık arama indeksinde aramayı sürdürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Ağ arama belirteci. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Dağıtık arama indeksinde ters görüntü aramasını sürdürür.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Ağ görüntü arama belirteci. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Bulunan terimleri vurgulayan HTML biçimlendirilmiş metin oluşturur.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Bulunan belge. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Arama sonucu vurgulayıcı. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Vurgulama seçenekleri. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Tüm indekslenmiş belgelerin bir dizisini alır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | shardIndex | int | Parça indeksi. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Tüm indekslenmiş belgelerin bir dizisi.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Belirtilen belgenin iç içe öğelerinin bir dizisini alır (ZIP, OST, PST gibi kapsayıcı belgeler için).


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Belge bilgisi. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Belge öğelerinin bir dizisi.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


İndekslenmiş bir belgenin metnini oluşturur ve bir çıktı adaptörü aracılığıyla iletir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | İndekslenmiş belge bilgisi. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Çıktı adaptörü. |
|

