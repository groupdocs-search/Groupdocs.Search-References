---
title: "DateFormatCollection"
second_title: "GroupDocs.Search for Java API Reference"
description: "DateFormat वस्तुओं का संग्रह दर्शाता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

DateFormat वस्तुओं का संग्रह दर्शाता है।


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | संग्रह में एक डेट फ़ॉर्मेट वस्तु जोड़ता है। |
|
|  | [clear()](#clear--) | संग्रह से सभी तत्वों को हटाता है। |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | निर्धारित करता है कि क्या संग्रह में कोई विशिष्ट आइटम मौजूद है। |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | संग्रह के तत्वों को एक  Array  में कॉपी करता है, एक विशिष्ट  Array  इंडेक्स से शुरू होते हुए। |
|
|  | [size()](#size--) | संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है। |
|
|  | [isReadOnly()](#isReadOnly--) | एक मान प्राप्त करता है जो यह दर्शाता है कि संग्रह केवल-पढ़ने योग्य है या नहीं। |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | संग्रह से किसी विशिष्ट तत्व की पहली उपस्थिति को हटाता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटररेट करने वाला एक इटरेटर लौटाता है। |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


संग्रह में एक डेट फ़ॉर्मेट वस्तु जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | संग्रह में जोड़ने के लिए तिथि स्वरूप ऑब्जेक्ट। |
|

### clear() {#clear--}
```
public abstract void clear()
```


संग्रह से सभी तत्वों को हटाता है।


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


निर्धारित करता है कि क्या संग्रह में कोई विशिष्ट आइटम मौजूद है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | संग्रह में खोजने के लिए आइटम। |
|

**Returns:**
boolean -  true  यदि आइटम संग्रह में पाया जाता है; अन्यथा,  false .

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


संग्रह के तत्वों को एक  Array  में कॉपी करता है, एक विशिष्ट  Array  इंडेक्स से शुरू होते हुए।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | एक-आयामी  Array  जो संग्रह से कॉपी किए गए तत्वों का गंतव्य है। |
|
|  | arrayIndex | int | ऐरे में वह शून्य-आधारित सूचकांक जहाँ कॉपी शुरू होती है। |
|

### size() {#size--}
```
public abstract int size()
```


संग्रह में मौजूद तत्वों की संख्या प्राप्त करता है।


**Returns:**
int - संग्रह में मौजूद तत्वों की संख्या।

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


एक मान प्राप्त करता है जो यह दर्शाता है कि संग्रह केवल-पढ़ने योग्य है या नहीं।


**Returns:**
boolean -  true  यदि संग्रह केवल-पढ़ने योग्य है; अन्यथा,  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


संग्रह से किसी विशिष्ट तत्व की पहली उपस्थिति को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | संग्रह से हटाने के लिए आइटम। |
|

**Returns:**
boolean -  true  यदि आइटम को संग्रह से सफलतापूर्वक हटाया गया; अन्यथा,  false . यह मेथड भी  false  लौटाता है यदि आइटम संग्रह में नहीं मिला।

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


संग्रह के माध्यम से इटररेट करने वाला एक इटरेटर लौटाता है।


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटररेट करने के लिए किया जा सकता है।

