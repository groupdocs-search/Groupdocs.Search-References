---
title: "IndexRepository"
second_title: "GroupDocs.Search for Java API Reference"
description: "कई इंडेक्सों को संयोजित करने और उन पर सामान्य संचालन करने के लिए एक कंटेनर का प्रतिनिधित्व करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

कई इंडेक्सों को संयोजित करने और उन पर सामान्य संचालन करने के लिए एक कंटेनर का प्रतिनिधित्व करता है।


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // मौजूदा इंडेक्स लोड कर रहा है
repository.addToRepository(indexFolder2); // एक और मौजूदा इंडेक्स लोड कर रहा है
SearchResult result = repository.search(query); // रिपॉज़िटरी के इंडेक्स में खोज रहा है
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | नया उदाहरण प्रारंभ करता है |
IndexRepository
वर्ग।
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getEvents()](#getEvents--) | इवेंट्स की सदस्यता के लिए इवेंट हब प्राप्त करता है। |
|
|  | [getIndexes()](#getIndexes--) | इसमें शामिल इंडेक्स प्राप्त करता है। |
IndexRepository
.
|
|  | [close()](#close--) | द्वारा उपयोग किए गए सभी संसाधनों को रिलीज़ करता है |
IndexRepository
.
|
|  | [create()](#create--) | मेमोरी में एक नया इंडेक्स बनाता है। |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | मेमोरी में एक नया इंडेक्स बनाता है। |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | डिस्क पर एक नया इंडेक्स बनाता है। |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | डिस्क पर एक नया इंडेक्स बनाता है। |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | इंडेक्स रिपॉजिटरी में एक इंडेक्स जोड़ता है। |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | इंडेक्स रिपॉजिटरी में एक इंडेक्स खोलता और जोड़ता है। |
|
|  | [update()](#update--) | रिपॉजिटरी में सभी इंडेक्स को अपडेट करता है। |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | रिपॉजिटरी में सभी इंडेक्स को अपडेट करता है। |
|
|  | [search(String query)](#search-java.lang.String-) | रिपॉजिटरी के सभी इंडेक्स में खोज करता है। |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | रिपॉजिटरी के सभी इंडेक्स में खोज करता है। |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | रिपॉजिटरी के सभी इंडेक्स में खोज करता है। |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | रिपॉजिटरी के सभी इंडेक्स में खोज करता है। |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


नया उदाहरण प्रारंभ करता है
IndexRepository
वर्ग।


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


इवेंट्स की सदस्यता के लिए इवेंट हब प्राप्त करता है।


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


इसमें शामिल इंडेक्स प्राप्त करता है।
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - इंडेक्स।

### close() {#close--}
```
public final void close()
```


द्वारा उपयोग किए गए सभी संसाधनों को रिलीज़ करता है
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


मेमोरी में एक नया इंडेक्स बनाता है।


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से मेमोरी में एक इंडेक्स कैसे बनाया जाए।

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


मेमोरी में एक नया इंडेक्स बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | इंडेक्स सेटिंग्स। |

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से मेमोरी में एक इंडेक्स कैसे बनाया जाए।

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // इंडेक्सिंग के दौरान स्टॉप वर्ड्स के उपयोग को निष्क्रिय करना
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


डिस्क पर एक नया इंडेक्स बनाता है।
इंडेक्स निर्माण से पहले इंडेक्स फ़ोल्डर साफ़ किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर। |

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से डिस्क पर एक इंडेक्स कैसे बनाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


डिस्क पर एक नया इंडेक्स बनाता है।
इंडेक्स निर्माण से पहले इंडेक्स फ़ोल्डर साफ़ किया जाएगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर। |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | इंडेक्स सेटिंग्स। |

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी के माध्यम से डिस्क पर एक इंडेक्स कैसे बनाया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // इंडेक्सिंग के दौरान स्टॉप वर्ड्स के उपयोग को निष्क्रिय करना
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


इंडेक्स रिपॉजिटरी में एक इंडेक्स जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | जोड़ने के लिए इंडेक्स। |

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी में एक इंडेक्स कैसे जोड़ा जाए।

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


इंडेक्स रिपॉजिटरी में एक इंडेक्स खोलता और जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexFolder | java.lang.String | इंडेक्स फ़ोल्डर। |

उदाहरण दर्शाता है कि इंडेक्स रिपॉजिटरी में एक इंडेक्स कैसे जोड़ा जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


रिपॉजिटरी में सभी इंडेक्स को अपडेट करता है।

उदाहरण यह दर्शाता है कि रिपॉज़िटरी में इंडेक्स को कैसे अपडेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // इंडेक्स बनाना
index.add(documentsFolder); // दस्तावेज़ों को इंडेक्स करना
// दस्तावेज़ फ़ोल्डर से दस्तावेज़ हटाएँ या उन्हें संशोधित करें या फ़ोल्डर में नए दस्तावेज़ जोड़ें
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


रिपॉजिटरी में सभी इंडेक्स को अपडेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | अपडेट विकल्प। |

उदाहरण यह दर्शाता है कि रिपॉज़िटरी में इंडेक्स को कैसे अपडेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // इंडेक्स बनाना
index.add(documentsFolder); // दस्तावेज़ों को इंडेक्स करना
// दस्तावेज़ फ़ोल्डर से दस्तावेज़ हटाएँ या उन्हें संशोधित करें या फ़ोल्डर में नए दस्तावेज़ जोड़ें
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // इंडेक्सिंग थ्रेड्स की संख्या सेट करना
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


रिपॉजिटरी के सभी इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | क्वेरी | java.lang.String | सर्च क्वेरी। |

उदाहरण यह दर्शाता है कि इंडेक्स रिपॉज़िटरी में खोज कैसे की जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // इंडेक्स बनाना
index.add(documentsFolder); // दस्तावेज़ों को इंडेक्स करना
SearchResult result = repository.search(query); // खोज कर रहा है
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


रिपॉजिटरी के सभी इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | क्वेरी | java.lang.String | सर्च क्वेरी। |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |

उदाहरण यह दर्शाता है कि इंडेक्स रिपॉज़िटरी में खोज कैसे की जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // इंडेक्स बनाना
index.add(documentsFolder); // दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // केस-सेंसिटिव सर्च का फ़्लैग सेट करना
SearchResult result = repository.search(query, options); // खोज कर रहा है
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


रिपॉजिटरी के सभी इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | सर्च क्वेरी। |

उदाहरण यह दर्शाता है कि इंडेक्स रिपॉज़िटरी में खोज कैसे की जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // इंडेक्स बनाना
index.add(documentsFolder); // दस्तावेज़ों को इंडेक्स करना
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // ऑब्जेक्ट रूप में सर्च क्वेरी बनाना
SearchResult result = repository.search(query); // खोज कर रहा है
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


रिपॉजिटरी के सभी इंडेक्स में खोज करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | सर्च क्वेरी। |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |

उदाहरण यह दर्शाता है कि इंडेक्स रिपॉज़िटरी में खोज कैसे की जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // इंडेक्स बनाना
index.add(documentsFolder); // दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // केस-सेंसिटिव सर्च का फ़्लैग सेट करना
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // ऑब्जेक्ट रूप में सर्च क्वेरी बनाना
SearchResult result = repository.search(query, options); // खोज कर रहा है
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

