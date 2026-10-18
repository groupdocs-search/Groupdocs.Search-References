---
title: "Index"
second_title: "GroupDocs.Search .NET के लिए API Reference"
description: "दस्तावेज़ों को इंडेक्स करने और उन पर खोज करने के लिए मुख्य क्लास का प्रतिनिधित्व करता है।"
type: docs
weight: 700
url: /hi/net/groupdocs.search/index/
---
## Index class

दस्तावेज़ों को इंडेक्स करने और उन पर खोज करने के लिए मुख्य क्लास का प्रतिनिधित्व करता है।

```csharp
public class Index : IDisposable
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [Index](index#constructor)() | मेमोरी में एक नया उदाहरण प्रारंभ करता है [`Index`](../index) वर्ग का। |
| [Index](index#constructor_1)(IndexSettings) | विशिष्ट इंडेक्स सेटिंग्स के साथ मेमोरी में एक नया उदाहरण प्रारंभ करता है [`Index`](../index) वर्ग का। |
| [Index](index#constructor_2)(string) | एक नया उदाहरण प्रारंभ करता है [`Index`](../index) वर्ग का। डिस्क पर एक नया इंडेक्स बनाता है या मौजूदा इंडेक्स खोलता है। |
| [Index](index#constructor_3)(string, bool) | एक नया उदाहरण प्रारंभ करता है [`Index`](../index) वर्ग का। यदि *overwriteIfExists* `false` है तो डिस्क से मौजूदा इंडेक्स लोड करता है; अन्यथा डिस्क पर एक नया इंडेक्स बनाता है। |
| [Index](index#constructor_4)(string, IndexSettings) | नया [`Index`](../index) क्लास का उदाहरण प्रारंभ करता है। विशिष्ट सेटिंग्स के साथ नया इंडेक्स बनाता है या डिस्क पर मौजूदा इंडेक्स खोलता है। |
| [Index](index#constructor_5)(string, IndexSettings, bool) | नया [`Index`](../index) क्लास का उदाहरण प्रारंभ करता है। यदि *overwriteIfExists* `false` है तो डिस्क से मौजूदा इंडेक्स लोड करता है; अन्यथा विशिष्ट इंडेक्स सेटिंग्स के साथ डिस्क पर नया इंडेक्स बनाता है। |

## गुण

| नाम | विवरण |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | डिक्शनरी रिपॉज़िटरी प्राप्त करता है। |
| [Events](../../groupdocs.search/index/events) { get; } | इवेंट्स की सदस्यता लेने के लिए इवेंट हब प्राप्त करता है। |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | इंडेक्स की मूल जानकारी प्राप्त करता है। |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | इंडेक्स सेटिंग्स प्राप्त करता है। |
| [Repository](../../groupdocs.search/index/repository) { get; } | यदि इंडेक्स उसमें सम्मिलित है तो इंडेक्स रिपॉज़िटरी ऑब्जेक्ट प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | पूरे इंडेक्स को मेमोरी में लोड करता है। इंडेक्स में किए गए किसी भी परिवर्तन को मूल फ़ोल्डर में स्वतः सहेजा नहीं जाता। |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | पूरे इंडेक्स को मेमोरी में लोड करता है। इंडेक्स में किए गए किसी भी परिवर्तन को मूल फ़ोल्डर में स्वतः सहेजा नहीं जाता। |
| [Add](../../groupdocs.search/index/add#add_2)(string) | इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा। |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइलें या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा। |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़ जोड़ता है। |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। निकाले गए डेटा को इंडेक्स में जोड़ता है। |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइल या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा। |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | इंडेक्सिंग ऑपरेशन करता है। पूर्ण या सापेक्ष पथ द्वारा फ़ाइलें या फ़ोल्डर जोड़ता है। सभी उपफ़ोल्डरों की दस्तावेज़ों को इंडेक्स किया जाएगा। |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | अपडेट ऑपरेशन के दौरान पुनः इंडेक्सिंग किए बिना निर्दिष्ट एट्रिब्यूट परिवर्तन बैच को इंडेक्स किए गए दस्तावेज़ों पर लागू करता है। |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | डिस्क पर क्षतिग्रस्त सेगमेंट फ़ाइलों के लिए इंडेक्स की जाँच करता है। यदि *fixIndexFunctionality* `true` है तो यह विधि क्षतिग्रस्त सेगमेंट की उपस्थिति में इंडेक्स कार्यक्षमता को ठीक करती है; अन्यथा नहीं करती। |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | इंडेक्स से इंडेक्स किए गए फ़ाइलों या फ़ोल्डरों को हटाता है। फिर हटाए गए पथों के बिना इंडेक्स को अपडेट करता है। ध्यान दें कि यदि कोई दस्तावेज़ फ़ोल्डर के हिस्से के रूप में इंडेक्स में जोड़ा गया था तो उसे व्यक्तिगत रूप से हटाया नहीं जा सकता। |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | स्ट्रीम या संरचनाओं से इंडेक्स किए गए दस्तावेज़ों को हटाता है। फिर हटाए गए दस्तावेज़ों के बिना इंडेक्स को अपडेट करता है। |
| [Dispose](../../groupdocs.search/index/dispose)() | [`Index`](../index) द्वारा उपयोग किए गए सभी संसाधनों को मुक्त करता है। |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | निर्दिष्ट इंडेक्स किए गए दस्तावेज़ से जुड़े सभी एट्रिब्यूट प्राप्त करता है। |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | एक इंडेक्स किए गए दस्तावेज़ का टेक्स्ट उत्पन्न करता है और उसे आउटपुट एडाप्टर के माध्यम से भेजता है। |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | इंडेक्स किए गए दस्तावेज़ के लिए HTML स्वरूपित टेक्स्ट उत्पन्न करता है और उसे आउटपुट एडाप्टर के माध्यम से स्थानांतरित करता है। |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | दस्तावेज़ कुंजी द्वारा एक इंडेक्स किया गया दस्तावेज़ प्राप्त करता है। |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | निर्दिष्ट दस्तावेज़ के नेस्टेड आइटमों की एक एरे प्राप्त करता है (जैसे ZIP, OST, PST जैसे कंटेनर दस्तावेज़ों के लिए)। |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | सभी इंडेक्स किए गए दस्तावेज़ों की एक एरे प्राप्त करता है। |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | इंडेक्स किए गए पथों की एक एरे प्राप्त करता है - दस्तावेज़ या फ़ोल्डर। |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | इंडेक्सिंग ऑपरेशनों पर रिपोर्ट प्राप्त करता है। |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | खोज ऑपरेशनों पर रिपोर्ट प्राप्त करता है। |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | हाइलाइट किए गए पाए गए शब्दों के साथ HTML स्वरूपित पाठ उत्पन्न करता है। |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | हाइलाइट किए गए पाए गए शब्दों के साथ HTML स्वरूपित पाठ उत्पन्न करता है। |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | निर्दिष्ट सूचकांक को वर्तमान सूचकांक में मिलाता है। ध्यान दें कि अन्य सूचकांक नहीं बदलेगा। |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | निर्दिष्ट सूचकांक रिपॉजिटरी से सूचकांकों को वर्तमान सूचकांक में मिलाता है। ध्यान दें कि रिपॉजिटरी में सूचकांक नहीं बदलेगा। |
| [Notify](../../groupdocs.search/index/notify)(Notification) | सूचना देने के लिए निर्दिष्ट नोटिफिकेशन ऑब्जेक्ट को सूचकांक को पास करता है। |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | उन्हें एक-दूसरे के साथ मिलाकर सूचकांक खंडों की संख्या को न्यूनतम करता है। यह ऑपरेशन खोज प्रदर्शन को सुधारता है। |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | उन्हें एक-दूसरे के साथ मिलाकर सूचकांक खंडों की संख्या को न्यूनतम करता है। यह ऑपरेशन खोज प्रदर्शन को सुधारता है। |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | इन-मेमोरी सूचकांक को डिस्क पर सहेजता है। नियमित सूचकांक को भी किसी अन्य फ़ोल्डर में सहेजता है। यह सूचकांक की सेटिंग्स को नहीं बदलता। |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | सूचकांक में खोज करता है। |
| [Search](../../groupdocs.search/index/search#search_3)(string) | सूचकांक में खोज करता है। |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | सूचकांक में रिवर्स इमेज सर्च करता है। |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | सूचकांक में खोज करता है। |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | सूचकांक में खोज करता है। |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | मेथड Search से शुरू किए गए चंक सर्च को जारी रखता है। |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | मेथड Search से शुरू किए गए चंक सर्च को जारी रखता है। |
| [Update](../../groupdocs.search/index/update#update)() | पिछले अपडेट के बाद बदलें या हटाए गए दस्तावेज़ों को पुनः-सूचकांकित करता है। सूचकांकित फ़ोल्डरों में जोड़ी गई नई फ़ाइलों को जोड़ता है। |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | पिछले अपडेट के बाद बदलें या हटाए गए दस्तावेज़ों को पुनः-सूचकांकित करता है। सूचकांकित फ़ोल्डरों में जोड़ी गई नई फ़ाइलों को जोड़ता है। |

### टिप्पणियाँ

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### उदाहरण

यह उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### संबंधित देखें

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- संपादित न करें: generated by xmldocmd GroupDocs.search.dll के लिए -->
