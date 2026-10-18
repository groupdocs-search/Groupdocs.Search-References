---
title: "StopWordDictionary"
second_title: "GroupDocs.Search for Java API Reference"
description: "स्टॉप शब्दों की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

स्टॉप शब्दों की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | StopWordDictionary में शामिल स्टॉप शब्दों की संख्या प्राप्त करता है। |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण में जोड़ता है। |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण में जोड़ता है। |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण से हटाता है। |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण से हटाता है। |
|
|  | [contains(String word)](#contains-java.lang.String-) | निर्धारित करता है कि एक StopWordDictionary ऑब्जेक्ट में निर्दिष्ट शब्द है या नहीं। |
|
|  | [clear()](#clear--) | एक StopWordDictionary ऑब्जेक्ट से सभी शब्द हटाता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


StopWordDictionary में शामिल स्टॉप शब्दों की संख्या प्राप्त करता है।


**Returns:**
int - डिक्शनरी में स्टॉप शब्दों की संख्या।

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.Iterable<java.lang.String> | डिक्शनरी में जोड़ने के लिए शब्दों का संग्रह। |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String[] | डिक्शनरी में जोड़ने के लिए शब्दों का संग्रह। |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.Iterable<java.lang.String> | हटाने के लिए शब्दों का संग्रह। |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


निर्दिष्ट शब्दों के संग्रह को इस StopWordDictionary के उदाहरण से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String[] | हटाने के लिए शब्दों का संग्रह। |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


निर्धारित करता है कि एक StopWordDictionary ऑब्जेक्ट में निर्दिष्ट शब्द है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String | StopWordDictionary ऑब्जेक्ट में खोजने के लिए शब्द। |
|

**Returns:**
boolean - true यदि StopWordDictionary ऑब्जेक्ट में निर्दिष्ट शब्द है; अन्यथा false।

### clear() {#clear--}
```
public abstract void clear()
```


एक StopWordDictionary ऑब्जेक्ट से सभी शब्द हटाता है।


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.String> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

