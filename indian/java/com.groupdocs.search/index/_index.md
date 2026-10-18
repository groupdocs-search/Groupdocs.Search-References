---
title: "Index"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ों को इंडेक्स करने और उनके माध्यम से खोज करने के लिए मुख्य वर्ग का प्रतिनिधित्व करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

दस्तावेज़ों को इंडेक्स करने और उनके माध्यम से खोज करने के लिए मुख्य वर्ग का प्रतिनिधित्व करता है।


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchResult result = index.search(query); // इंडेक्स में खोज रहा है
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Index()](#Index--) | स्मृति में  Index  वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | विशिष्ट इंडेक्स सेटिंग्स के साथ स्मृति में  Index  वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) |   Index  वर्ग का एक नया उदाहरण प्रारंभ करता है। |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | नया उदाहरण प्रारंभ करता है |
Index
वर्ग।
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | नया उदाहरण प्रारंभ करता है |
Index
वर्ग।
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | नया उदाहरण प्रारंभ करता है |
Index
वर्ग।
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getEvents()](#getEvents--) | इवेंट्स की सदस्यता के लिए इवेंट हब प्राप्त करता है। |
|
|  | [getIndexInfo()](#getIndexInfo--) | इंडेक्स पर मूल जानकारी प्राप्त करता है। |
|
|  | [getRepository()](#getRepository--) | यदि इंडेक्स उसमें शामिल है तो इंडेक्स रिपॉजिटरी ऑब्जेक्ट प्राप्त करता है। |
|
|  | [getIndexSettings()](#getIndexSettings--) | इंडेक्स सेटिंग्स प्राप्त करता है। |
|
|  | [getDictionaries()](#getDictionaries--) | शब्दकोश रिपॉजिटरी प्राप्त करता है। |
|
|  | [close()](#close--) | द्वारा उपयोग किए गए सभी संसाधनों को रिलीज़ करता है |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [add(String[] paths)](#add-java.lang.String---) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [update()](#update--) | पिछले अपडेट के बाद बदलें या हटाए गए दस्तावेज़ों को पुनः-इंडेक्स करता है। |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | पिछले अपडेट के बाद बदलें या हटाए गए दस्तावेज़ों को पुनः-इंडेक्स करता है। |
|
|  | [getIndexingReports()](#getIndexingReports--) | इंडेक्सिंग ऑपरेशनों पर रिपोर्ट प्राप्त करता है। |
|
|  | [getSearchReports()](#getSearchReports--) | सर्च ऑपरेशनों पर रिपोर्ट प्राप्त करता है। |
|
|  | [search(String query)](#search-java.lang.String-) | इंडेक्स में खोज करता है। |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | इंडेक्स में खोज करता है। |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | इंडेक्स में खोज करता है। |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | इंडेक्स में खोज करता है। |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | इंडेक्स में रिवर्स इमेज सर्च करता है। |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | मेथड Search से शुरू किए गए चंक सर्च को जारी रखता है। |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | मेथड Search से शुरू किए गए चंक सर्च को जारी रखता है। |
|
|  | [optimize()](#optimize--) | इंडेक्स सेगमेंट्स की संख्या को एक-दूसरे के साथ मर्ज करके न्यूनतम करता है। |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | इंडेक्स सेगमेंट्स की संख्या को एक-दूसरे के साथ मर्ज करके न्यूनतम करता है। |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | निर्दिष्ट इंडेक्स को वर्तमान इंडेक्स में मर्ज करता है। |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | निर्दिष्ट इंडेक्स रिपॉजिटरी से इंडेक्स को वर्तमान इंडेक्स में मर्ज करता है। |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | हाइलाइट किए गए खोजे गए शब्दों के साथ HTML फ़ॉर्मेटेड टेक्स्ट बनाता है। |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | हाइलाइट किए गए खोजे गए शब्दों के साथ HTML फ़ॉर्मेटेड टेक्स्ट बनाता है। |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | सभी इंडेक्स्ड दस्तावेज़ों की एक एरे प्राप्त करता है। |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | दस्तावेज़ आइटम्स की एक एरे प्राप्त करता है। |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | दस्तावेज़ कुंजी द्वारा एक इंडेक्स्ड दस्तावेज़ प्राप्त करता है। |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | एक इंडेक्स्ड दस्तावेज़ का टेक्स्ट बनाता है और उसे आउटपुट एडैप्टर के माध्यम से पास करता है। |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | इंडेक्स्ड दस्तावेज़ के लिए HTML फ़ॉर्मेटेड टेक्स्ट बनाता है और उसे आउटपुट एडैप्टर के माध्यम से ट्रांसफ़र करता है। |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | इंडेक्स्ड पाथ्स की एक एरे प्राप्त करता है - दस्तावेज़ या फ़ोल्डर। |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | इंडेक्स से इंडेक्स्ड फ़ाइलें या फ़ोल्डर हटाता है। |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | स्ट्रीम या स्ट्रक्चर से इंडेक्स्ड दस्तावेज़ हटाता है। |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | सूचना करने के लिए निर्दिष्ट नोटिफिकेशन ऑब्जेक्ट को इंडेक्स में पास करता है। |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | अपडेट ऑपरेशन के दौरान रीइंडेक्सिंग किए बिना निर्दिष्ट एट्रिब्यूट परिवर्तन बैच को इंडेक्स्ड दस्तावेज़ों पर लागू करता है। |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | निर्दिष्ट इंडेक्स्ड दस्तावेज़ से जुड़े सभी एट्रिब्यूट्स प्राप्त करता है। |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | पूरे इंडेक्स को मेमोरी में लोड करता है। |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | पूरे इंडेक्स को मेमोरी में लोड करता है। |
|
### Index() {#Index--}
```
public Index()
```


स्मृति में  Index  वर्ग का एक नया उदाहरण प्रारंभ करता है।


उदाहरण दर्शाता है कि डिस्क पर फ़ाइलें सहेजे बिना मेमोरी में इंडेक्स कैसे बनाएं।

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


विशिष्ट इंडेक्स सेटिंग्स के साथ स्मृति में  Index  वर्ग का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | इंडेक्स सेटिंग्स ऑब्जेक्ट। |


उदाहरण दर्शाता है कि विशेष इंडेक्स सेटिंग्स के साथ डिस्क पर फ़ाइलें सहेजे बिना मेमोरी में इंडेक्स कैसे बनाएं।

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Index क्लास का एक नया उदाहरण आरंभ करता है। डिस्क पर एक नया इंडेक्स बनाता है या मौजूदा इंडेक्स खोलता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर पथ। |


उदाहरण दर्शाता है कि डिस्क पर इंडेक्स कैसे बनाया जाए या मौजूदा इंडेक्स कैसे खोला जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


नया उदाहरण प्रारंभ करता है
Index
वर्ग।
विशिष्ट सेटिंग्स के साथ एक नया इंडेक्स बनाता है या डिस्क पर मौजूदा इंडेक्स खोलता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर पथ। |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | इंडेक्स सेटिंग्स ऑब्जेक्ट। |

उदाहरण दर्शाता है कि विशिष्ट इंडेक्स सेटिंग्स के साथ डिस्क पर इंडेक्स कैसे बनाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


नया उदाहरण प्रारंभ करता है
Index
वर्ग।
डिस्क से मौजूदा इंडेक्स लोड करता है यदि
overwriteIfExists
है
false
;
अन्यथा डिस्क पर एक नया इंडेक्स बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर पथ। |
|
|  | overwriteIfExists | boolean | इंडेक्स फ़ोल्डर को ओवरराइट करने का फ़्लैग। |

उदाहरण दर्शाता है कि पहले से एक अन्य इंडेक्स वाले फ़ोल्डर में नया इंडेक्स कैसे बनाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


नया उदाहरण प्रारंभ करता है
Index
वर्ग।
डिस्क से मौजूदा इंडेक्स लोड करता है यदि
overwriteIfExists
है
false
;
अन्यथा विशिष्ट इंडेक्स सेटिंग्स के साथ डिस्क पर नया इंडेक्स बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर पथ। |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | इंडेक्स सेटिंग्स ऑब्जेक्ट। |
|
|  | overwriteIfExists | boolean | इंडेक्स फ़ोल्डर को ओवरराइट करने का फ़्लैग। |

उदाहरण दर्शाता है कि विशिष्ट इंडेक्स सेटिंग्स के साथ डिस्क पर इंडेक्स कैसे बनाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


इवेंट्स की सदस्यता के लिए इवेंट हब प्राप्त करता है।


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


इंडेक्स पर मूल जानकारी प्राप्त करता है।


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


यदि इंडेक्स उसमें शामिल है तो इंडेक्स रिपॉजिटरी ऑब्जेक्ट प्राप्त करता है।


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


इंडेक्स सेटिंग्स प्राप्त करता है।


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


शब्दकोश रिपॉजिटरी प्राप्त करता है।


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


द्वारा उपयोग किए गए सभी संसाधनों को रिलीज़ करता है
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


इंडेक्सिंग ऑपरेशन करता है।
एक निरपेक्ष या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है।
सभी उपफ़ोल्डरों से दस्तावेज़ों को इंडेक्स किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | इंडेक्स की जाने वाली फ़ाइल या फ़ोल्डर का पथ। |

उदाहरण दर्शाता है कि इंडेक्स में दस्तावेज़ कैसे जोड़े जाएँ।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(folderPath); // निर्दिष्ट फ़ोल्डर में दस्तावेज़ों का अनुक्रमण
index.add(filePath); // निर्दिष्ट दस्तावेज़ का अनुक्रमण
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


इंडेक्सिंग ऑपरेशन करता है।
एक निरपेक्ष या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है।
सभी उपफ़ोल्डरों से दस्तावेज़ों को इंडेक्स किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | इंडेक्स की जाने वाली फ़ाइल या फ़ोल्डर का पथ। |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | अनुक्रमण विकल्प। |

उदाहरण दर्शाता है कि विशेष अनुक्रमण विकल्पों के साथ अनुक्रम में दस्तावेज़ कैसे जोड़ें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // इंडेक्सिंग थ्रेड्स की संख्या सेट करना
index.add(folderPath, options); // निर्दिष्ट फ़ोल्डर में दस्तावेज़ों का अनुक्रमण
index.add(filePath, options); // निर्दिष्ट दस्तावेज़ का अनुक्रमण
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


इंडेक्सिंग ऑपरेशन करता है।
एक पूर्ण या सापेक्ष पथ द्वारा फ़ाइलें या फ़ोल्डर जोड़ता है।
सभी उपफ़ोल्डरों से दस्तावेज़ों को इंडेक्स किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पथ | java.lang.String[] | अनुक्रमित की जाने वाली फ़ाइलों या फ़ोल्डरों के पथ। |

उदाहरण दर्शाता है कि इंडेक्स में दस्तावेज़ कैसे जोड़े जाएँ।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // निर्दिष्ट पथों पर दस्तावेज़ों का अनुक्रमण
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


इंडेक्सिंग ऑपरेशन करता है।
एक पूर्ण या सापेक्ष पथ द्वारा फ़ाइलें या फ़ोल्डर जोड़ता है।
सभी उपफ़ोल्डरों से दस्तावेज़ों को इंडेक्स किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पथ | java.lang.String[] | अनुक्रमित की जाने वाली फ़ाइलों या फ़ोल्डरों के पथ। |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | अनुक्रमण विकल्प। |

उदाहरण दर्शाता है कि विशेष अनुक्रमण विकल्पों के साथ अनुक्रम में दस्तावेज़ कैसे जोड़ें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // इंडेक्सिंग थ्रेड्स की संख्या सेट करना
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // निर्दिष्ट पथों पर दस्तावेज़ों का अनुक्रमण
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


इंडेक्सिंग ऑपरेशन करता है।
फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़ जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़। |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | अनुक्रमण विकल्प। |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


इंडेक्सिंग ऑपरेशन करता है।
निकाले गए डेटा को अनुक्रम में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | निकाला गया डेटा। |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | अनुक्रमण विकल्प। |
|

### update() {#update--}
```
public final void update()
```


पिछले अपडेट के बाद बदलें या हटाए गए दस्तावेज़ों को पुनः-इंडेक्स करता है।
अनुक्रमित फ़ोल्डरों में जोड़ी गई नई फ़ाइलें जोड़ता है।

उदाहरण दर्शाता है कि अनुक्रम को कैसे अपडेट करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
// दस्तावेज़ फ़ोल्डर से दस्तावेज़ हटाएँ या उन्हें संशोधित करें या फ़ोल्डर में नए दस्तावेज़ जोड़ें
index.update(); // अनुक्रम को अपडेट कर रहा है
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


पिछले अपडेट के बाद बदलें या हटाए गए दस्तावेज़ों को पुनः-इंडेक्स करता है।
अनुक्रमित फ़ोल्डरों में जोड़ी गई नई फ़ाइलें जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | अपडेट विकल्प। |

उदाहरण दर्शाता है कि विशेष अपडेट विकल्पों के साथ अनुक्रम को कैसे अपडेट करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
// दस्तावेज़ फ़ोल्डर से दस्तावेज़ हटाएँ या उन्हें संशोधित करें या फ़ोल्डर में नए दस्तावेज़ जोड़ें
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // इंडेक्सिंग थ्रेड्स की संख्या सेट करना
index.update(options); // अनुक्रम को अपडेट कर रहा है
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


इंडेक्सिंग ऑपरेशनों पर रिपोर्ट प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.IndexingReport[] - अनुक्रमण रिपोर्ट।

उदाहरण दर्शाता है कि अनुक्रमण रिपोर्ट कैसे प्राप्त करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
IndexingReport[] reports = index.getIndexingReports(); // अनुक्रमण रिपोर्ट प्राप्त कर रहा है
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


सर्च ऑपरेशनों पर रिपोर्ट प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.SearchReport[] - खोज रिपोर्ट।

उदाहरण दिखाता है कि खोज रिपोर्ट कैसे प्राप्त करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchResult result1 = index.search(query1); // खोज
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // खोज रिपोर्ट प्राप्त कर रहा है
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | क्वेरी | java.lang.String | सर्च क्वेरी। |

निम्नलिखित उदाहरण दिखाता है कि सरल खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchResult result = index.search(query); // खोज
 
```
 
````

निम्नलिखित उदाहरण दिखाता है कि रेगेक्स खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
String query = "^[0-9]{3,}"; // खोज क्वेरी की शुरुआत में कैरेट प्रतीक इंडेक्स को बताता है कि यह रेगेक्स क्वेरी है
SearchResult result = index.search(query); // खोज
 
```
 
````

निम्नलिखित उदाहरण दिखाता है कि फ़ैसिटेड खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
String query = "content:Newton"; // क्वेरी में कोलन से पहले शब्द दस्तावेज़ फ़ील्ड का नाम दर्शाता है जिसे खोजा जाना है
SearchResult result = index.search(query); // खोज
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | क्वेरी | java.lang.String | सर्च क्वेरी। |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |

निम्नलिखित उदाहरण दिखाता है कि फज़ी खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // फज़ी खोज को सक्षम करना
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // प्रत्येक शब्द के लिए संभावित अंतर की संख्या सेट करना
// शुरुआत और अंत में डबल कोट्स इंडेक्स को बताते हैं कि यह वाक्यांश खोज क्वेरी है
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // खोज करना
 
```
 
````

निम्नलिखित उदाहरण दिखाता है कि समानार्थक शब्द खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // समानार्थक शब्द खोज को सक्षम करना
String query = "cry";
SearchResult result = index.search(query, options); // खोज करना
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | सर्च क्वेरी। |

निम्नलिखित उदाहरण दिखाता है कि ऑब्जेक्ट रूप में क्वेरी का उपयोग करके खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
// सबक्वेरी 1 बनाना
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // केवल subquery 1 के लिए खोज विकल्प सेट कर रहा है
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // फज़ी खोज को सक्षम कर रहा है
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // अधिकतम अंतर की संख्या सेट कर रहा है
// subquery 2 बना रहा है
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// subquery 3 बना रहा है
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// उप‑प्रश्नों को एक क्वेरी में संयोजित करना
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // खोज
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | सर्च क्वेरी। |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |

निम्नलिखित उदाहरण दिखाता है कि ऑब्जेक्ट रूप में क्वेरी का उपयोग करके खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
// तिथि सीमा खोज का उप‑प्रश्न बनाना
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// 0 से 2 तक छूटे शब्दों की संख्या के साथ वाइल्डकार्ड का उप‑प्रश्न बनाना
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// सरल शब्द का उप‑प्रश्न बनाना
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // केवल उप‑प्रश्न 3 के लिए खोज विकल्प सेट करना
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// उप‑प्रश्नों को एक क्वेरी में संयोजित करना
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// पाए गए घटनाओं की बढ़ी हुई क्षमता के साथ खोज विकल्प वस्तु बनाना
SearchOptions options = new SearchOptions(); // समग्र खोज विकल्प
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // खोज करना
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


इंडेक्स में रिवर्स इमेज सर्च करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | खोजने के लिए छवि। |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | छवि खोज विकल्प। |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


मेथड Search से शुरू किए गए चंक सर्च को जारी रखता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | चंक खोज टोकन। |

यह उदाहरण दिखाता है कि चंक खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // चंक खोज को सक्षम कर रहा है
SearchResult result = index.search(query, options); // चंक खोज शुरू कर रहा है
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // चंक खोज जारी रख रहा है
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


मेथड Search से शुरू किए गए चंक सर्च को जारी रखता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | चंक खोज टोकन। |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | रद्दीकरण वस्तु। |

यह उदाहरण दिखाता है कि वस्तु रूप में क्वेरी का उपयोग करके खोज कैसे करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
Cancellation cancellation = new Cancellation(); // यदि रद्द किया जाए तो यह रद्दीकरण वस्तु सभी खोज जारी रखने को रोक देती है
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // चंक खोज को सक्षम कर रहा है
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // चंक खोज शुरू कर रहा है
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // चंक खोज जारी रख रहा है
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


इंडेक्स सेगमेंट्स की संख्या को एक-दूसरे के साथ मर्ज करके न्यूनतम करता है।
यह ऑपरेशन खोज प्रदर्शन को बेहतर बनाता है।

यह उदाहरण दिखाता है कि इंडेक्स के खंडों को कैसे मिलाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder1); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को अनुक्रमित करना
index.add(documentsFolder2); // AddToIndex को प्रत्येक कॉल इंडेक्स में कम से कम एक नया खंड बनाता है
index.add(documentsFolder3);
// इंडेक्स के खंडों को मिलाना
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


इंडेक्स सेगमेंट्स की संख्या को एक-दूसरे के साथ मर्ज करके न्यूनतम करता है।
यह ऑपरेशन खोज प्रदर्शन को बेहतर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | विलय विकल्प। |

यह उदाहरण विशेष विलय विकल्पों के साथ एक इंडेक्स के खंडों को कैसे मिलाया जाए दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder1); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को अनुक्रमित करना
index.add(documentsFolder2); // AddToIndex को प्रत्येक कॉल इंडेक्स में कम से कम एक नया खंड बनाता है
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // असिंक्रोनस ऑपरेशन
options.setCancellation(new Cancellation()); // रद्दीकरण ऑब्जेक्ट बनाना
// इंडेक्स के खंडों को मिलाना
index.optimize(options); // यह मेथड ऑपरेशन के पूर्ण होने से पहले ही लौटेगा
options.getCancellation().cancelAfter(10000); // ऑपरेशन की अधिकतम अवधि को 10 सेकंड पर सेट करना
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


निर्दिष्ट इंडेक्स को वर्तमान इंडेक्स में मर्ज करता है।
ध्यान दें कि अन्य इंडेक्स नहीं बदलेगा।


यदि अन्य इंडेक्स का पहले का संस्करण है, तो इसे मिलाने से पहले अपडेट करना आवश्यक है
IndexUpdater
.


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | वह इंडेक्स जिसमें मिलाना है। |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | विलय विकल्प। |

यह उदाहरण दिखाता है कि एक इंडेक्स को वर्तमान इंडेक्स में कैसे मिलाया जाए।

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // इंडेक्स1 बनाना
index1.add(documentsFolder1); // दस्तावेज़ों को अनुक्रमित करना
Index index2 = new Index(indexFolder2); // इंडेक्स2 बनाना
index2.add(documentsFolder2); // दस्तावेज़ों को अनुक्रमित करना
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // रद्दीकरण ऑब्जेक्ट बनाना
// index2 को index1 में मिलाना। ध्यान दें कि index2 फ़ाइलें नहीं बदलेगी।
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


निर्दिष्ट इंडेक्स रिपॉजिटरी से इंडेक्स को वर्तमान इंडेक्स में मर्ज करता है।
ध्यान दें कि रिपॉज़िटरी में सूचकांक नहीं बदले जाएंगे।


यदि अन्य सूचकांकों का पूर्व संस्करण है, तो उन्हें मर्ज करने से पहले अपडेट किया जाना चाहिए।
IndexUpdater
.


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | जिस सूचकांक रिपॉज़िटरी में मर्ज किया जाएगा वह। |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | विलय विकल्प। |

यह उदाहरण दर्शाता है कि कैसे एक सूचकांक रिपॉज़िटरी को वर्तमान सूचकांक में मर्ज किया जाता है।

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // इंडेक्स1 बनाना
index1.add(documentsFolder1); // दस्तावेज़ों को अनुक्रमित करना
IndexRepository repository = new IndexRepository(); // सूचकांक रिपॉज़िटरी बना रहा है
Index index2 = repository.create(indexFolder2); // index2 बना रहा है
index2.add(documentsFolder2); // दस्तावेज़ों को अनुक्रमित करना
Index index3 = repository.create(indexFolder3); // index3 बना रहा है
index3.add(documentsFolder3); // दस्तावेज़ों को इंडेक्स कर रहा है
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // रद्दीकरण ऑब्जेक्ट बनाना
// सभी सूचकांकों को सूचकांक रिपॉज़िटरी में index1 में मर्ज कर रहा है। ध्यान दें कि index2 और index3 नहीं बदले जाएंगे।
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


हाइलाइट किए गए खोजे गए शब्दों के साथ HTML फ़ॉर्मेटेड टेक्स्ट बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | पाया गया दस्तावेज़। |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | खोज परिणाम हाईलाइटर। |

यह उदाहरण दर्शाता है कि HTML स्वरूपित पाठ में घटनाओं को कैसे हाईलाइट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentFolder);
// शब्द 'eternity' की खोज करें
SearchResult result = index.search("eternity");
// पाठ में घटनाओं को हाईलाइट कर रहा है
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // पहला पाया गया दस्तावेज़ प्राप्त कर रहा है
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // फ़ाइल के लिए आउटपुट एडाप्टर बना रहा है
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // हाइलाइटर ऑब्जेक्ट बना रहा है
index.highlight(document, highlighter); // हाइलाइटेड घटनाओं के साथ HTML स्वरूपित टेक्स्ट उत्पन्न कर रहा है
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


हाइलाइट किए गए खोजे गए शब्दों के साथ HTML फ़ॉर्मेटेड टेक्स्ट बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | पाया गया दस्तावेज़। |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | खोज परिणाम हाईलाइटर। |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | हाइलाइट विकल्प। |

यह उदाहरण दर्शाता है कि HTML स्वरूपित पाठ में घटनाओं को कैसे हाईलाइट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentFolder);
// शब्द 'eternity' की खोज करें
SearchResult result = index.search("eternity");
// पाठ में घटनाओं को हाईलाइट कर रहा है
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // पहला पाया गया दस्तावेज़ प्राप्त कर रहा है
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // फ़ाइल के लिए आउटपुट एडाप्टर बना रहा है
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // हाइलाइटर ऑब्जेक्ट बना रहा है
HighlightOptions options = new HighlightOptions(); // हाइलाइट विकल्प ऑब्जेक्ट बना रहा है
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // हाइलाइटेड घटनाओं के साथ HTML स्वरूपित टेक्स्ट उत्पन्न कर रहा है
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


सभी इंडेक्स्ड दस्तावेज़ों की एक एरे प्राप्त करता है।


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - सभी अनुक्रमित दस्तावेज़ों की एक एरे।

यह उदाहरण दिखाता है कि कैसे एक इंडेक्स से अनुक्रमित दस्तावेज़ों की सूची प्राप्त की जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// अनुक्रमित दस्तावेज़ों की सूची प्राप्त कर रहा है
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


दस्तावेज़ आइटम्स की एक एरे प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | एक दस्तावेज़ जानकारी। |

यह उदाहरण दिखाता है कि कैसे एक इंडेक्स से अनुक्रमित दस्तावेज़ के आइटमों की सूची प्राप्त की जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// अनुक्रमित दस्तावेज़ों की सूची प्राप्त कर रहा है
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // दस्तावेज़ आइटमों की सूची प्राप्त कर रहा है
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - एक दस्तावेज़ आइटमों की एरे।

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


दस्तावेज़ कुंजी द्वारा एक इंडेक्स्ड दस्तावेज़ प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़कुंजी | java.lang.String | दस्तावेज़ कुंजी। |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


एक इंडेक्स्ड दस्तावेज़ का टेक्स्ट बनाता है और उसे आउटपुट एडैप्टर के माध्यम से पास करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | अनुक्रमित दस्तावेज़ जानकारी। |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | आउटपुट एडैप्टर। |

यह उदाहरण दिखाता है कि कैसे एक इंडेक्स से अनुक्रमित दस्तावेज़ का टेक्स्ट प्राप्त किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// अनुक्रमित दस्तावेज़ों की सूची प्राप्त कर रहा है
DocumentInfo[] documents = index.getIndexedDocuments();
// दस्तावेज़ पाठ प्राप्त करना
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


इंडेक्स्ड दस्तावेज़ के लिए HTML फ़ॉर्मेटेड टेक्स्ट बनाता है और उसे आउटपुट एडैप्टर के माध्यम से ट्रांसफ़र करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | अनुक्रमित दस्तावेज़ जानकारी। |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | आउटपुट एडैप्टर। |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | पाठ पुनर्प्राप्ति विकल्प। |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


इंडेक्स्ड पाथ्स की एक एरे प्राप्त करता है - दस्तावेज़ या फ़ोल्डर।


**Returns:**
java.lang.String[] - अनुक्रमित पथों की एक सरणी।

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


अनुक्रमित फ़ाइलों या फ़ोल्डरों को इंडेक्स से हटाता है। फिर हटाए गए पथों के बिना इंडेक्स को अपडेट करता है।
ध्यान दें कि यदि कोई व्यक्तिगत दस्तावेज़ फ़ोल्डर के हिस्से के रूप में इंडेक्स में जोड़ा गया था, तो उसे इंडेक्स से हटाया नहीं जा सकता।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पथ | java.lang.String[] | हटाने के लिए फ़ाइलों या फ़ोल्डरों के पथ। |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | अपडेट विकल्प। |

यह उदाहरण दर्शाता है कि इंडेक्स से अनुक्रमित पथों को कैसे हटाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डरों से दस्तावेज़ों का अनुक्रमण
index.add(documentsFolder1);
index.add(documentsFolder2);
// इंडेक्स से अनुक्रमित पथ प्राप्त करना
String[] indexedPaths1 = index.getIndexedPaths();
// अनुक्रमित पथों को कंसोल में लिखना
System.out.println("Indexed paths:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// इंडेक्स से पथ को हटाना
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// हटाने के बाद अनुक्रमित पथ प्राप्त करना
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nDeleted paths: " + deleteResult.getSuccessCount());
System.out.println("\nइंडेक्स्ड पाथ्स:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


स्ट्रीम या संरचनाओं से इंडेक्स किए गए दस्तावेज़ों को हटाता है। फिर हटाए गए दस्तावेज़ों के बिना इंडेक्स को अपडेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | अपडेट विकल्प। |
|
|  | documentKeys | java.lang.String[] | स्ट्रीम या संरचनाओं से जोड़े गए दस्तावेज़ों की कुंजियाँ। |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


सूचना करने के लिए निर्दिष्ट नोटिफिकेशन ऑब्जेक्ट को इंडेक्स में पास करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | सूचना वस्तु। |
|

**Returns:**
boolean - यदि सूचना सफलतापूर्वक निष्पादित हुई तो  true  लौटाता है; अन्यथा  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


अपडेट ऑपरेशन के दौरान रीइंडेक्सिंग किए बिना निर्दिष्ट एट्रिब्यूट परिवर्तन बैच को इंडेक्स्ड दस्तावेज़ों पर लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | गुणधर्म परिवर्तन बैच। |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


निर्दिष्ट इंडेक्स्ड दस्तावेज़ से जुड़े सभी एट्रिब्यूट्स प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | दस्तावेज़ पथ। |
|

**Returns:**
java.lang.String[] - दस्तावेज़ से जुड़े गुणधर्म।

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


पूरे इंडेक्स को मेमोरी में लोड करता है।
इंडेक्स में किए गए किसी भी परिवर्तन को मूल फ़ोल्डर में स्वचालित रूप से सहेजा नहीं जाता।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर पथ। |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


पूरे इंडेक्स को मेमोरी में लोड करता है।
इंडेक्स में किए गए किसी भी परिवर्तन को मूल फ़ोल्डर में स्वचालित रूप से सहेजा नहीं जाता।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर पथ। |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | इंडेक्स सेटिंग्स ऑब्जेक्ट। |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

