---
title: SearchQuery
second_title: GroupDocs.NET API संदर्भ के लिए खोजें
description: वस्तु के रूप में एक खज क्वेर क प्रतनधत्व करत है
type: docs
weight: 1240
url: /hi/net/groupdocs.search/searchquery/
---
## SearchQuery class

वस्तु के रूप में एक खोज क्वेरी का प्रतिनिधित्व करता है।

```csharp
public abstract class SearchQuery
```

## गुण

| नाम | विवरण |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | बाल प्रश्नों की संख्या प्राप्त करता है। |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | फ़ील्ड का नाम प्राप्त करता है। |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | पहली चाइल्ड क्वेरी प्राप्त करता है। |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | इस खोज क्वेरी के खोज विकल्पों को प्राप्त या सेट करता है। |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | दूसरी चाइल्ड क्वेरी प्राप्त करता है। |

## तरीकों

| नाम | विवरण |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | एक संयुक्त क्वेरी बनाता है जो केवल वही दस्तावेज़ खोजेगा जो प्रत्येक मूल क्वेरी के लिए मिलेंगे। |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | दिनांक सीमा क्वेरी बनाता है. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | निर्दिष्ट क्वेरी में एक फ़ील्ड जोड़ता है। |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | एक उलटी क्वेरी बनाता है जो मूल क्वेरी के लिए पाए जाने वाले दस्तावेज़ों के विरुद्ध एक इंडेक्स में बाकी दस्तावेज़ ढूंढेगा। |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | एक संख्यात्मक श्रेणी क्वेरी बनाता है। |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | एक संयुक्त क्वेरी बनाता है जो कम से कम एक मूल क्वेरी के लिए पाए जाने वाले सभी दस्तावेज़ों को खोजेगा। |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | एक वाक्यांश खोज क्वेरी बनाता है। |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | रेगुलर एक्सप्रेशन क्वेरी बनाता है. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | रेगुलर एक्सप्रेशन क्वेरी बनाता है. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | वाक्यांश खोज के लिए एक वाइल्डकार्ड बनाता है। |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | वाक्यांश खोज के लिए एक वाइल्डकार्ड बनाता है। |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | एक शब्द पैटर्न क्वेरी बनाता है। |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | एक साधारण शब्द क्वेरी बनाता है। |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | इंडेक्स द्वारा चाइल्ड क्वेरी प्राप्त करता है। |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | रिटर्न एString जो वर्तमान का प्रतिनिधित्व करता है[`SearchQuery`](../searchquery) उदाहरण. |

### टिप्पणियों

**और अधिक जानें**

* [खोज कर](https://docs.groupdocs.com/display/searchnet/Searching)
* [पाठ और वस्तु के रूप में प्रश्न](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [ऑब्जेक्ट फॉर्म में नेस्टिंग सर्च क्वेरीज़](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### उदाहरण

उदाहरण वर्ग के एक विशिष्ट उपयोग को प्रदर्शित करता है।

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

* नाम स्थान [GroupDocs.Search](../../groupdocs.search)
* सभा [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
