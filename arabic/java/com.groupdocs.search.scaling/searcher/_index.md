---
title: "باحث"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل خدمة تدير استعلامات البحث إلى شظايا شبكة البحث."
type: docs
weight: 12
url: /ar/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

يمثل خدمة تدير استعلامات البحث إلى شظايا شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | يبدأ بحثًا باستخدام استعلام بصيغة نصية في فهرس البحث الموزع. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | يبدأ بحثًا في فهرس البحث الموزع. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | ينفّذ بحثًا عكسيًا عن صورة في فهرس البحث الموزع. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | يكمل بحثًا في فهرس البحث الموزع. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | يكمل بحثًا عكسيًا عن صورة في فهرس البحث الموزع. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | ينشئ نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | يحصل على مصفوفة من جميع المستندات المفهرسة. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | يحصل على مصفوفة من العناصر المتداخلة للمستند المحدد (للمستندات الحاوية مثل ZIP، OST، PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | ينشئ نص المستند المفهرس ويمرره عبر محول الإخراج. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


يبدأ بحثًا باستخدام استعلام بصيغة نصية في فهرس البحث الموزع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | java.lang.String | استعلام البحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


يبدأ بحثًا في فهرس البحث الموزع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | استعلام البحث. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | خيارات البحث. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


ينفّذ بحثًا عكسيًا عن صورة في فهرس البحث الموزع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | الصورة للبحث. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | خيارات بحث الصورة. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


يكمل بحثًا في فهرس البحث الموزع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | رمز البحث في الشبكة. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


يكمل بحثًا عكسيًا عن صورة في فهرس البحث الموزع.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | رمز البحث عن الصور في الشبكة. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


ينشئ نصًا بتنسيق HTML مع تسليط الضوء على المصطلحات التي تم العثور عليها.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | المستند الموجود. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | مُبرز نتيجة البحث. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | خيارات التمييز. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


يحصل على مصفوفة من جميع المستندات المفهرسة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | shardIndex | int | فهرس الشريحة. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - مصفوفة تحتوي على جميع المستندات المفهرسة.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


يحصل على مصفوفة من العناصر المتداخلة للمستند المحدد (للمستندات الحاوية مثل ZIP، OST، PST).


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | معلومات المستند. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - مصفوفة من عناصر المستند.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


ينشئ نص المستند المفهرس ويمرره عبر محول الإخراج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | معلومات المستند المفهرس. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | محول الإخراج. |
|

