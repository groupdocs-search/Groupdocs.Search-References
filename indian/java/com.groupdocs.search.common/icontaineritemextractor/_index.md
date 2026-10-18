---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search for Java API Reference"
description: "कंटेनर दस्तावेज़ों से आइटम निकालने के लिए मेथड प्रदान करता है।"
type: docs
weight: 35
url: /hi/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

कंटेनर दस्तावेज़ों से आइटम निकालने के लिए मेथड प्रदान करता है।


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | दस्तावेज़ फ़ॉर्मेट परिवार प्राप्त करता है। |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | कंटेनर दस्तावेज़ से आइटम निकालता है। |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | कंटेनर दस्तावेज़ से आइटम निकालता है। |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


दस्तावेज़ फ़ॉर्मेट परिवार प्राप्त करता है।


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


कंटेनर दस्तावेज़ से आइटम निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | फ़ाइल पथ। |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - निकाले गए आइटमों की एक सरणी।

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


कंटेनर दस्तावेज़ से आइटम निकालता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्ट्रीम | java.io.InputStream | दस्तावेज़ स्ट्रीम। |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - निकाले गए आइटमों की एक सरणी।

