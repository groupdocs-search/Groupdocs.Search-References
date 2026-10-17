---
title: "DictionaryRepository"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مستودعًا لجميع القواميس في الفهرس."
type: docs
weight: 12
url: /ar/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

يمثل مستودع جميع القواميس في الفهرس.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | يحصل على قاموس للأسماء المستعارة. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | يحصل على قاموس لكلمات الوقف. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | يحصل على قاموس للمرادفات. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | يحصل على قاموس لكلمات مرور المستند. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | يحصل على مصحح إملائي. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | يحصل على قاموس للكلمات المتجانسة. |
|
|  | [getAlphabet()](#getAlphabet--) | يحصل على قاموس للأحرف. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | يحصل على قاموس لاستبدالات الأحرف. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | يحصل على مزود صيغ الكلمات. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | يضبط مزود صيغ الكلمات. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


يحصل على قاموس للأسماء المستعارة.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


يحصل على قاموس لكلمات الوقف.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


يحصل على قاموس للمرادفات.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


يحصل على قاموس لكلمات مرور المستند.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


يحصل على مصحح إملائي.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


يحصل على قاموس للكلمات المتجانسة.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


يحصل على قاموس للأحرف.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


يحصل على قاموس لاستبدالات الأحرف.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


يحصل على مزود صيغ الكلمات.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


يضبط مزود صيغ الكلمات.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | مزود صيغ الكلمات. |
|

