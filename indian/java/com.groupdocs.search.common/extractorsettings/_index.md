---
title: "ExtractorSettings"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ डेटा एक्सट्रैक्टर के लिए सेटिंग्स शामिल करता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

दस्तावेज़ डेटा एक्सट्रैक्टर के लिए सेटिंग्स शामिल करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | एक्सट्रैक्टर के उपयोग किए जाने वाले इंडेक्स प्रकार को प्राप्त करता है। |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | एक्सट्रैक्टर के उपयोग किए जाने वाले इंडेक्स प्रकार को सेट करता है। |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


एक्सट्रैक्टर के उपयोग किए जाने वाले इंडेक्स प्रकार को प्राप्त करता है। डिफ़ॉल्ट मान है  GroupDocs.Search.Options.IndexType.NormalIndex .


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


एक्सट्रैक्टर के उपयोग किए जाने वाले इंडेक्स प्रकार को सेट करता है। डिफ़ॉल्ट मान है  GroupDocs.Search.Options.IndexType.NormalIndex .


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | इंडेक्स प्रकार जिसके लिए एक्सट्रैक्टर उपयोग किया जाता है। |
|

