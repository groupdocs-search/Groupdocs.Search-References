---
title: "Indexer"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक सेवा का प्रतिनिधित्व करता है जो खोज नेटवर्क के शार्ड्स में अनुक्रमित दस्तावेज़ों के वितरण को प्रबंधित करती है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

एक सेवा का प्रतिनिधित्व करता है जो खोज नेटवर्क के शार्ड्स में अनुक्रमित दस्तावेज़ों के वितरण को प्रबंधित करती है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | इंडेक्सिंग ऑपरेशन करता है। |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | इंडेक्स किए गए दस्तावेज़ों को हटाता है। |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | इंडेक्स सेगमेंट्स की संख्या को एक-दूसरे के साथ मर्ज करके न्यूनतम करता है। |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | इंडेक्स किए गए दस्तावेज़ों की सूची को शार्ड्स पर मौजूद दस्तावेज़ों के साथ सिंक्रोनाइज़ करता है। |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | निर्दिष्ट गुण परिवर्तन बैच को पुनः इंडेक्सिंग किए बिना इंडेक्स किए गए दस्तावेज़ों पर लागू करता है। |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | निर्दिष्ट इंडेक्स्ड दस्तावेज़ से जुड़े सभी एट्रिब्यूट्स प्राप्त करता है। |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | निर्दिष्ट शार्ड से शब्दकोश प्राप्त करता है। |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | वर्णमाला शब्दकोश प्राप्त करता है। |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | उपनाम शब्दकोश प्राप्त करता है। |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | अक्षर प्रतिस्थापन शब्दकोश प्राप्त करता है। |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | पर्याय शब्दकोश प्राप्त करता है। |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | समध्वनि शब्दकोश प्राप्त करता है। |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | वर्तनी सुधारक शब्दकोश प्राप्त करता है। |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | स्टॉप वर्ड शब्दकोश प्राप्त करता है। |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | पासवर्ड शब्दकोश प्राप्त करता है। |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | निर्दिष्ट शार्ड में एक शब्दकोश सेट करता है। |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | सभी शार्ड में एक शब्दकोश सेट करता है। |
|
|  | [deleteAllData()](#deleteAllData--) | सर्च नेटवर्क के सभी शार्ड से सभी अनुक्रमित डेटा को हटाता है। |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


अनुक्रमण ऑपरेशन करता है। केवल स्ट्रीम और संरचना से अनुक्रमण समर्थित है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | फ़ाइल सिस्टम, स्ट्रीम या संरचना से दस्तावेज़। |
|
|  | पासवर्ड | java.lang.String[] | दस्तावेज़ पासवर्ड। |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | जोड़ने के विकल्प। |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


अनुक्रमण ऑपरेशन करता है। निकाले गए डेटा को सर्च नेटवर्क में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | निकाला गया डेटा। |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | अनुक्रमण विकल्प। |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


इंडेक्स किए गए दस्तावेज़ों को हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | स्ट्रीम या संरचनाओं से जोड़े गए दस्तावेज़ों की कुंजियाँ। |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | हटाने के विकल्प। |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


इंडेक्स खंडों की संख्या को एक-दूसरे के साथ मिलाकर कम करता है। यह ऑपरेशन सर्च प्रदर्शन को सुधारता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | ऑप्टिमाइज़ विकल्प। |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


अनुक्रमित दस्तावेज़ों की सूची को शार्ड पर मौजूद दस्तावेज़ों के साथ समन्वयित करता है। यह ऑपरेशन सर्च नेटवर्क नोड्स के साथ संचार समस्याओं के कारण उत्पन्न अनुक्रमण और दस्तावेज़ हटाने की समस्याओं को ठीक करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | समन्वय विकल्प। |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


निर्दिष्ट गुण परिवर्तन बैच को पुनः इंडेक्सिंग किए बिना इंडेक्स किए गए दस्तावेज़ों पर लागू करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | गुणधर्म परिवर्तन बैच। |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | गुण बदलने के विकल्प। |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


निर्दिष्ट इंडेक्स्ड दस्तावेज़ से जुड़े सभी एट्रिब्यूट्स प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | दस्तावेज़कुंजी | java.lang.String | दस्तावेज़ कुंजी। |
|

**Returns:**
java.lang.String[] - निर्दिष्ट अनुक्रमित दस्तावेज़ से जुड़े गुण।

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


निर्दिष्ट शार्ड से शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | शब्दकोश प्रकार। |
|
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


वर्णमाला शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


उपनाम शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


अक्षर प्रतिस्थापन शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


पर्याय शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


समध्वनि शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


वर्तनी सुधारक शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


स्टॉप वर्ड शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


पासवर्ड शब्दकोश प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | shardIndex | int | शार्ड इंडेक्स। |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


निर्दिष्ट शार्ड में एक शब्दकोश सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | शब्दकोश। |
|
|  | shardIndex | int | शार्ड इंडेक्स। |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


सभी शार्ड में एक शब्दकोश सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | शब्दकोश। |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


सर्च नेटवर्क के सभी शार्ड से सभी अनुक्रमित डेटा को हटाता है।


