---
title: "Searcher"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक सेवा का प्रतिनिधित्व करता है जो खोज नेटवर्क के शार्ड्स को खोज क्वेरीज़ को प्रबंधित करती है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

एक सेवा का प्रतिनिधित्व करता है जो खोज नेटवर्क के शार्ड्स को खोज क्वेरीज़ को प्रबंधित करती है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | वितरित सर्च इंडेक्स में टेक्स्ट रूप में क्वेरी के साथ खोज शुरू करता है। |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | वितरित सर्च इंडेक्स में खोज शुरू करता है। |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | वितरित सर्च इंडेक्स में रिवर्स इमेज सर्च करता है। |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | वितरित सर्च इंडेक्स में खोज जारी रखता है। |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | वितरित सर्च इंडेक्स में रिवर्स इमेज सर्च जारी रखता है। |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | हाइलाइट किए गए खोजे गए शब्दों के साथ HTML फ़ॉर्मेटेड टेक्स्ट बनाता है। |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | सभी इंडेक्स्ड दस्तावेज़ों की एक एरे प्राप्त करता है। |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | निर्दिष्ट दस्तावेज़ के नेस्टेड आइटम्स की एक एरे प्राप्त करता है (जैसे ZIP, OST, PST कंटेनर दस्तावेज़ों के लिए)। |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | एक इंडेक्स्ड दस्तावेज़ का टेक्स्ट बनाता है और उसे आउटपुट एडैप्टर के माध्यम से पास करता है। |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


वितरित सर्च इंडेक्स में टेक्स्ट रूप में क्वेरी के साथ खोज शुरू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | क्वेरी | java.lang.String | सर्च क्वेरी। |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


वितरित सर्च इंडेक्स में खोज शुरू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | सर्च क्वेरी। |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


वितरित सर्च इंडेक्स में रिवर्स इमेज सर्च करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | खोजने के लिए छवि। |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | छवि खोज विकल्प। |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


वितरित सर्च इंडेक्स में खोज जारी रखता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | नेटवर्क सर्च टोकन। |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


वितरित सर्च इंडेक्स में रिवर्स इमेज सर्च जारी रखता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | नेटवर्क इमेज सर्च टोकन। |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


हाइलाइट किए गए खोजे गए शब्दों के साथ HTML फ़ॉर्मेटेड टेक्स्ट बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | पाया गया दस्तावेज़। |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | खोज परिणाम हाईलाइटर। |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | हाइलाइट विकल्प। |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


सभी इंडेक्स्ड दस्तावेज़ों की एक एरे प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - सभी अनुक्रमित दस्तावेज़ों की एक सरणी।

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


निर्दिष्ट दस्तावेज़ के नेस्टेड आइटम्स की एक एरे प्राप्त करता है (जैसे ZIP, OST, PST कंटेनर दस्तावेज़ों के लिए)।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | दस्तावेज़ जानकारी। |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - दस्तावेज़ आइटमों की एक सरणी।

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


एक इंडेक्स्ड दस्तावेज़ का टेक्स्ट बनाता है और उसे आउटपुट एडैप्टर के माध्यम से पास करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | अनुक्रमित दस्तावेज़ जानकारी। |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | आउटपुट एडैप्टर। |
|

