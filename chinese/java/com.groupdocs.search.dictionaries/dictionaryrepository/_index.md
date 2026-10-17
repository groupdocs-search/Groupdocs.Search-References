---
title: "DictionaryRepository"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示 Index 中所有字典的仓库。"
type: docs
weight: 12
url: /zh/java/com.groupdocs.search.dictionaries/dictionaryrepository/
---
**Inheritance:**
java.lang.Object
```
public abstract class DictionaryRepository
```

表示索引中所有字典的存储库。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DictionaryRepository()](#DictionaryRepository--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getAliasDictionary()](#getAliasDictionary--) | 获取别名字典。 |
|
|  | [getStopWordDictionary()](#getStopWordDictionary--) | 获取停用词字典。 |
|
|  | [getSynonymDictionary()](#getSynonymDictionary--) | 获取同义词字典。 |
|
|  | [getDocumentPasswords()](#getDocumentPasswords--) | 获取文档密码字典。 |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | 获取拼写校正器。 |
|
|  | [getHomophoneDictionary()](#getHomophoneDictionary--) | 获取同音字字典。 |
|
|  | [getAlphabet()](#getAlphabet--) | 获取字符字典。 |
|
|  | [getCharacterReplacements()](#getCharacterReplacements--) | 获取字符替换字典。 |
|
|  | [getWordFormsProvider()](#getWordFormsProvider--) | 获取词形提供程序。 |
|
|  | [setWordFormsProvider(IWordFormsProvider value)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | 设置词形提供程序。 |
|
### DictionaryRepository() {#DictionaryRepository--}
```
public DictionaryRepository()
```


### getAliasDictionary() {#getAliasDictionary--}
```
public abstract AliasDictionary getAliasDictionary()
```


获取别名字典。


**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary of aliases.

### getStopWordDictionary() {#getStopWordDictionary--}
```
public abstract StopWordDictionary getStopWordDictionary()
```


获取停用词字典。


**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary of stop words.

### getSynonymDictionary() {#getSynonymDictionary--}
```
public abstract SynonymDictionary getSynonymDictionary()
```


获取同义词字典。


**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary of synonyms.

### getDocumentPasswords() {#getDocumentPasswords--}
```
public abstract PasswordDictionary getDocumentPasswords()
```


获取文档密码字典。


**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary of document passwords.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public abstract SpellingCorrector getSpellingCorrector()
```


获取拼写校正器。


**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The spelling corrector.

### getHomophoneDictionary() {#getHomophoneDictionary--}
```
public abstract HomophoneDictionary getHomophoneDictionary()
```


获取同音字字典。


**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary of homophones.

### getAlphabet() {#getAlphabet--}
```
public abstract Alphabet getAlphabet()
```


获取字符字典。


**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary of characters.

### getCharacterReplacements() {#getCharacterReplacements--}
```
public abstract CharacterReplacementDictionary getCharacterReplacements()
```


获取字符替换字典。


**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary of character replacements.

### getWordFormsProvider() {#getWordFormsProvider--}
```
public abstract IWordFormsProvider getWordFormsProvider()
```


获取词形提供程序。


**Returns:**
[IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) - The word forms provider.

### setWordFormsProvider(IWordFormsProvider value) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public abstract void setWordFormsProvider(IWordFormsProvider value)
```


设置词形提供程序。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | value | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | 词形提供程序。 |
|

