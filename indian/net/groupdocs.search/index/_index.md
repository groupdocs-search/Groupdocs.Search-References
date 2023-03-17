---
title: Index
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: इंडेक्संग दस्तवेजं के लए मुख्य वर्ग क प्रतनधत्व करत है और उनके मध्यम से खज करत है
type: docs
weight: 680
url: /hi/net/groupdocs.search/index/
---
## Index class

इंडेक्सिंग दस्तावेजों के लिए मुख्य वर्ग का प्रतिनिधित्व करता है और उनके माध्यम से खोज करता है।

```csharp
public class Index : IDisposable
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Index](index#constructor)() | का एक नया उदाहरण प्रारंभ करता है[`Index`](../index) वर्ग स्मृति में. |
| [Index](index#constructor_1)(IndexSettings) | का एक नया उदाहरण प्रारंभ करता है[`Index`](../index) विशेष अनुक्रमणिका सेटिंग्स के साथ स्मृति में वर्ग। |
| [Index](index#constructor_2)(string) | का एक नया उदाहरण प्रारंभ करता है[`Index`](../index) class. एक नया बनाता है या डिस्क पर एक मौजूदा इंडेक्स खोलता है। |
| [Index](index#constructor_3)(string, bool) | का एक नया उदाहरण प्रारंभ करता है[`Index`](../index) class. यदि डिस्क से मौजूदा इंडेक्स लोड करता है*overwriteIfExists* है`असत्य`; अन्यथा डिस्क पर एक नया इंडेक्स बनाता है। |
| [Index](index#constructor_4)(string, IndexSettings) | का एक नया उदाहरण प्रारंभ करता है[`Index`](../index) class. विशेष सेटिंग्स के साथ एक नया इंडेक्स बनाता है या डिस्क पर एक मौजूदा इंडेक्स खोलता है। |
| [Index](index#constructor_5)(string, IndexSettings, bool) | का एक नया उदाहरण प्रारंभ करता है[`Index`](../index) class. यदि डिस्क से मौजूदा इंडेक्स लोड करता है*overwriteIfExists* है`असत्य` ; विशेष अनुक्रमणिका सेटिंग के साथ डिस्क पर एक नया अनुक्रमणिका बनाता है अन्यथा. |

## गुण

| नाम | विवरण |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | डिक्शनरी रिपॉजिटरी प्राप्त करता है। |
| [Events](../../groupdocs.search/index/events) { get; } | ईवेंट की सदस्यता के लिए ईवेंट हब प्राप्त करता है। |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | सूचकांक पर बुनियादी जानकारी प्राप्त करता है। |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | इंडेक्स सेटिंग्स प्राप्त करता है। |
| [Repository](../../groupdocs.search/index/repository) { get; } | इंडेक्स रिपोजिटरी ऑब्जेक्ट प्राप्त करता है यदि इंडेक्स इसमें शामिल है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | इंडेक्सिंग ऑपरेशन करता है। एक फ़ाइल या फ़ोल्डर को एक पूर्ण या सापेक्ष पथ से जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा। |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | इंडेक्सिंग ऑपरेशन करता है। एक पूर्ण या सापेक्ष पथ से फ़ाइलें या फ़ोल्डर जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा। |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़ जोड़ता है। |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। निकाले गए डेटा को इंडेक्स में जोड़ता है। |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। एक फ़ाइल या फ़ोल्डर को एक पूर्ण या सापेक्ष पथ से जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा। |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। एक पूर्ण या सापेक्ष पथ से फ़ाइलें या फ़ोल्डर जोड़ता है। सभी सबफ़ोल्डर्स के दस्तावेज़ों को अनुक्रमित किया जाएगा। |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | अपडेट ऑपरेशन के दौरान पुन: अनुक्रमण किए बिना अनुक्रमित दस्तावेज़ों में विशेषता परिवर्तनों के निर्दिष्ट बैच को लागू करता है। |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | अनुक्रमणिका से अनुक्रमित फ़ाइलों या फ़ोल्डरों को हटाता है। फिर हटाए गए पथों के बिना इंडेक्स को अपडेट करता है। |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | धाराओं या संरचनाओं से अनुक्रमित दस्तावेजों को हटाता है। फिर हटाए गए दस्तावेज़ों के बिना अनुक्रमणिका को अद्यतन करता है. |
| [Dispose](../../groupdocs.search/index/dispose)() | द्वारा उपयोग किए गए सभी संसाधनों को जारी करता है[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | निर्दिष्ट अनुक्रमित दस्तावेज़ से जुड़ी सभी विशेषताओं को प्राप्त करता है। |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | अनुक्रमित दस्तावेज़ के लिए HTML स्वरूपित पाठ उत्पन्न करता है और इसे आउटपुट एडेप्टर के माध्यम से स्थानांतरित करता है। |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | अनुक्रमित दस्तावेज़ के लिए HTML स्वरूपित पाठ उत्पन्न करता है और इसे आउटपुट एडेप्टर के माध्यम से स्थानांतरित करता है। |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | निर्दिष्ट दस्तावेज़ के नेस्टेड आइटम की एक सरणी प्राप्त करता है (कंटेनर दस्तावेज़ जैसे ZIP, OST, PST के लिए)। |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | सभी अनुक्रमित दस्तावेज़ों की एक सरणी प्राप्त करता है। |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | अनुक्रमित पथों की एक सरणी प्राप्त करता है - दस्तावेज़ या फ़ोल्डर। |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | इंडेक्सिंग ऑपरेशंस पर रिपोर्ट प्राप्त करता है। |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | खोज कार्यों पर रिपोर्ट प्राप्त करता है। |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | हाइलाइट किए गए शब्दों के साथ HTML स्वरूपित पाठ उत्पन्न करता है। |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | हाइलाइट किए गए शब्दों के साथ HTML स्वरूपित पाठ उत्पन्न करता है। |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | निर्दिष्ट इंडेक्स को वर्तमान इंडेक्स में मर्ज करता है। ध्यान दें कि अन्य इंडेक्स नहीं बदला जाएगा। |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | निर्दिष्ट इंडेक्स रिपॉजिटरी से इंडेक्स को वर्तमान इंडेक्स में मर्ज करता है। ध्यान दें कि रिपॉजिटरी में इंडेक्स नहीं बदला जाएगा। |
| [Notify](../../groupdocs.search/index/notify)(Notification) | अधिसूचना करने के लिए निर्दिष्ट अधिसूचना वस्तु को सूचकांक में पास करता है। |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | इंडेक्स सेगमेंट को एक दूसरे के साथ मर्ज करके संख्या को कम करता है। यह ऑपरेशन खोज प्रदर्शन में सुधार करता है। |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | इंडेक्स सेगमेंट को एक दूसरे के साथ मर्ज करके संख्या को कम करता है। यह ऑपरेशन खोज प्रदर्शन में सुधार करता है। |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | इंडेक्स में खोजता है। |
| [Search](../../groupdocs.search/index/search#search_3)(string) | इंडेक्स में खोजता है। |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | इंडेक्स में रिवर्स इमेज सर्च करता है। |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | इंडेक्स में खोजता है। |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | इंडेक्स में खोजता है। |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | मेथड सर्च के साथ शुरू हुई चंक सर्च को जारी रखता है। |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | मेथड सर्च के साथ शुरू हुई चंक सर्च को जारी रखता है। |
| [Update](../../groupdocs.search/index/update#update)() | उन दस्तावेज़ों को पुन: अनुक्रमित करता है जिन्हें पिछले अपडेट के बाद से बदल दिया गया है या हटा दिया गया है। उन नई फ़ाइलों को जोड़ता है जिन्हें अनुक्रमित फ़ोल्डर में जोड़ा गया है। |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | उन दस्तावेज़ों को पुन: अनुक्रमित करता है जिन्हें पिछले अपडेट के बाद से बदल दिया गया है या हटा दिया गया है। उन नई फ़ाइलों को जोड़ता है जिन्हें अनुक्रमित फ़ोल्डर में जोड़ा गया है। |

### टिप्पणियों

**और अधिक जानें**

* [एक सूचकांक बनाना](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [इंडेक्सिंग](https://docs.groupdocs.com/display/searchnet/Indexing)
* [खोज कर](https://docs.groupdocs.com/display/searchnet/Searching)

### उदाहरण

उदाहरण वर्ग के एक विशिष्ट उपयोग को प्रदर्शित करता है।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

SearchResult result = index.Search(query); // इंडेक्स में खोजा जा रहा है
```

### यह सभी देखें

* नाम स्थान [GroupDocs.Search](../../groupdocs.search)
* सभा [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
