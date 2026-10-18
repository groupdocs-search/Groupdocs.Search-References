---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search for Java API Reference"
description: "कस्टम एक्सट्रैक्टर्स का एक संग्रह शामिल करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

कस्टम एक्सट्रैक्टर्स का एक संग्रह शामिल है। यदि संग्रह में किसी फ़ाइल एक्सटेंशन के लिए एक एक्सट्रैक्टर है जो बिल्ट‑इन एक्सट्रैक्टर्स द्वारा कवर किया गया है, तो यह एक्सट्रैक्टर बिल्ट‑इन वाले के बजाय उपयोग किया जाएगा।


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [size()](#size--) | संग्रह में शामिल एक्सट्रैक्टर्स की संख्या प्राप्त करता है। |
|
|  | [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो यह दर्शाता है कि संग्रह केवल-पढ़ने योग्य है या नहीं। |
|
|  | [iterator()](#iterator--) | इस संग्रह के लिए एक इटररेटर लौटाता है। |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | संग्रह में एक एक्सट्रैक्टर जोड़ता है। |
|
|  | [clear()](#clear--) | संग्रह से सभी एक्सट्रैक्टर्स को हटाता है। |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | निर्धारित करता है कि संग्रह में कोई विशिष्ट एक्सट्रैक्टर मौजूद है या नहीं। |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | संग्रह के तत्वों को एक एरे में कॉपी करता है, एक विशिष्ट एरे इंडेक्स से शुरू करके। |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | संग्रह से एक एक्सट्रैक्टर को हटाता है। |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


संग्रह में शामिल एक्सट्रैक्टर्स की संख्या प्राप्त करता है।


**Returns:**
int - संग्रह में मौजूद एक्सट्रैक्टरों की संख्या।

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि संग्रह केवल-पढ़ने योग्य है या नहीं।


**Returns:**
boolean - एक मान जो दर्शाता है कि संग्रह केवल-पढ़ने योग्य है या नहीं।

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


इस संग्रह के लिए एक इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - एक इटरेटर ऑब्जेक्ट जिसे संग्रह के माध्यम से इटरिट करने के लिए उपयोग किया जा सकता है।

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


संग्रह में एक एक्सट्रैक्टर जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | संग्रह में जोड़ने के लिए एक्सट्रैक्टर। |
|

### clear() {#clear--}
```
public abstract void clear()
```


संग्रह से सभी एक्सट्रैक्टर्स को हटाता है।


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


निर्धारित करता है कि संग्रह में कोई विशिष्ट एक्सट्रैक्टर मौजूद है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | संग्रह में खोजने के लिए एक्सट्रैक्टर। |
|

**Returns:**
boolean -  true  यदि  आइटम  संग्रह में पाया जाता है; अन्यथा,  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


संग्रह के तत्वों को एक एरे में कॉपी करता है, एक विशिष्ट एरे इंडेक्स से शुरू करके।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | एक-आयामी एरे जो संग्रह से कॉपी किए गए तत्वों का गंतव्य है। एरे में शून्य-आधारित इंडेक्सिंग होनी चाहिए। |
|
|  | arrayIndex | int | ऐरे में वह शून्य-आधारित सूचकांक जहाँ कॉपी शुरू होती है। |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


संग्रह से एक एक्सट्रैक्टर को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | संग्रह से हटाने के लिए एक्सट्रैक्टर। |
|

**Returns:**
boolean -  true  यदि  एक्सट्रैक्टर  को संग्रह से सफलतापूर्वक हटाया गया; अन्यथा,  false . यह मेथड भी  false  लौटाता है यदि  एक्सट्रैक्टर  मूल संग्रह में नहीं मिला।

