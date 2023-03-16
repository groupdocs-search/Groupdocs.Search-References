---
title: IndexingReport
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: इंडेक्संग ऑपरेशन पर एक वस्तृत जनकर क प्रतनधत्व करत है
type: docs
weight: 240
url: /hi/net/groupdocs.search.common/indexingreport/
---
## IndexingReport class

इंडेक्सिंग ऑपरेशन पर एक विस्तृत जानकारी का प्रतिनिधित्व करता है।

```csharp
public class IndexingReport
```

## गुण

| नाम | विवरण |
| --- | --- |
| [EndTime](../../groupdocs.search.common/indexingreport/endtime) { get; } | इंडेक्सिंग समाप्ति समय प्राप्त करता है। |
| [Errors](../../groupdocs.search.common/indexingreport/errors) { get; } | त्रुटियों की सूची प्राप्त करता है। |
| [IndexedDocuments](../../groupdocs.search.common/indexingreport/indexeddocuments) { get; } | अनुक्रमित दस्तावेजों की सूची प्राप्त करता है। |
| [IndexedDocumentsSize](../../groupdocs.search.common/indexingreport/indexeddocumentssize) { get; } | एमबी में अनुक्रमित दस्तावेजों की कुल लंबाई प्राप्त करता है। |
| [IndexingTime](../../groupdocs.search.common/indexingreport/indexingtime) { get; } | इंडेक्सिंग अवधि प्राप्त करता है। |
| [RemovedDocuments](../../groupdocs.search.common/indexingreport/removeddocuments) { get; } | इंडेक्स दस्तावेज़ों से हटाए गए की सूची प्राप्त करता है। |
| [SegmentCount](../../groupdocs.search.common/indexingreport/segmentcount) { get; } | इंडेक्स सेगमेंट की संख्या प्राप्त करता है। |
| [StartTime](../../groupdocs.search.common/indexingreport/starttime) { get; } | इंडेक्सिंग प्रारंभ समय प्राप्त करता है। |
| [TotalDocumentsInIndex](../../groupdocs.search.common/indexingreport/totaldocumentsinindex) { get; } | सूचकांक में दस्तावेजों की कुल संख्या प्राप्त करता है। |
| [TotalIndexSize](../../groupdocs.search.common/indexingreport/totalindexsize) { get; } | बाइट्स में कुल सूचकांक आकार प्राप्त करता है। |
| [TotalTermCount](../../groupdocs.search.common/indexingreport/totaltermcount) { get; } | सूचकांक में शब्दों की कुल संख्या प्राप्त करता है। |
| [UpdatedDocuments](../../groupdocs.search.common/indexingreport/updateddocuments) { get; } | अद्यतन दस्तावेजों की सूची प्राप्त करता है। |

### टिप्पणियों

**और अधिक जानें**

* [अनुक्रमण रिपोर्ट](https://docs.groupdocs.com/display/searchnet/Indexing+reports)

### उदाहरण

उदाहरण वर्ग के एक विशिष्ट उपयोग को प्रदर्शित करता है।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

// निर्दिष्ट फ़ोल्डर में एक इंडेक्स बनाना
Index index = new Index(indexFolder);

// इंडेक्सिंग दस्तावेज़
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// इंडेक्सिंग रिपोर्ट प्राप्त करना
IndexingReport[] reports = index.GetIndexingReports();

// कंसोल पर रिपोर्ट प्रिंट करना
foreach (IndexingReport report in reports)
{
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.IndexingTime);
    Console.WriteLine("Documents total: " + report.TotalDocumentsInIndex);
    Console.WriteLine("Terms total: " + report.TotalTermCount);
    Console.WriteLine("Indexed documents size (MB): " + report.IndexedDocumentsSize);
    Console.WriteLine("Index size (MB): " + (report.TotalIndexSize / 1024.0 / 1024.0));
    Console.WriteLine();
}
```

### यह सभी देखें

* नाम स्थान [GroupDocs.Search.Common](../../groupdocs.search.common)
* सभा [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->