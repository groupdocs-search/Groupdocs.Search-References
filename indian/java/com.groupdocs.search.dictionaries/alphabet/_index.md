---
title: "वर्णमाला"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्सिंग के दौरान अक्षर प्रकार का पता लगाने के लिए उपयोग किए जाने वाले अक्षरों के शब्दकोश का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

इंडेक्सिंग के दौरान कैरेक्टर प्रकार का पता लगाने के लिए उपयोग किए जाने वाले कैरेक्टर शब्दकोश का इंटरफ़ेस परिभाषित करता है। प्रत्येक कैरेक्टर को विभाजक, अक्षर, या दोनों के रूप में संभाला जा सकता है।


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | एक कैरेक्टर का प्रकार प्राप्त करता है। |
|
|  | [getCount()](#getCount--) | वर्णमाला में मौजूद कैरेक्टर्स की संख्या प्राप्त करता है। |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | इस वर्णमाला के इस उदाहरण में निर्दिष्ट संग्रह के प्रत्येक कैरेक्टर के प्रकार को सेट करता है। |
|
|  | [clear()](#clear--) | इस वर्णमाला में सभी कैरेक्टर्स के लिए CharacterType.Separator प्रकार सेट करता है। |
|
|  | [iterator()](#iterator--) | संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है। |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


एक कैरेक्टर का प्रकार प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कैरेक्टर | char | प्रकार प्राप्त करने के लिए कैरेक्टर। |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


वर्णमाला में मौजूद कैरेक्टर्स की संख्या प्राप्त करता है।


**Returns:**
int - शब्दकोश में कैरेक्टर्स की संख्या।

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


इस वर्णमाला के इस उदाहरण में निर्दिष्ट संग्रह के प्रत्येक कैरेक्टर के प्रकार को सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कैरेक्टर्स | char[] | प्रकार सेट करने के लिए कैरेक्टर्स का संग्रह। |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | कैरेक्टर प्रकार। |
|

### clear() {#clear--}
```
public abstract void clear()
```


इस वर्णमाला में सभी कैरेक्टर्स के लिए CharacterType.Separator प्रकार सेट करता है।


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


संग्रह के माध्यम से इटरेट करने वाला इटररेटर लौटाता है।


**Returns:**
java.util.Iterator<java.lang.Character> - एक इटरेटर जिसका उपयोग संग्रह के माध्यम से इटरेट करने के लिए किया जा सकता है।

