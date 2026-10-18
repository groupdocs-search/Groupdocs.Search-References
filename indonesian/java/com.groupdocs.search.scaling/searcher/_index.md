---
title: "Searcher"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili layanan yang mengelola kueri pencarian ke shard jaringan pencarian."
type: docs
weight: 12
url: /id/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Mewakili layanan yang mengelola kueri pencarian ke shard jaringan pencarian.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Memulai pencarian dengan kueri dalam bentuk teks pada indeks pencarian terdistribusi. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Memulai pencarian pada indeks pencarian terdistribusi. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Melakukan pencarian gambar terbalik pada indeks pencarian terdistribusi. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Melanjutkan pencarian pada indeks pencarian terdistribusi. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Melanjutkan pencarian gambar terbalik pada indeks pencarian terdistribusi. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Mendapatkan array semua dokumen yang diindeks. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Mendapatkan array item bersarang dari dokumen yang ditentukan (untuk dokumen kontainer seperti ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Menghasilkan teks dokumen yang diindeks dan melewatkannya melalui adaptor output. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Memulai pencarian dengan kueri dalam bentuk teks pada indeks pencarian terdistribusi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | java.lang.String | Kueri pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Memulai pencarian pada indeks pencarian terdistribusi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Kueri pencarian. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Opsi pencarian. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Melakukan pencarian gambar terbalik pada indeks pencarian terdistribusi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Gambar yang akan dicari. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Opsi pencarian gambar. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Melanjutkan pencarian pada indeks pencarian terdistribusi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Token pencarian jaringan. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Melanjutkan pencarian gambar terbalik pada indeks pencarian terdistribusi.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Token pencarian gambar jaringan. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Menghasilkan teks berformat HTML dengan istilah yang ditemukan disorot.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Dokumen yang ditemukan. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Penyorot hasil pencarian. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Opsi sorotan. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Mendapatkan array semua dokumen yang diindeks.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | shardIndex | int | Indeks shard. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Sebuah array dari semua dokumen yang diindeks.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Mendapatkan array item bersarang dari dokumen yang ditentukan (untuk dokumen kontainer seperti ZIP, OST, PST).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Informasi dokumen. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - Sebuah array dari item dokumen.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Menghasilkan teks dokumen yang diindeks dan melewatkannya melalui adaptor output.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Info dokumen yang diindeks. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Adapter output. |
|

