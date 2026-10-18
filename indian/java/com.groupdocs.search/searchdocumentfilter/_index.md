---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज दस्तावेज़ फ़िल्टर बनाने के लिए विधियों को शामिल करता है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

खोज दस्तावेज़ फ़िल्टर बनाने के लिए विधियों को शामिल करता है।


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो निर्दिष्ट संभावित एक्सटेंशन की सूची में नहीं हैं। |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | एक फ़िल्टर बनाता है जिसका उलटा तर्क निर्दिष्ट आंतरिक फ़िल्टर के संबंध में है। |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | निर्दिष्ट फ़िल्टरों का तार्किक संयोजन बनाता है। |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | निर्दिष्ट फ़िल्टरों का तार्किक विच्छेद बनाता है। |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जिनमें निर्दिष्ट अनुमत गुणों की सूची में से कोई मान नहीं है। |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। नियमित अभिव्यक्ति दस्तावेज़ के पूर्ण पथ पर लागू की जाती है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पैटर्न | java.lang.String | नियमित अभिव्यक्ति पैटर्न। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। नियमित अभिव्यक्ति दस्तावेज़ के पूर्ण पथ पर लागू की जाती है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पैटर्न | java.lang.String | नियमित अभिव्यक्ति पैटर्न। |
|
|  | विकल्प | int | नियमित अभिव्यक्ति विकल्प। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो निर्दिष्ट संभावित एक्सटेंशन की सूची में नहीं हैं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | एक्सटेंशन | java.lang.String[] | संभावित एक्सटेंशन की सूची। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


एक फ़िल्टर बनाता है जिसका उलटा तर्क निर्दिष्ट आंतरिक फ़िल्टर के संबंध में है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | आंतरिक सर्च दस्तावेज़ फ़िल्टर। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


निर्दिष्ट फ़िल्टरों का तार्किक संयोजन बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | सर्च दस्तावेज़ फ़िल्टर। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


निर्दिष्ट फ़िल्टरों का तार्किक विच्छेद बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | सर्च दस्तावेज़ फ़िल्टर। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जिनमें निर्दिष्ट अनुमत गुणों की सूची में से कोई मान नहीं है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | गुण | java.lang.String[] | अनुमत गुणों की सूची। |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

