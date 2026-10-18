---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्सिंग प्रक्रिया के दौरान उपयोग किए जाने वाले अक्षर प्रतिस्थापन शब्दकोश का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

इंडेक्सिंग प्रक्रिया के दौरान उपयोग की जाने वाली कैरेक्टर रिप्लेसमेंट डिक्शनरी का इंटरफ़ेस परिभाषित करता है। कैरेक्टर रिप्लेसमेंट का उपयोग उदाहरण के लिए, उच्चारण वाले अक्षरों से एक्सेंट हटाने या केस‑इंसेंसिटिव इंडेक्स बनाने के लिए किया जा सकता है।


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | इस CharacterReplacementDictionary में शामिल अक्षरों की संख्या प्राप्त करता है। |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | निर्दिष्ट कैरेक्टर रिप्लेसमेंट संग्रह को इस CharacterReplacementDictionary के उदाहरण में जोड़ता है। |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | निर्दिष्ट कैरेक्टर रिप्लेसमेंट संग्रह को इस CharacterReplacementDictionary के उदाहरण में जोड़ता है। |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | इस  CharacterReplacementDictionary  के इस उदाहरण से निर्दिष्ट अक्षर प्रतिस्थापन संग्रह को हटाता है। |
|
|  | [contains(char character)](#contains-char-) | निर्धारित करता है कि क्या एक  CharacterReplacementDictionary  ऑब्जेक्ट में निर्दिष्ट अक्षर के लिए प्रतिस्थापन मौजूद है। |
|
|  | [getReplacement(char character)](#getReplacement-char-) | निर्दिष्ट अक्षर के लिए एक प्रतिस्थापन प्राप्त करता है। |
|
|  | [clear()](#clear--) | एक  CharacterReplacementDictionary  ऑब्जेक्ट से सभी अक्षर प्रतिस्थापन हटाता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


इस CharacterReplacementDictionary में शामिल अक्षरों की संख्या प्राप्त करता है।


**Returns:**
int - शब्दकोश में कैरेक्टर्स की संख्या।

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


निर्दिष्ट कैरेक्टर रिप्लेसमेंट संग्रह को इस CharacterReplacementDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | डिक्शनरी में जोड़ने के लिए अक्षर प्रतिस्थापन का संग्रह। |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


निर्दिष्ट कैरेक्टर रिप्लेसमेंट संग्रह को इस CharacterReplacementDictionary के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | डिक्शनरी में जोड़ने के लिए अक्षर प्रतिस्थापन का संग्रह। |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


इस  CharacterReplacementDictionary  के इस उदाहरण से निर्दिष्ट अक्षर प्रतिस्थापन संग्रह को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कैरेक्टर्स | char[] | हटाने के लिए अक्षरों का संग्रह। |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


निर्धारित करता है कि क्या एक  CharacterReplacementDictionary  ऑब्जेक्ट में निर्दिष्ट अक्षर के लिए प्रतिस्थापन मौजूद है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कैरेक्टर | char | डिक्शनरी में खोजने के लिए  CharacterReplacementDictionary  ऑब्जेक्ट का अक्षर। |
|

**Returns:**
boolean -  true  यदि  CharacterReplacementDictionary  ऑब्जेक्ट में निर्दिष्ट अक्षर मौजूद है; अन्यथा,  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


निर्दिष्ट अक्षर के लिए एक प्रतिस्थापन प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कैरेक्टर | char | जिस अक्षर के लिए प्रतिस्थापन प्राप्त करना है वह अक्षर। |
|

**Returns:**
char - निर्दिष्ट अक्षर के लिए प्रतिस्थापन।

### clear() {#clear--}
```
public abstract void clear()
```


एक  CharacterReplacementDictionary  ऑब्जेक्ट से सभी अक्षर प्रतिस्थापन हटाता है।


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.Character> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

