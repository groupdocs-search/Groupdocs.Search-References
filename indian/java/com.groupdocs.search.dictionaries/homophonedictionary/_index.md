---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search for Java API Reference"
description: "हेटरोग्राफिक होमोफोन की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 18
url: /hi/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

हेटरोग्राफिक होमोफोन की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | इस  HomophoneDictionary  में मौजूद शब्दों की संख्या प्राप्त करता है। |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | निर्दिष्ट होमोफोन समूहों के संग्रह को इस  HomophoneDictionary  के उदाहरण में जोड़ता है। |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | निर्दिष्ट होमोफोन समूहों के संग्रह को इस  HomophoneDictionary  के उदाहरण में जोड़ता है। |
|
|  | [clear()](#clear--) | एक  HomophoneDictionary  वस्तु से सभी शब्द हटाता है। |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | निर्दिष्ट शब्द के होमोफोन प्राप्त करता है। |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | निर्दिष्ट शब्द से संबंधित सभी होमोफोन समूह प्राप्त करता है। |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | इस शब्दकोश में मौजूद सभी होमोफोन समूह प्राप्त करता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


इस  HomophoneDictionary  में मौजूद शब्दों की संख्या प्राप्त करता है।


**Returns:**
int - शब्दों की संख्या।

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


निर्दिष्ट होमोफोन समूहों के संग्रह को इस  HomophoneDictionary  के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | शब्दकोश में जोड़ने के लिए होमोफोन समूहों का संग्रह। |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


निर्दिष्ट होमोफोन समूहों के संग्रह को इस  HomophoneDictionary  के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | शब्दकोश में जोड़ने के लिए होमोफोन समूहों का संग्रह। |
|

### clear() {#clear--}
```
public abstract void clear()
```


एक  HomophoneDictionary  वस्तु से सभी शब्द हटाता है।


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


निर्दिष्ट शब्द के होमोफोन प्राप्त करता है। परिणामी एरे में मूल शब्द शामिल नहीं होता।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String | होमोफोन सुझाने के लिए शब्द। |
|

**Returns:**
java.lang.String[] - निर्दिष्ट शब्द के होमोफोन या खाली एरे यदि HomophoneDictionary ऑब्जेक्ट में निर्दिष्ट शब्द नहीं है।

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


निर्दिष्ट शब्द से संबंधित सभी होमोफोन समूह प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String | होमोफोन समूह प्राप्त करने के लिए शब्द। |
|

**Returns:**
java.lang.String[][] - सभी होमोफोन समूह जिनमें निर्दिष्ट शब्द शामिल है।

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


इस शब्दकोश में मौजूद सभी होमोफोन समूह प्राप्त करता है।


**Returns:**
java.lang.String[][] - सभी होमोफोन समूह।

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.String> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

