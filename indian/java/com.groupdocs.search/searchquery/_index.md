---
title: "SearchQuery"
second_title: "GroupDocs.Search for Java API Reference"
description: "ऑब्जेक्ट रूप में खोज क्वेरी का प्रतिनिधित्व करता है।"
type: docs
weight: 25
url: /hi/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

ऑब्जेक्ट रूप में खोज क्वेरी का प्रतिनिधित्व करता है।


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
 
// तिथि सीमा खोज का उप‑प्रश्न बनाना
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// 0 से 2 तक छूटे शब्दों की संख्या के साथ वाइल्डकार्ड का उप‑प्रश्न बनाना
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// सरल शब्द का उप‑प्रश्न बनाना
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // केवल उप‑प्रश्न 3 के लिए खोज विकल्प सेट करना
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// उप‑प्रश्नों को एक क्वेरी में संयोजित करना
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// पाए गए घटनाओं की बढ़ी हुई क्षमता के साथ खोज विकल्प वस्तु बनाना
SearchOptions options = new SearchOptions(); // समग्र खोज विकल्प
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // खोज करना
 
```
 
````


## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | फ़ील्ड का नाम प्राप्त करता है। |
|
|  | [getChildCount()](#getChildCount--) | संतान क्वेरीज़ की संख्या प्राप्त करता है। |
|
|  | [getFirstChild()](#getFirstChild--) | पहली संतान क्वेरी प्राप्त करता है। |
|
|  | [getSecondChild()](#getSecondChild--) | दूसरी संतान क्वेरी प्राप्त करता है। |
|
|  | [getChild(int index)](#getChild-int-) | इंडेक्स द्वारा एक संतान क्वेरी प्राप्त करता है। |
|
|  | [getSearchOptions()](#getSearchOptions--) | इस seach क्वेरी के खोज विकल्प प्राप्त करता है या सेट करता है। |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | इस seach क्वेरी के खोज विकल्प प्राप्त करता है या सेट करता है। |
|
|  | [toString()](#toString--) | वर्तमान  SearchQuery  इंस्टेंस का प्रतिनिधित्व करने वाली  System.String  लौटाता है। |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | एक सरल शब्द क्वेरी बनाता है। |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | एक शब्द पैटर्न क्वेरी बनाता है। |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | नियमित अभिव्यक्ति क्वेरी बनाता है। |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | नियमित अभिव्यक्ति क्वेरी बनाता है। |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | संख्यात्मक रेंज क्वेरी बनाता है। |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | तारीख रेंज क्वेरी बनाता है। |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | वाक्यांश खोज क्वेरी बनाता है। |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | एक संयुक्त क्वेरी बनाता है जो केवल उन दस्तावेज़ों को पाएगा जो प्रत्येक मूल क्वेरी के लिए पाए जाएंगे। |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | निर्दिष्ट क्वेरी में एक फ़ील्ड जोड़ता है। |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | एक उल्टी क्वेरी बनाता है जो इंडेक्स में शेष दस्तावेज़ों को उन दस्तावेज़ों के विरुद्ध पाएगा जो मूल क्वेरी के लिए पाए जाएंगे। |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | एक संयुक्त क्वेरी बनाता है जो केवल उन दस्तावेज़ों को पाएगा जो प्रत्येक मूल क्वेरी के लिए पाए जाएंगे। |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | एक संयुक्त क्वेरी बनाता है जो सभी दस्तावेज़ों को पाएगा जो कम से कम मूल क्वेरी में से एक के लिए पाए जाएंगे। |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | एक संयुक्त क्वेरी बनाता है जो सभी दस्तावेज़ों को पाएगा जो कम से कम मूल क्वेरी में से एक के लिए पाए जाएंगे। |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | वाक्यांश खोज के लिए वाइल्डकार्ड बनाता है। |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | वाक्यांश खोज के लिए वाइल्डकार्ड बनाता है। |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


फ़ील्ड का नाम प्राप्त करता है।


**Returns:**
java.lang.String - फ़ील्ड नाम।

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


संतान क्वेरीज़ की संख्या प्राप्त करता है।


**Returns:**
int - चाइल्ड क्वेरीज़ की संख्या।

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


पहली संतान क्वेरी प्राप्त करता है।


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


दूसरी संतान क्वेरी प्राप्त करता है।


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


इंडेक्स द्वारा एक संतान क्वेरी प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | इंडेक्स। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


इस seach क्वेरी के खोज विकल्प प्राप्त करता है या सेट करता है।


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


इस seach क्वेरी के खोज विकल्प प्राप्त करता है या सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | खोज विकल्प। |
|

### toString() {#toString--}
```
public abstract String toString()
```


वर्तमान  SearchQuery  इंस्टेंस का प्रतिनिधित्व करने वाली  System.String  लौटाता है।


**Returns:**
java.lang.String - एक  System.String  जो वर्तमान  SearchQuery  इंस्टेंस का प्रतिनिधित्व करता है।

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


एक सरल शब्द क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | टर्म | java.lang.String | खोजने के लिए टर्म। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


एक शब्द पैटर्न क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | शब्द पैटर्न। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


नियमित अभिव्यक्ति क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पैटर्न | java.lang.String | मैच करने के लिए नियमित अभिव्यक्ति पैटर्न। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


नियमित अभिव्यक्ति क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पैटर्न | java.lang.String | मैच करने के लिए नियमित अभिव्यक्ति पैटर्न। |
|
|  | विकल्प | int | नियमित अभिव्यक्ति को संशोधित करने वाले एनीमरेशन मानों का बिटवाइज़ संयोजन। इस मान में  RegexOptions.IgnoreCase  फ़्लैग होना चाहिए। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


संख्यात्मक रेंज क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शुरू | long | रेंज का शुरू मान। |
|
|  | अंत | long | रेंज का अंत मान। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


तारीख रेंज क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शुरू | java.util.Date | रेंज का शुरू मान। |
|
|  | अंत | java.util.Date | रेंज का अंत मान। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


वाक्यांश खोज क्वेरी बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | चाइल्ड क्वेरीज़। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


एक संयुक्त क्वेरी बनाता है जो केवल उन दस्तावेज़ों को पाएगा जो प्रत्येक मूल क्वेरी के लिए पाए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | जिस फ़ील्ड नाम में खोज करनी है। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


निर्दिष्ट क्वेरी में एक फ़ील्ड जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | fieldName | java.lang.String | जिस फ़ील्ड नाम में खोज करनी है। |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | फ़ील्ड जोड़ने के लिए क्वेरी। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


एक उल्टी क्वेरी बनाता है जो इंडेक्स में शेष दस्तावेज़ों को उन दस्तावेज़ों के विरुद्ध पाएगा जो मूल क्वेरी के लिए पाए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | उलटने के लिए क्वेरी। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


एक संयुक्त क्वेरी बनाता है जो केवल उन दस्तावेज़ों को पाएगा जो प्रत्येक मूल क्वेरी के लिए पाए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | बाएँ चाइल्ड क्वेरी। |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | दाएँ चाइल्ड क्वेरी। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


एक संयुक्त क्वेरी बनाता है जो सभी दस्तावेज़ों को पाएगा जो कम से कम मूल क्वेरी में से एक के लिए पाए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | बाएँ चाइल्ड क्वेरी। |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | दाएँ चाइल्ड क्वेरी। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


एक संयुक्त क्वेरी बनाता है जो सभी दस्तावेज़ों को पाएगा जो कम से कम मूल क्वेरी में से एक के लिए पाए जाएंगे।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | चाइल्ड क्वेरीज़। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


वाक्यांश खोज के लिए वाइल्डकार्ड बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | count | int | वाइल्डकार्ड में शब्दों की संख्या। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


वाक्यांश खोज के लिए वाइल्डकार्ड बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | minCount | int | वाइल्डकार्ड में शब्दों की न्यूनतम संख्या। |
|
|  | maxCount | int | वाइल्डकार्ड में शब्दों की अधिकतम संख्या। |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

