---
title: "WordPattern"
second_title: "GroupDocs.Search for Java API Reference"
description: "शब्द वाइल्डकार्ड खोज में उपयोग के लिए शब्द पैटर्न का प्रतिनिधित्व करता है।"
type: docs
weight: 34
url: /hi/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

शब्द वाइल्डकार्ड खोज में उपयोग के लिए शब्द पैटर्न का प्रतिनिधित्व करता है।


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | WordPattern क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | शब्द पैटर्न में एक स्ट्रिंग जोड़ता है। |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | शब्द पैटर्न में एक कैरेक्टर जोड़ता है। |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | शब्द पैटर्न में एक कैरेक्टर वाइल्डकार्ड जोड़ता है। |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | शब्द पैटर्न में शून्य या एक कैरेक्टर वाइल्डकार्ड जोड़ता है। |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | शब्द पैटर्न में शून्य या अधिक कैरेक्टर वाइल्डकार्ड जोड़ता है। |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | शब्द पैटर्न में एक या अधिक कैरेक्टर वाइल्डकार्ड जोड़ता है। |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | शब्द पैटर्न में एक वाइल्डकार्ड जोड़ता है। |
|
|  | [toString()](#toString--) | वर्तमान WordPattern का प्रतिनिधित्व करने वाला एक System.String लौटाता है। |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


WordPattern क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


शब्द पैटर्न में एक स्ट्रिंग जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पाठ | java.lang.String | जोड़ने के लिए स्ट्रिंग। |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


शब्द पैटर्न में एक कैरेक्टर जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | कैरेक्टर | char | जोड़ने के लिए अक्षर। |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


शब्द पैटर्न में एक कैरेक्टर वाइल्डकार्ड जोड़ता है।


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


शब्द पैटर्न में शून्य या एक कैरेक्टर वाइल्डकार्ड जोड़ता है।


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


शब्द पैटर्न में शून्य या अधिक कैरेक्टर वाइल्डकार्ड जोड़ता है।


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


शब्द पैटर्न में एक या अधिक कैरेक्टर वाइल्डकार्ड जोड़ता है।


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


शब्द पैटर्न में एक वाइल्डकार्ड जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | न्यूनतम | int | अक्षरों की न्यूनतम संख्या। |
|
|  | अधिकतम | int | अक्षरों की अधिकतम संख्या। |
|

### toString() {#toString--}
```
public String toString()
```


वर्तमान WordPattern का प्रतिनिधित्व करने वाला एक System.String लौटाता है।


**Returns:**
java.lang.String - एक System.String जो वर्तमान WordPattern का प्रतिनिधित्व करता है।

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
