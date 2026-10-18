---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक कंटेनर आइटम जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

एक कंटेनर आइटम जानकारी का प्रतिनिधित्व करता है।


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | एक नया उदाहरण प्रारंभ करता है  ExtractedItemInfo  क्लास का। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | एक दस्तावेज़ प्रकार प्राप्त करता है। |
|
|  | [getFields()](#getFields--) | एक निकाले गए फ़ील्ड प्राप्त करता है। |
|
|  | [getItemInfo()](#getItemInfo--) | एक आइटम की जानकारी प्राप्त करता है। |
|
|  | [getInnerPath()](#getInnerPath--) | एक आंतरिक पथ प्राप्त करता है। |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


एक नया उदाहरण प्रारंभ करता है  ExtractedItemInfo  क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | दस्तावेज़ फ़ॉर्मेट परिवार। |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | निकाले गए फ़ील्ड। |
|
|  | itemInfo | java.lang.String | आइटम की जानकारी। |
|
|  | innerPath | java.lang.String | कंटेनर में आइटम का पथ। |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


एक दस्तावेज़ प्रकार प्राप्त करता है।


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


एक निकाले गए फ़ील्ड प्राप्त करता है।


**Returns:**
com.groupdocs.search.common.DocumentField[] - निकाले गए फ़ील्ड।

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


एक आइटम की जानकारी प्राप्त करता है।


**Returns:**
java.lang.String - आइटम की जानकारी।

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


एक आंतरिक पथ प्राप्त करता है।


**Returns:**
java.lang.String - आंतरिक पथ।

