---
title: "वर्तनीसुधारक"
second_title: "GroupDocs.Search for Java API Reference"
description: "क्वेरी में शब्दों के लिए वर्तनी सुधारक का इंटरफ़ेस परिभाषित करता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

क्वेरी में शब्दों के लिए वर्तनी सुधारक का इंटरफ़ेस परिभाषित करता है।


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCount()](#getCount--) | इस वर्तनीसुधारक में मौजूद शब्दों की संख्या प्राप्त करता है। |
|
|  | [getWords()](#getWords--) | इस वर्तनीसुधारक में वर्तमान में मौजूद शब्दों का संग्रह प्राप्त करता है। |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | निर्दिष्ट शब्दों के संग्रह को इस SpellingCorrector के उदाहरण में जोड़ता है। |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | निर्दिष्ट शब्दों के संग्रह को इस SpellingCorrector के उदाहरण में जोड़ता है। |
|
|  | [clear()](#clear--) | एक SpellingCorrector ऑब्जेक्ट से सभी शब्द हटाता है। |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


इस वर्तनीसुधारक में मौजूद शब्दों की संख्या प्राप्त करता है।


**Returns:**
int - इस SpellingCorrector में शामिल शब्दों की संख्या।

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


इस वर्तनीसुधारक में वर्तमान में मौजूद शब्दों का संग्रह प्राप्त करता है।


**Returns:**
java.lang.String[] - शब्दों का संग्रह।

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


निर्दिष्ट शब्दों के संग्रह को इस SpellingCorrector के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.Iterable<java.lang.String> | डिक्शनरी में जोड़ने के लिए शब्दों का संग्रह। |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


निर्दिष्ट शब्दों के संग्रह को इस SpellingCorrector के उदाहरण में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String[] | डिक्शनरी में जोड़ने के लिए शब्दों का संग्रह। |
|

### clear() {#clear--}
```
public abstract void clear()
```


एक SpellingCorrector ऑब्जेक्ट से सभी शब्द हटाता है।


