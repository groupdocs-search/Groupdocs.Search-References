---
title: "DocumentFilter"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ फ़िल्टरों के लिए आधार वर्ग का प्रतिनिधित्व करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

डॉक्यूमेंट फ़िल्टर के बेस क्लास को दर्शाता है। इसमें डॉक्यूमेंट फ़िल्टर इंस्टेंस बनाने के लिए मेथड्स शामिल हैं।


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [toString()](#toString--) | डॉक्यूमेंट फ़िल्टर का स्ट्रिंग प्रतिनिधित्व लौटाता है। |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | निम्न सीमा से पहले की निर्माण तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | उच्च सीमा के बाद की निर्माण तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | निर्दिष्ट सीमा से बाहर की निर्माण तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | निम्न सीमा से पहले की संशोधन तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | उच्च सीमा के बाद की संशोधन तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | निर्दिष्ट सीमा से बाहर की संशोधन तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | निम्न सीमा से कम लंबाई वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | उच्च सीमा से अधिक लंबाई वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | निर्दिष्ट दस्तावेज़ लंबाई सीमा से बाहर के दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | अनुमत एक्सटेंशन न होने वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है। |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | एक फ़िल्टर बनाता है जिसका उलटा तर्क निर्दिष्ट आंतरिक फ़िल्टर के संबंध में है। |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | निर्दिष्ट फ़िल्टरों का तार्किक संयोजन बनाता है। |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | निर्दिष्ट फ़िल्टरों का तार्किक विच्छेद बनाता है। |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


डॉक्यूमेंट फ़िल्टर का स्ट्रिंग प्रतिनिधित्व लौटाता है।


**Returns:**
java.lang.String - डॉक्यूमेंट फ़िल्टर का स्ट्रिंग प्रतिनिधित्व।

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


निम्न सीमा से पहले की निर्माण तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lowerBound | java.util.Date | डॉक्यूमेंट निर्माण समय की निम्न सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


उच्च सीमा के बाद की निर्माण तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | upperBound | java.util.Date | दस्तावेज़ निर्माण समय की ऊपरी सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


निर्दिष्ट सीमा से बाहर की निर्माण तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lowerBound | java.util.Date | डॉक्यूमेंट निर्माण समय की निम्न सीमा। |
|
|  | upperBound | java.util.Date | दस्तावेज़ निर्माण समय की ऊपरी सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


निम्न सीमा से पहले की संशोधन तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lowerBound | java.util.Date | दस्तावेज़ संशोधन समय की निचली सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


उच्च सीमा के बाद की संशोधन तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | upperBound | java.util.Date | दस्तावेज़ संशोधन समय की ऊपरी सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


निर्दिष्ट सीमा से बाहर की संशोधन तिथि वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lowerBound | java.util.Date | दस्तावेज़ संशोधन समय की निचली सीमा। |
|
|  | upperBound | java.util.Date | दस्तावेज़ संशोधन समय की ऊपरी सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


एक फ़िल्टर बनाता है जो उन दस्तावेज़ों को छोड़ता है जो नियमित अभिव्यक्ति से मेल नहीं खाते। नियमित अभिव्यक्ति दस्तावेज़ के पूर्ण पथ पर लागू की जाती है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पैटर्न | java.lang.String | नियमित अभिव्यक्ति पैटर्न। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
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
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


निम्न सीमा से कम लंबाई वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lowerBound | long | दस्तावेज़ लंबाई की निचली सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


उच्च सीमा से अधिक लंबाई वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | upperBound | long | दस्तावेज़ लंबाई की ऊपरी सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


निर्दिष्ट दस्तावेज़ लंबाई सीमा से बाहर के दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | lowerBound | long | दस्तावेज़ लंबाई की निचली सीमा। |
|
|  | upperBound | long | दस्तावेज़ लंबाई की ऊपरी सीमा। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


अनुमत एक्सटेंशन न होने वाले दस्तावेज़ों को छोड़ने के लिए फ़िल्टर बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | एक्सटेंशन | java.lang.String[] | अनुमत एक्सटेंशन की सूची। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


एक फ़िल्टर बनाता है जिसका उलटा तर्क निर्दिष्ट आंतरिक फ़िल्टर के संबंध में है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | आंतरिक दस्तावेज़ फ़िल्टर। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


निर्दिष्ट फ़िल्टरों का तार्किक संयोजन बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | दस्तावेज़ फ़िल्टर। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


निर्दिष्ट फ़िल्टरों का तार्किक विच्छेद बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | दस्तावेज़ फ़िल्टर। |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

