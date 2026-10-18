---
title: "खोज"
second_title: "GroupDocs.Search .NET के लिए API Reference"
description: "सूचकांक में खोज करता है।"
type: docs
weight: 260
url: /hi/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

सूचकांक में खोज करता है।

```csharp
public SearchResult Search(string query)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्वेरी | String | खोज क्वेरी। |

### रिटर्न मान

खोज परिणाम।

### उदाहरण

निम्नलिखित उदाहरण दर्शाता है कि सरल खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

निम्नलिखित उदाहरण दर्शाता है कि रेगेक्स खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

निम्नलिखित उदाहरण दर्शाता है कि फ़ैसिटेड खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### संबंधित देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

सूचकांक में खोज करता है।

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्वेरी | String | खोज क्वेरी। |
| विकल्प | SearchOptions | खोज विकल्प। |

### रिटर्न मान

खोज परिणाम।

### उदाहरण

निम्नलिखित उदाहरण दर्शाता है कि फ़ज़ी खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// शुरुआत और अंत में दोहरे उद्धरण चिह्न सूचकांक को बताते हैं कि यह वाक्यांश खोज क्वेरी है
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

निम्नलिखित उदाहरण दर्शाता है कि समानार्थक शब्द खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Enabling the synonym search

string query = "cry";
SearchResult result = index.Search(query, options); // Searching
```

### संबंधित देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

सूचकांक में खोज करता है।

```csharp
public SearchResult Search(SearchQuery query)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्वेरी | SearchQuery | खोज क्वेरी। |

### रिटर्न मान

खोज परिणाम।

### उदाहरण

निम्नलिखित उदाहरण दर्शाता है कि ऑब्जेक्ट रूप में क्वेरी का उपयोग करके खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// सबक्वेरी 1 बनाना
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// सबक्वेरी 2 बनाना
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// सबक्वेरी 3 बनाना
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// सबक्वेरीज़ को एक क्वेरी में संयोजित करना
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### संबंधित देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

सूचकांक में खोज करता है।

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| क्वेरी | SearchQuery | खोज क्वेरी। |
| विकल्प | SearchOptions | खोज विकल्प। |

### रिटर्न मान

खोज परिणाम।

### उदाहरण

निम्नलिखित उदाहरण दर्शाता है कि ऑब्जेक्ट रूप में क्वेरी का उपयोग करके खोज कैसे की जाए।

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// तिथि सीमा खोज की सबक्वेरी बनाना
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// 0 से 2 तक छूटे शब्दों की संख्या के साथ वाइल्डकार्ड की सबक्वेरी बनाना
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// सरल शब्द की सबक्वेरी बनाना
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// सबक्वेरीज़ को एक क्वेरी में संयोजित करना
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// पाए गए घटनाओं की बढ़ी हुई क्षमता के साथ खोज विकल्प ऑब्जेक्ट बनाना
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### संबंधित देखें

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

सूचकांक में रिवर्स इमेज सर्च करता है।

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| छवि | SearchImage | खोजने के लिए छवि। |
| विकल्प | ImageSearchOptions | छवि खोज विकल्प। |

### रिटर्न मान

रिवर्स इमेज सर्च का परिणाम।

### संबंधित देखें

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- संपादित न करें: generated by xmldocmd GroupDocs.search.dll के लिए -->
