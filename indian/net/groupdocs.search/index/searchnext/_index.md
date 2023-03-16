---
title: SearchNext
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: मेथड सर्च के सथ शुरू हुई चंक सर्च क जर रखत है
type: docs
weight: 230
url: /hi/net/groupdocs.search/index/searchnext/
---
## SearchNext(ChunkSearchToken) {#searchnext}

मेथड सर्च के साथ शुरू हुई चंक सर्च को जारी रखता है।

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | चंक खोज टोकन। |

### प्रतिलाभ की मात्रा

खोज परिणाम।

### उदाहरण

उदाहरण दर्शाता है कि खंड खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

SearchOptions options = new SearchOptions();
options.IsChunkSearch = true; // चंक खोज को सक्षम करना

SearchResult result = index.Search(query, options); // चंक खोज शुरू करना
Console.WriteLine("Document count: " + result.DocumentCount);
Console.WriteLine("Occurrence count: " + result.OccurrenceCount);

while (result.NextChunkSearchToken != null)
{
    result = index.SearchNext(result.NextChunkSearchToken); // चंक खोज जारी है
    Console.WriteLine("Document count: " + result.DocumentCount);
    Console.WriteLine("Occurrence count: " + result.OccurrenceCount);
}
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## SearchNext(ChunkSearchToken, Cancellation) {#searchnext_1}

मेथड सर्च के साथ शुरू हुई चंक सर्च को जारी रखता है।

```csharp
public SearchResult SearchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| chunkSearchToken | ChunkSearchToken | चंक खोज टोकन। |
| cancellation | Cancellation | रद्दीकरण वस्तु। |

### प्रतिलाभ की मात्रा

खोज परिणाम।

### उदाहरण

उदाहरण दर्शाता है कि ऑब्जेक्ट फॉर्म में क्वेरी का उपयोग करके खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

Cancellation cancellation = new Cancellation(); // रद्दीकरण ऑब्जेक्ट रद्द होने पर सभी खोज निरंतरता को रद्द कर देता है
SearchOptions options = new SearchOptions();
options.IsChunkSearch = true; // चंक खोज को सक्षम करना
options.Cancellation = cancellation;

SearchResult result = index.Search(query, options); // चंक खोज शुरू करना
Console.WriteLine("Document count: " + result.DocumentCount);
Console.WriteLine("Occurrence count: " + result.OccurrenceCount);

while (result.NextChunkSearchToken != null)
{
    result = index.SearchNext(result.NextChunkSearchToken, cancellation); // चंक खोज जारी है
    Console.WriteLine("Document count: " + result.DocumentCount);
    Console.WriteLine("Occurrence count: " + result.OccurrenceCount);
}
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [ChunkSearchToken](../../../groupdocs.search.common/chunksearchtoken)
* class [Cancellation](../../../groupdocs.search.common/cancellation)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->