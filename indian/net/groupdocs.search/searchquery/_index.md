---
title: "SearchQuery"
second_title: "GroupDocs.Search .NET के लिए API Reference"
description: "ऑब्जेक्ट रूप में सर्च क्वेरी का प्रतिनिधित्व करता है।"
type: docs
weight: 1580
url: /hi/net/groupdocs.search/searchquery/
---
## SearchQuery class

ऑब्जेक्ट रूप में सर्च क्वेरी का प्रतिनिधित्व करता है।

```csharp
public abstract class SearchQuery
```

## गुण

| नाम | विवरण |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | चाइल्ड क्वेरीज़ की संख्या प्राप्त करता है। |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | फ़ील्ड का नाम प्राप्त करता है। |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | पहली चाइल्ड क्वेरी प्राप्त करता है। |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | इस seach क्वेरी के खोज विकल्प प्राप्त करता है या सेट करता है। |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | दूसरी चाइल्ड क्वेरी प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | एक संयुक्त क्वेरी बनाता है जो केवल उन दस्तावेज़ों को पाएगा जो प्रत्येक मूल क्वेरी के लिए पाए जाएंगे। |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | एक संयुक्त क्वेरी बनाता है जो केवल उन दस्तावेज़ों को पाएगा जो प्रत्येक मूल क्वेरी के लिए पाए जाएंगे। |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | एक तिथि सीमा क्वेरी बनाता है। |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | निर्दिष्ट क्वेरी में एक फ़ील्ड जोड़ता है। |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | एक उलटा क्वेरी बनाता है जो इंडेक्स में शेष दस्तावेज़ों को मूल क्वेरी के लिए पाए जाने वाले दस्तावेज़ों के विरुद्ध खोजेगा। |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | एक संख्यात्मक सीमा क्वेरी बनाता है। |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | एक संयुक्त क्वेरी बनाता है जो सभी दस्तावेज़ों को खोजेगा जो मूल क्वेरी में से कम से कम एक के लिए पाए जाएंगे। |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | एक संयुक्त क्वेरी बनाता है जो सभी दस्तावेज़ों को खोजेगा जो मूल क्वेरी में से कम से कम एक के लिए पाए जाएंगे। |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | एक वाक्यांश खोज क्वेरी बनाता है। |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | एक नियमित अभिव्यक्ति क्वेरी बनाता है। |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | एक नियमित अभिव्यक्ति क्वेरी बनाता है। |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | वाक्यांश खोज के लिए एक वाइल्डकार्ड बनाता है। |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | वाक्यांश खोज के लिए एक वाइल्डकार्ड बनाता है। |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | एक शब्द पैटर्न क्वेरी बनाता है। |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | एक सरल शब्द क्वेरी बनाता है। |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | इंडेक्स द्वारा एक चाइल्ड क्वेरी प्राप्त करता है। |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | वर्तमान [`SearchQuery`](../searchquery) इंस्टेंस का प्रतिनिधित्व करने वाली एक स्ट्रिंग लौटाता है। |

### टिप्पणियाँ

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### उदाहरण

यह उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

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

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- संपादित न करें: generated by xmldocmd GroupDocs.search.dll के लिए -->
