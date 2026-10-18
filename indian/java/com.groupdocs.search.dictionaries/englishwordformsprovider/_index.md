---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search for Java API Reference"
description: "अंग्रेज़ी शब्द रूप प्रदान करने वाले का प्रतिनिधित्व करता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

अंग्रेज़ी शब्द रूप प्रदान करने वाले का प्रतिनिधित्व करता है।


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | नया उदाहरण प्रारंभ करता है |
EnglishWordFormsProvider
वर्ग।
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | निर्दिष्ट शब्द के लिए शब्द रूप प्राप्त करता है। |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


नया उदाहरण प्रारंभ करता है
EnglishWordFormsProvider
वर्ग।


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


निर्दिष्ट शब्द के लिए शब्द रूप प्राप्त करता है।
परिणामी सरणी में मूल शब्द शामिल नहीं है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | शब्द | java.lang.String | शब्द रूप सुझाने के लिए शब्द। |
|

**Returns:**
java.lang.String[] - निर्दिष्ट शब्द के लिए शब्द रूप या खाली सरणी यदि IWordFormsProvider निर्दिष्ट शब्द के लिए शब्द रूप प्रदान नहीं करता है।

