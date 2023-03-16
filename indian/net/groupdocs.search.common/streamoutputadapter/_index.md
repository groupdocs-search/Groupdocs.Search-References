---
title: StreamOutputAdapter
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: एक आउटपुट एडेप्टर क प्रतनधत्व करत है ज आउटपुट क a में एकत्र करत हैStream .
type: docs
weight: 300
url: /hi/net/groupdocs.search.common/streamoutputadapter/
---
## StreamOutputAdapter class

एक आउटपुट एडेप्टर का प्रतिनिधित्व करता है जो आउटपुट को a में एकत्र करता हैStream .

```csharp
public class StreamOutputAdapter : OutputAdapter
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [StreamOutputAdapter](streamoutputadapter#constructor)(OutputFormat, Stream) | का एक नया उदाहरण प्रारंभ करता है[`StreamOutputAdapter`](../streamoutputadapter) वर्ग. |

## गुण

| नाम | विवरण |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | आउटपुट स्वरूप प्राप्त करता है। |
| [Stream](../../groupdocs.search.common/streamoutputadapter/stream) { get; } | एक आउटपुट स्ट्रीम प्राप्त करता है। |

### टिप्पणियों

**और अधिक जानें**

* [आउटपुट एडेप्टर](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### उदाहरण

उदाहरण वर्ग के एक विशिष्ट उपयोग को प्रदर्शित करता है।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बनाना

index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

DocumentInfo[] documents = index.GetIndexedDocuments(); // अनुक्रमित दस्तावेजों पर जानकारी प्राप्त करना

using (Stream stream = new MemoryStream()) // एक स्ट्रीम बनाना
{
    StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // एक स्ट्रीम बनाना output adapter
    index.GetDocumentText(documents[0], adapter); // धारा में एक दस्तावेज़ पाठ उत्पन्न करना
}
```

### यह सभी देखें

* class [OutputAdapter](../outputadapter)
* नाम स्थान [GroupDocs.Search.Common](../../groupdocs.search.common)
* सभा [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->