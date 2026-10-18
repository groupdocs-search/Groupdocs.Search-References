---
title: "HighlightOptions"
second_title: "GroupDocs.Search .NET के लिए API Reference"
description: "पाए गए शब्दों को हाइलाइट करने के लिए विकल्प प्रदान करता है।"
type: docs
weight: 910
url: /hi/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

पाए गए शब्दों को हाइलाइट करने के लिए विकल्प प्रदान करता है।

```csharp
public class HighlightOptions : TextOptions
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [HighlightOptions](highlightoptions)() | नए उदाहरण को प्रारंभ करता है [`HighlightOptions`](../highlightoptions) क्लास का। |

## गुण

| नाम | विवरण |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | इंडेक्सिंग के लिए उपयोग किए गए अतिरिक्त दस्तावेज़ फ़ील्ड्स को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान `null` है। ध्यान दें कि यह मान केवल तब उपयोग किया जाता है जब दस्तावेज़ पाठ को इंडेक्स में सहेजा नहीं गया हो। |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | स्वचालित रूप से एन्कोडिंग का पता लगाने के लिए संकेत देने वाला मान प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान `false` है। |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | कैंसलेशन ऑब्जेक्ट को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान `null` है। |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | इंडेक्सिंग के लिए उपयोग किए गए कस्टम टेक्स्ट एक्सट्रैक्टर को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान `null` है। ध्यान दें कि यह मान केवल तब उपयोग किया जाता है जब दस्तावेज़ पाठ को इंडेक्स में सहेजा नहीं गया हो। |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | टेक्स्ट दस्तावेज़ों से टेक्स्ट निकालने के लिए उपयोग की गई एन्कोडिंग को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान `null` है, जिसका अर्थ है कि डिफ़ॉल्ट एन्कोडिंग UTF-8 उपयोग की जाती है। यदि AutoDetectEncoding `true` है तो यह मान डिफ़ॉल्ट एन्कोडिंग के रूप में उपयोग किया जाता है। |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | आउटपुट HTML में Head टैग उत्पन्न किया जाता है या नहीं, यह दर्शाने वाला मान प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान `true` है। |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | घटनाओं को हाइलाइट करने के लिए उपयोग किए जाने वाले रंग को प्राप्त करता है या सेट करता है। डिफ़ॉल्ट मान #FFD800 है। |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | रिवर्स इमेज सर्च के लिए इमेज इंडेक्सिंग विकल्प प्राप्त करता है। |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | मेटाडाटा फ़ील्ड्स को इंडेक्स करने के विकल्प प्राप्त करता है। |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | OCR प्रोसेसिंग और पहचाने गए टेक्स्ट को इंडेक्स करने के विकल्प प्राप्त करता है। |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | पाए गए शब्द को हाइलाइट करने के अंत टैग को प्राप्त करता या सेट करता है। यह टैग केवल प्लेन टेक्स्ट में हाइलाइट करने पर उपयोग किया जाता है। डिफ़ॉल्ट मान एक खाली स्ट्रिंग है। |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | पाए गए शब्द को हाइलाइट करने के शुरू टैग को प्राप्त करता या सेट करता है। यह टैग केवल प्लेन टेक्स्ट में हाइलाइट करने पर उपयोग किया जाता है। डिफ़ॉल्ट मान एक खाली स्ट्रिंग है। |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | हाइलाइट किए गए शब्द के बाद टेक्स्ट फ्रैगमेंट में शब्दों की अधिकतम संख्या को प्राप्त करता या सेट करता है। मान 0 से 10000 के बीच होना चाहिए। डिफ़ॉल्ट मान `7` है। |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | हाइलाइट किए गए शब्द से पहले टेक्स्ट फ्रैगमेंट में शब्दों की अधिकतम संख्या को प्राप्त करता या सेट करता है। मान 0 से 10000 के बीच होना चाहिए। डिफ़ॉल्ट मान `7` है। |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | टेक्स्ट फ्रैगमेंट में शब्दों की अधिकतम संख्या को प्राप्त करता या सेट करता है। मान 0 से 10000 के बीच होना चाहिए। डिफ़ॉल्ट मान `21` है। |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | एक मान प्राप्त करता या सेट करता है जो दर्शाता है कि प्रक्रिया को फ़ाइलों और डायरेक्टरीज़ तक पहुँचने के लिए SeBackupPrivilege और FILE_FLAG_BACKUP_SEMANTICS का उपयोग करना चाहिए या नहीं। डिफ़ॉल्ट मान `false` है। |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | एक मान प्राप्त करता या सेट करता है जो दर्शाता है कि घटनाओं को हाइलाइट करने के लिए इनलाइन स्टाइल्स का उपयोग किया जाता है या नहीं। डिफ़ॉल्ट मान `true` है। |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | एक मान प्राप्त करता या सेट करता है जो दर्शाता है कि यदि संभव हो तो टेक्स्ट एक्सट्रैक्शन के लिए रॉ मोड का उपयोग किया जाता है या नहीं। डिफ़ॉल्ट मान `false` है। रॉ मोड इंडेक्सिंग गति को काफी बढ़ा सकता है, लेकिन सामान्य मोड निकाले गए टेक्स्ट के फ़ॉर्मेटिंग को सुधारता है। |

### टिप्पणियाँ

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### संबंधित देखें

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- संपादित न करें: generated by xmldocmd GroupDocs.search.dll के लिए -->
