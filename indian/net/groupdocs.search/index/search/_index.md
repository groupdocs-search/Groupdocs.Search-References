---
title: Search
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: इंडेक्स में खजत है
type: docs
weight: 220
url: /hi/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

इंडेक्स में खोजता है।

```csharp
public SearchResult Search(string query)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| query | String | खोज क्वेरी। |

### प्रतिलाभ की मात्रा

खोज परिणाम।

### उदाहरण

निम्न उदाहरण दर्शाता है कि सरल खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

SearchResult result = index.Search(query); // खोज कर
```

निम्न उदाहरण दर्शाता है कि रेगेक्स खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

string query = "^[0-9]{3,}"; // खोज क्वेरी की शुरुआत में कैरेट प्रतीक इंडेक्स को बताता है कि यह एक रेगेक्स क्वेरी है
SearchResult result = index.Search(query); // खोज कर
```

निम्न उदाहरण प्रदर्शित करता है कि फ़ेसिटेड खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

string query = "content:Newton"; // क्वेरी में कोलन से पहले शब्द का अर्थ है खोजे जाने वाले दस्तावेज़ फ़ील्ड का नाम
SearchResult result = index.Search(query); // खोज कर
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

इंडेक्स में खोजता है।

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| query | String | खोज क्वेरी। |
| options | SearchOptions | खोज विकल्प। |

### प्रतिलाभ की मात्रा

खोज परिणाम।

### उदाहरण

निम्न उदाहरण दर्शाता है कि अस्पष्ट खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // फ़ज़ी खोज को सक्षम करना
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // प्रत्येक शब्द के लिए संभावित अंतरों की संख्या निर्धारित करना

// शुरुआत और अंत में डबल कोट्स इंडेक्स को बताते हैं कि यह वाक्यांश खोज क्वेरी है
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // खोज कर
```

निम्न उदाहरण प्रदर्शित करता है कि समानार्थी खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // समानार्थी खोज को सक्षम करना

string query = "cry";
SearchResult result = index.Search(query, options); // खोज कर
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

इंडेक्स में खोजता है।

```csharp
public SearchResult Search(SearchQuery query)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| query | SearchQuery | खोज क्वेरी। |

### प्रतिलाभ की मात्रा

खोज परिणाम।

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि ऑब्जेक्ट फॉर्म में क्वेरी का उपयोग करके खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

// सबक्वेरी बनाना 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // केवल सबक्वेरी 1 के लिए खोज विकल्प सेट करना
subquery1.SearchOptions.FuzzySearch.Enabled = true; // फ़ज़ी खोज को सक्षम करना
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // मतभेदों की अधिकतम संख्या निर्धारित करना

// सबक्वेरी बनाना 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// सबक्वेरी बनाना 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// उपश्रेणियों को एक प्रश्न में जोड़ना
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // खोज कर
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

इंडेक्स में खोजता है।

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| query | SearchQuery | खोज क्वेरी। |
| options | SearchOptions | खोज विकल्प। |

### प्रतिलाभ की मात्रा

खोज परिणाम।

### उदाहरण

निम्न उदाहरण प्रदर्शित करता है कि ऑब्जेक्ट फॉर्म में क्वेरी का उपयोग करके खोज कैसे करें।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.Add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ अनुक्रमण

// दिनांक सीमा खोज की सबक्वेरी बनाना
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0 से 2 तक छूटे हुए शब्दों की संख्या के साथ वाइल्डकार्ड की सबक्वेरी बनाना
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// सरल शब्द की सबक्वेरी बनाना
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // केवल सबक्वेरी 3 के लिए खोज विकल्प सेट करना
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// उपश्रेणियों को एक प्रश्न में जोड़ना
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// खोज विकल्प ऑब्जेक्ट बनाना, मिली हुई घटनाओं की बढ़ी हुई क्षमता के साथ
SearchOptions options = new SearchOptions(); // समग्र खोज विकल्प
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // खोज कर
```

### यह सभी देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

इंडेक्स में रिवर्स इमेज सर्च करता है।

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| image | SearchImage | खोजने के लिए छवि। |
| options | ImageSearchOptions | छवि खोज विकल्प। |

### प्रतिलाभ की मात्रा

रिवर्स इमेज सर्च का नतीजा।

### यह सभी देखें

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* नाम स्थान [GroupDocs.Search](../../index)
* सभा [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
