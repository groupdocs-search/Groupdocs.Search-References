---
title: "DictionaryRepository"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स में सभी शब्दकोशों का रिपॉजिटरी दर्शाता है।"
type: docs
weight: 12
url: /hi/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

इंडेक्स में सभी शब्दकोशों का रिपॉज़िटरी का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | उपनामों का शब्दकोश प्राप्त करता है। |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | स्टॉप शब्दों का शब्दकोश प्राप्त करता है। |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | समानार्थकों का शब्दकोश प्राप्त करता है। |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | दस्तावेज़ पासवर्डों का शब्दकोश प्राप्त करता है। |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | वर्तनी सुधारक प्राप्त करता है। |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | समध्वनि शब्दों का शब्दकोश प्राप्त करता है। |
|
|  | [getAlphabet()](#getAlphabet--) | अक्षरों का शब्दकोश प्राप्त करता है। |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | अक्षर प्रतिस्थापनों का शब्दकोश प्राप्त करता है। |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | शब्द रूप प्रदाता प्राप्त करता है। |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | शब्द रूप प्रदाता सेट करता है। |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


उपनामों का शब्दकोश प्राप्त करता है।


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


स्टॉप शब्दों का शब्दकोश प्राप्त करता है।


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


समानार्थकों का शब्दकोश प्राप्त करता है।


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


दस्तावेज़ पासवर्डों का शब्दकोश प्राप्त करता है।


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


वर्तनी सुधारक प्राप्त करता है।


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


समध्वनि शब्दों का शब्दकोश प्राप्त करता है।


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


अक्षरों का शब्दकोश प्राप्त करता है।


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


अक्षर प्रतिस्थापनों का शब्दकोश प्राप्त करता है।


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


शब्द रूप प्रदाता प्राप्त करता है।


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


शब्द रूप प्रदाता सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | एक शब्द रूप प्रदाता। |
|

