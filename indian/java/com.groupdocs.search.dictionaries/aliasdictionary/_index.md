---
title: "AliasDictionary"
second_title: "GroupDocs.Search for Java API Reference"
description: "उपनामों के शब्दकोश का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 14
url: /hi/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

उपनामों के शब्दकोश का इंटरफ़ेस परिभाषित करता है।


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | AliasDictionary में शामिल उपनामों की संख्या प्राप्त करता है। |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | निर्दिष्ट उपनाम/प्रतिस्थापन जोड़ों के संग्रह को इस AliasDictionary के उदाहरण में जोड़ता है। |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | निर्दिष्ट उपनाम/प्रतिस्थापन जोड़ों के संग्रह को इस AliasDictionary के उदाहरण में जोड़ता है। |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | निर्दिष्ट उपनाम और संबंधित पाठ की जोड़ी को इस AliasDictionary के उदाहरण में जोड़ता है। |
|
|  | [remove(String alias)](#remove-java.lang.String-) | एक AliasDictionary वस्तु से निर्दिष्ट उपनाम को हटाता है। |
|
|  | [contains(String alias)](#contains-java.lang.String-) | निर्धारित करता है कि एक AliasDictionary वस्तु में निर्दिष्ट उपनाम शामिल है या नहीं। |
|
|  | [getText(String alias)](#getText-java.lang.String-) | निर्दिष्ट उपनाम से जुड़ा पाठ प्राप्त करता है। |
|
|  | [clear()](#clear--) | एक AliasDictionary वस्तु से सभी उपनाम हटाता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


AliasDictionary में शामिल उपनामों की संख्या प्राप्त करता है।


**Returns:**
int - AliasDictionary में शामिल उपनामों की संख्या।

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


निर्दिष्ट उपनाम/प्रतिस्थापन जोड़ों के संग्रह को इस AliasDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | जोड़े | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | डिक्शनरी में जोड़ने के लिए उपनाम/प्रतिस्थापन जोड़ों का संग्रह। |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


निर्दिष्ट उपनाम/प्रतिस्थापन जोड़ों के संग्रह को इस AliasDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | डिक्शनरी में जोड़ने के लिए उपनाम/प्रतिस्थापन जोड़ों का संग्रह। |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


निर्दिष्ट उपनाम और संबंधित पाठ की जोड़ी को इस AliasDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | उपनाम | java.lang.String | डिक्शनरी में जोड़ने के लिए उपनाम। |
|
|  | पाठ | java.lang.String | उपनाम से जुड़ने के लिए पाठ। |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


एक AliasDictionary वस्तु से निर्दिष्ट उपनाम को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | उपनाम | java.lang.String | हटाने के लिए उपनाम। |
|

**Returns:**
boolean - यह मेथड true लौटाता है यदि उपनाम सफलतापूर्वक पाया गया और हटाया गया है। यह मेथड false लौटाता है यदि उपनाम AliasDictionary ऑब्जेक्ट में नहीं मिला।

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


निर्धारित करता है कि एक AliasDictionary वस्तु में निर्दिष्ट उपनाम शामिल है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | उपनाम | java.lang.String | AliasDictionary ऑब्जेक्ट में खोजने के लिए उपनाम। |
|

**Returns:**
boolean - true यदि AliasDictionary ऑब्जेक्ट में निर्दिष्ट उपनाम मौजूद है; अन्यथा false।

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


निर्दिष्ट उपनाम से जुड़ा पाठ प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | उपनाम | java.lang.String | AliasDictionary ऑब्जेक्ट में खोजने के लिए उपनाम। |
|

**Returns:**
java.lang.String - निर्दिष्ट उपनाम से जुड़ा पाठ या null।

### clear() {#clear--}
```
public abstract void clear()
```


एक AliasDictionary वस्तु से सभी उपनाम हटाता है।


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.String> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

