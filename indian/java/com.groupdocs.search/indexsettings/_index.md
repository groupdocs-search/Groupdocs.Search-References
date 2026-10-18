---
title: "IndexSettings"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स सेटिंग्स का प्रतिनिधित्व करता है जो इंडेक्सिंग संचालन को अनुकूलित करने की अनुमति देती हैं।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

इंडेक्स सेटिंग्स का प्रतिनिधित्व करता है जो इंडेक्सिंग संचालन को अनुकूलित करने की अनुमति देती हैं।


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // इंडेक्स प्रकार सेट कर रहा है
Index index = new Index(indexFolder, settings); // एक इंडेक्स बना रहा है
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | IndexSettings क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | एक मान प्राप्त करता है जो दर्शाता है कि इंडेक्स मेमोरी में संग्रहीत है या डिस्क पर। |
|
|  | [getUseStopWords()](#getUseStopWords--) | एक मान प्राप्त करता है जो दर्शाता है कि स्टॉप शब्दों का उपयोग करना है या नहीं। |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | एक मान सेट करता है जो दर्शाता है कि स्टॉप शब्दों का उपयोग करना है या नहीं। |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | इंडेक्सिंग रिपोर्टों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | इंडेक्सिंग रिपोर्टों की अधिकतम संख्या सेट करता है। |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | खोज रिपोर्टों की अधिकतम संख्या प्राप्त करता है। |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | खोज रिपोर्टों की अधिकतम संख्या सेट करता है। |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | एक मान प्राप्त करता है जो दर्शाता है कि अक्षर प्रतिस्थापन का उपयोग करना है या नहीं। |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | एक मान सेट करता है जो दर्शाता है कि अक्षर प्रतिस्थापन का उपयोग करना है या नहीं। |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | एक दस्तावेज़ फ़िल्टर प्राप्त करता है। |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | एक दस्तावेज़ फ़िल्टर सेट करता है। |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | पाठ संग्रह सेटिंग्स प्राप्त करता है। |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | पाठ संग्रह सेटिंग्स सेट करता है। |
|
|  | [getIndexType()](#getIndexType--) | इंडेक्स प्रकार प्राप्त करता है। |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | इंडेक्स प्रकार सेट करता है। |
|
|  | [getSearchThreads()](#getSearchThreads--) | खोज के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या प्राप्त करता है। |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | खोज के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या सेट करता है। |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | कस्टम एक्सट्रैक्टर संग्रह प्राप्त करता है। |
|
|  | [getLogger()](#getLogger--) | इंडेक्स में घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किए जाने वाले लॉगर को प्राप्त करता है। |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | इंडेक्स में घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किए जाने वाले लॉगर को सेट करता है। |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


IndexSettings क्लास का एक नया उदाहरण प्रारंभ करता है।


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


एक मान प्राप्त करता है जो दर्शाता है कि इंडेक्स मेमोरी में संग्रहीत है या डिस्क पर।


**Returns:**
boolean - एक मान जो दर्शाता है कि इंडेक्स मेमोरी में संग्रहीत है या डिस्क पर।

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


स्टॉप शब्दों का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान true है।


**Returns:**
boolean - एक मान जो दर्शाता है कि स्टॉप शब्दों का उपयोग करना है या नहीं।

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


स्टॉप शब्दों का उपयोग करना है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान true है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | स्टॉप शब्दों का उपयोग करना है या नहीं, यह दर्शाने वाला मान। |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


इंडेक्सिंग रिपोर्टों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान 5 है।


**Returns:**
int - इंडेक्सिंग रिपोर्टों की अधिकतम संख्या।

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


इंडेक्सिंग रिपोर्टों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान 5 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | इंडेक्सिंग रिपोर्टों की अधिकतम संख्या। |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


सर्च रिपोर्टों की अधिकतम संख्या प्राप्त करता है। डिफ़ॉल्ट मान 10 है।


**Returns:**
int - सर्च रिपोर्टों की अधिकतम संख्या।

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


सर्च रिपोर्टों की अधिकतम संख्या सेट करता है। डिफ़ॉल्ट मान 10 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | सर्च रिपोर्टों की अधिकतम संख्या। |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


कैरेक्टर रिप्लेसमेंट का उपयोग करना है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - एक मान जो दर्शाता है कि कैरेक्टर रिप्लेसमेंट का उपयोग करना है या नहीं।

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


कैरेक्टर रिप्लेसमेंट का उपयोग करना है या नहीं, यह दर्शाने वाला मान सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | कैरेक्टर रिप्लेसमेंट का उपयोग करना है या नहीं, यह दर्शाने वाला मान। |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


डॉक्यूमेंट फ़िल्टर प्राप्त करता है। DocumentFilter समावेशन लॉजिक पर काम करता है। डॉक्यूमेंट फ़िल्टर इंस्टेंस बनाने के लिए DocumentFilter क्लास का उपयोग करें। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि सभी जोड़े गए दस्तावेज़ इंडेक्स किए जाते हैं।


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

उदाहरण दर्शाता है कि डॉक्यूमेंट फ़िल्टर कैसे सेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक्सटेंशन '.doc', '.docx', '.rtf' वाले दस्तावेज़ों को छोड़ने वाला फ़िल्टर बनाना
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // फ़ाइल एक्सटेंशन फ़िल्टर बनाना
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // फ़ाइल एक्सटेंशन फ़िल्टर को उलटना
settings.setDocumentFilter(invertedFilter);
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder, settings);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder);
// खोज करना
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


एक दस्तावेज़ फ़िल्टर सेट करता है। DocumentFilter समावेशन लॉजिक पर काम करता है। DocumentFilter उदाहरण बनाने के लिए GroupDocs.Search.Options.DocumentFilter क्लास का उपयोग करें। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि सभी जोड़े गए दस्तावेज़ इंडेक्स किए जाते हैं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | दस्तावेज़ फ़िल्टर। |

उदाहरण दर्शाता है कि डॉक्यूमेंट फ़िल्टर कैसे सेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// एक्सटेंशन '.doc', '.docx', '.rtf' वाले दस्तावेज़ों को छोड़ने वाला फ़िल्टर बनाना
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // फ़ाइल एक्सटेंशन फ़िल्टर बनाना
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // फ़ाइल एक्सटेंशन फ़िल्टर को उलटना
settings.setDocumentFilter(invertedFilter);
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder, settings);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder);
// खोज करना
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


टेक्स्ट स्टोरेज सेटिंग्स प्राप्त करता है। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि दस्तावेज़ टेक्स्ट संग्रहीत नहीं होते।


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

उदाहरण दर्शाता है कि टेक्स्ट स्टोरेज सेटिंग्स कैसे सेट करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// इंडेक्स सेटिंग्स इंस्टेंस बनाना
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // इंडेक्स टेक्स्ट स्टोरेज के लिए उच्च संपीड़न स्तर सेट करना
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder, settings);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder);
// खोज करना
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


टेक्स्ट स्टोरेज सेटिंग्स सेट करता है। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि दस्तावेज़ टेक्स्ट संग्रहीत नहीं होते।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | टेक्स्ट स्टोरेज सेटिंग्स। |

उदाहरण दर्शाता है कि टेक्स्ट स्टोरेज सेटिंग्स कैसे सेट करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// इंडेक्स सेटिंग्स इंस्टेंस बनाना
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // इंडेक्स टेक्स्ट स्टोरेज के लिए उच्च संपीड़न स्तर सेट करना
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder, settings);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder);
// खोज करना
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


इंडेक्स प्रकार प्राप्त करता है। डिफ़ॉल्ट मान GroupDocs.Search.Options.IndexType.NormalIndex है।


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


इंडेक्स प्रकार सेट करता है। डिफ़ॉल्ट मान GroupDocs.Search.Options.IndexType.NormalIndex है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | इंडेक्स प्रकार। |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


खोज के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या प्राप्त करता है। डिफ़ॉल्ट मान GroupDocs.Search.Options.NumberOfThreads.Default है, जिसका अर्थ है कि खोज प्रोसेसर कोर की संख्या के बराबर थ्रेड्स का उपयोग करके की जाएगी।


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


खोज के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या सेट करता है। डिफ़ॉल्ट मान GroupDocs.Search.Options.NumberOfThreads.Default है, जिसका अर्थ है कि खोज प्रोसेसर कोर की संख्या के बराबर थ्रेड्स का उपयोग करके की जाएगी।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | खोज के लिए उपयोग किए जाने वाले थ्रेड्स की संख्या। |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


कस्टम एक्सट्रैक्टर संग्रह प्राप्त करता है। कस्टम एक्सट्रैक्टर को लागू करने का पूर्ण उदाहरण GroupDocs.Search.Common.IFieldExtractor इंटरफ़ेस के दस्तावेज़ में प्रस्तुत किया गया है।


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


इंडेक्स में घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किया जाने वाला लॉगर प्राप्त करता है। ध्यान दें कि लॉगर सहेजा नहीं जाता और प्रत्येक बार जब इंडेक्स बनाया या लोड किया जाता है, तो इसे बनाना और असाइन करना आवश्यक है।


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


इंडेक्स में घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किए जाने वाले लॉगर को सेट करता है। ध्यान दें कि लॉगर सहेजा नहीं जाता और प्रत्येक बार जब इंडेक्स बनाया या लोड किया जाता है, तब इसे बनाना और असाइन करना आवश्यक होता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | इंडेक्स में घटनाओं और त्रुटियों को लॉग करने के लिए उपयोग किया जाने वाला लॉगर। |
|

