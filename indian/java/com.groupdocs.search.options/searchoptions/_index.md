---
title: "SearchOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "सर्च ऑपरेशन के लिए विकल्प प्रदान करता है।"
type: docs
weight: 34
url: /hi/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

सर्च ऑपरेशन के लिए विकल्प प्रदान करता है।


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | SearchOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | SearchOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | खोज में समानार्थक शब्दों के उपयोग का फ़्लैग प्राप्त करता है। |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | खोज में समानार्थक शब्दों के उपयोग का फ़्लैग सेट करता है। |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | खोज में होमोफोन के उपयोग का फ़्लैग प्राप्त करता है। |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | खोज में होमोफोन के उपयोग का फ़्लैग सेट करता है। |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | खोज में विभिन्न शब्द रूपों के उपयोग का फ़्लैग प्राप्त करता है। |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | खोज में विभिन्न शब्द रूपों के उपयोग का फ़्लैग सेट करता है। |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | पाए गए दस्तावेज़ों से जुड़े गुणों को पुनः प्राप्त करने का फ़्लैग प्राप्त करता है। |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | पाए गए दस्तावेज़ों से जुड़े गुणों को प्राप्त करने का फ़्लैग सेट करता है। |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | फ़ज़ी खोज विकल्प प्राप्त करता है। |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | वर्तनी सुधारक विकल्प प्राप्त करता है। |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | कीबोर्ड लेआउट सुधारक विकल्प प्राप्त करता है। |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | केस-सेंसिटिव खोज का फ़्लैग प्राप्त करता है। |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | केस-सेंसिटिव खोज का फ़्लैग सेट करता है। |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | खोज क्वेरी में सभी शब्दों की कुल अधिकतम आवृत्ति संख्या प्राप्त करता है। |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | खोज क्वेरी में सभी शब्दों की कुल अधिकतम आवृत्ति संख्या सेट करता है। |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | खोज क्वेरी में प्रत्येक शब्द की अधिकतम आवृत्ति संख्या प्राप्त करता है। |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | खोज क्वेरी में प्रत्येक शब्द की अधिकतम आवृत्ति संख्या सेट करता है। |
|
|  | [getDateFormats()](#getDateFormats--) | तारीख रेंज खोज के लिए तारीख फ़ॉर्मैट्स का संग्रह प्राप्त करता है। |
|
|  | [isChunkSearch()](#isChunkSearch--) | चंक्स द्वारा खोज का फ़्लैग प्राप्त करता है। |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | चंक्स द्वारा खोज का फ़्लैग सेट करता है। |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | सर्च दस्तावेज़ फ़िल्टर प्राप्त करता है। |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | खोज दस्तावेज़ फ़िल्टर सेट करता है। |
|
|  | [getCancellation()](#getCancellation--) | ऑपरेशन रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | ऑपरेशन रद्द करने वाले ऑब्जेक्ट को सेट करता है। |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


SearchOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


SearchOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


खोज में समानार्थक शब्दों के उपयोग का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
बूलियन - खोज में समानार्थक शब्दों के उपयोग का फ़्लैग।

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


खोज में समानार्थक शब्दों के उपयोग का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | खोज में समानार्थक शब्दों के उपयोग का फ़्लैग। |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


खोज में होमोफोन के उपयोग का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
बूलियन - खोज में होमोफोन के उपयोग का फ़्लैग।

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


खोज में होमोफोन के उपयोग का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | खोज में होमोफोन के उपयोग का फ़्लैग। |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


खोज में विभिन्न शब्द रूपों के उपयोग का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
बूलियन - खोज में विभिन्न शब्द रूपों के उपयोग का फ़्लैग।

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


खोज में विभिन्न शब्द रूपों के उपयोग का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | खोज में विभिन्न शब्द रूपों के उपयोग का फ़्लैग। |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


पाए गए दस्तावेज़ों से जुड़े गुणों को पुनः प्राप्त करने के फ़्लैग को प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - पाए गए दस्तावेज़ों से जुड़े गुणों को पुनः प्राप्त करने का फ़्लैग।

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


पाए गए दस्तावेज़ों से जुड़े गुणों को पुनः प्राप्त करने के फ़्लैग को सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | पाए गए दस्तावेज़ों से जुड़े गुणों को पुनः प्राप्त करने का फ़्लैग। |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


फ़ज़ी खोज विकल्प प्राप्त करता है।


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


वर्तनी सुधारक विकल्प प्राप्त करता है।


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


कीबोर्ड लेआउट सुधारक विकल्प प्राप्त करता है।


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


केस-सेंसिटिव खोज का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - केस-सेंसिटिव खोज का फ़्लैग।

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


केस-सेंसिटिव खोज का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | केस-सेंसिटिव खोज का फ़्लैग। |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


खोज क्वेरी में सभी शब्दों की कुल अधिकतम आवृत्तियों की संख्या प्राप्त करता है। डिफ़ॉल्ट मान 500000 है।


**Returns:**
int - कुल अधिकतम आवृत्तियों की संख्या।

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


खोज क्वेरी में सभी शब्दों की कुल अधिकतम आवृत्तियों की संख्या सेट करता है। डिफ़ॉल्ट मान 500000 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | कुल अधिकतम आवृत्तियों की संख्या। |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


खोज क्वेरी में प्रत्येक शब्द की अधिकतम आवृत्तियों की संख्या प्राप्त करता है। डिफ़ॉल्ट मान 100000 है।


**Returns:**
int - खोज क्वेरी में प्रत्येक शब्द की अधिकतम आवृत्तियों की संख्या।

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


खोज क्वेरी में प्रत्येक शब्द की अधिकतम आवृत्तियों की संख्या सेट करता है। डिफ़ॉल्ट मान 100000 है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | int | खोज क्वेरी में प्रत्येक शब्द की अधिकतम आवृत्तियों की संख्या। |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


डेट रेंज खोज के लिए तिथि स्वरूपों का संग्रह प्राप्त करता है। डिफ़ॉल्ट तिथि स्वरूप 'dd.MM.yyyy', 'MM/dd/yyyy', और 'yyyy-MM-dd' हैं।


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


उदाहरण दर्शाता है कि खोज के लिए तिथि स्वरूप कैसे सेट करें।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // डिफ़ॉल्ट तिथि स्वरूप हटाना
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// 'MM/dd/yyyy' पैटर्न बनाते हुए तिथि स्वरूप बनाना
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // इंडेक्स में खोजें
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


चंक्स द्वारा खोज का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - चंक्स द्वारा खोज का फ़्लैग।

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


चंक्स द्वारा खोज का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | चंक्स द्वारा खोज का फ़्लैग। |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


खोज दस्तावेज़ फ़िल्टर प्राप्त करता है। SearchDocumentFilter समावेशन लॉजिक पर काम करता है। खोज दस्तावेज़ फ़िल्टर इंस्टेंस बनाने के लिए SearchDocumentFilter क्लास का उपयोग करें। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि सभी पाए गए दस्तावेज़ लौटाए जाएंगे।


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


उदाहरण दर्शाता है कि डॉक्यूमेंट फ़िल्टर कैसे सेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder);
// एक्सटेंशन '.doc', '.docx', '.rtf' वाले दस्तावेज़ों को छोड़ने वाला सर्च डॉक्यूमेंट फ़िल्टर बनाना
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // फ़ाइल एक्सटेंशन फ़िल्टर बनाना
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // फ़ाइल एक्सटेंशन फ़िल्टर को उलटना
options.setSearchDocumentFilter(invertedFilter);
// इंडेक्स में खोज
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


सर्च डॉक्यूमेंट फ़िल्टर सेट करता है।  SearchDocumentFilter  समावेशन लॉजिक पर काम करता है। SearchDocumentFilter क्लास का उपयोग सर्च डॉक्यूमेंट फ़िल्टर इंस्टेंस बनाने के लिए करें। डिफ़ॉल्ट मान null है, जिसका अर्थ है कि सभी पाए गए दस्तावेज़ वापस किए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | सर्च डॉक्यूमेंट फ़िल्टर। |


उदाहरण दर्शाता है कि डॉक्यूमेंट फ़िल्टर कैसे सेट किया जाए।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder);
// एक्सटेंशन '.doc', '.docx', '.rtf' वाले दस्तावेज़ों को छोड़ने वाला सर्च डॉक्यूमेंट फ़िल्टर बनाना
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // फ़ाइल एक्सटेंशन फ़िल्टर बनाना
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // फ़ाइल एक्सटेंशन फ़िल्टर को उलटना
options.setSearchDocumentFilter(invertedFilter);
// इंडेक्स में खोज
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


ऑपरेशन रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। डिफ़ॉल्ट मान null है।


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


ऑपरेशन रद्द करने वाले ऑब्जेक्ट को सेट करता है। डिफ़ॉल्ट मान null है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | ऑपरेशन रद्द करने वाला ऑब्जेक्ट। |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
