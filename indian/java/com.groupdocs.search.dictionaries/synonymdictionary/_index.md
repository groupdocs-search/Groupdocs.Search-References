---
title: "SynonymDictionary"
second_title: "GroupDocs.Search for Java API Reference"
description: "समानार्थक शब्दों की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 23
url: /hi/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

समानार्थक शब्दों की डिक्शनरी का इंटरफ़ेस परिभाषित करता है।


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | इस SynonymDictionary में सम्मिलित शब्दों की संख्या प्राप्त करता है। |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | निर्दिष्ट समानार्थक समूहों का संग्रह इस SynonymDictionary के इस उदाहरण में जोड़ता है। |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | निर्दिष्ट समानार्थक समूहों का संग्रह इस SynonymDictionary के इस उदाहरण में जोड़ता है। |
|
|  | [clear()](#clear--) | इस SynonymDictionary वस्तु से सभी शब्द हटाता है। |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | निर्दिष्ट शब्द के समानार्थक शब्द प्राप्त करता है। |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | निर्दिष्ट शब्द से संबंधित सभी समानार्थक समूह प्राप्त करता है। |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | इस शब्दकोश में सम्मिलित सभी समानार्थक समूह प्राप्त करता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


इस SynonymDictionary में सम्मिलित शब्दों की संख्या प्राप्त करता है।


**Returns:**
int - इस SynonymDictionary में सम्मिलित शब्दों की संख्या।

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


निर्दिष्ट समानार्थक समूहों का संग्रह इस SynonymDictionary के इस उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | समानार्थक शब्द | java.lang.Iterable<java.lang.String[]> | शब्दकोश में जोड़ने के लिए समानार्थक समूहों का संग्रह। |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


निर्दिष्ट समानार्थक समूहों का संग्रह इस SynonymDictionary के इस उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | समानार्थक शब्द | java.lang.String[][] | शब्दकोश में जोड़ने के लिए समानार्थक समूहों का संग्रह। |
|

### clear() {#clear--}
```
public abstract void clear()
```


इस SynonymDictionary वस्तु से सभी शब्द हटाता है।


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


निर्दिष्ट शब्द के समानार्थक शब्द प्राप्त करता है। परिणामी सरणी में मूल शब्द शामिल नहीं होता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String | समानार्थक शब्द सुझाने के लिए शब्द। |
|

**Returns:**
java.lang.String[] - निर्दिष्ट शब्द के समानार्थक शब्द या यदि SynonymDictionary वस्तु में वह शब्द नहीं है तो खाली सरणी।

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


निर्दिष्ट शब्द से संबंधित सभी समानार्थक समूह प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String | समानार्थक शब्दों के समूह प्राप्त करने के लिए शब्द। |
|

**Returns:**
java.lang.String[][] - सभी समानार्थक शब्द समूह जिनमें निर्दिष्ट शब्द शामिल है।

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


इस शब्दकोश में सम्मिलित सभी समानार्थक समूह प्राप्त करता है।


**Returns:**
java.lang.String[][] - सभी समानार्थक शब्द समूह।

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.String> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

