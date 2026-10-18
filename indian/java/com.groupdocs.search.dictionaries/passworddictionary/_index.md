---
title: "PasswordDictionary"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ पासवर्ड की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

दस्तावेज़ पासवर्ड की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | डिक्शनरी में शामिल तत्वों की संख्या प्राप्त करता है। |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | फ़ाइल के लिए पासवर्ड प्राप्त करता है। |
|
|  | [clear()](#clear--) | इस PasswordDictionary वस्तु से सभी पासवर्ड हटाता है। |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | निर्धारित करता है कि डिक्शनरी में निर्दिष्ट दस्तावेज़ के लिए पासवर्ड है या नहीं। |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | डिक्शनरी में दस्तावेज़ के लिए पासवर्ड जोड़ता है। |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | डिक्शनरी से निर्दिष्ट दस्तावेज़ का पासवर्ड हटाता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


डिक्शनरी में शामिल तत्वों की संख्या प्राप्त करता है।


**Returns:**
int - डिक्शनरी में शामिल तत्वों की संख्या।

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


फ़ाइल के लिए पासवर्ड प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | फ़ाइल पथ। |
|

**Returns:**
java.lang.String - फ़ाइल के लिए पासवर्ड।

### clear() {#clear--}
```
public abstract void clear()
```


इस PasswordDictionary वस्तु से सभी पासवर्ड हटाता है।


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


निर्धारित करता है कि डिक्शनरी में निर्दिष्ट दस्तावेज़ के लिए पासवर्ड है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | दस्तावेज़ फ़ाइल पथ। |
|

**Returns:**
boolean - true यदि डिक्शनरी में दस्तावेज़ के लिए पासवर्ड है; अन्यथा false।

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


डिक्शनरी में दस्तावेज़ के लिए पासवर्ड जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | दस्तावेज़ फ़ाइल पथ। |
|
|  | पासवर्ड | java.lang.String | दस्तावेज़ पासवर्ड। |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


डिक्शनरी से निर्दिष्ट दस्तावेज़ का पासवर्ड हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | दस्तावेज़ फ़ाइल पथ। |
|

**Returns:**
boolean - true यदि पासवर्ड सफलतापूर्वक हटाया गया; अन्यथा false। यह विधि false भी लौटाती है यदि filePath डिक्शनरी में नहीं मिला।

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.String> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

