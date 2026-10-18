---
title: "DictionaryRepository"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에 있는 모든 사전의 저장소를 나타냅니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

인덱스에 있는 모든 사전의 저장소를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | 별칭 사전을 가져옵니다. |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | 불용어 사전을 가져옵니다. |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | 동의어 사전을 가져옵니다. |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | 문서 비밀번호 사전을 가져옵니다. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | 맞춤법 교정기를 가져옵니다. |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | 동음이의어 사전을 가져옵니다. |
|
|  | [getAlphabet()](#getAlphabet--) | 문자 사전을 가져옵니다. |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | 문자 대체 사전을 가져옵니다. |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | 단어 형태 제공자를 가져옵니다. |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | 단어 형태 제공자를 설정합니다. |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


별칭 사전을 가져옵니다.


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


불용어 사전을 가져옵니다.


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


동의어 사전을 가져옵니다.


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


문서 비밀번호 사전을 가져옵니다.


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


맞춤법 교정기를 가져옵니다.


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


동음이의어 사전을 가져옵니다.


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


문자 사전을 가져옵니다.


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


문자 대체 사전을 가져옵니다.


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


단어 형태 제공자를 가져옵니다.


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


단어 형태 제공자를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | 단어 형태 제공자. |
|

