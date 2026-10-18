---
title: "Indexer"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크의 샤드에 걸쳐 인덱싱된 문서의 배포를 관리하는 서비스를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.scaling/indexer/
---
**Inheritance:**
java.lang.Object
```
public abstract class Indexer
```

검색 네트워크의 샤드에 걸쳐 인덱싱된 문서의 배포를 관리하는 서비스를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Indexer()](#Indexer--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [add(Document[] documents, String[] passwords, IndexingOptions options)](#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-) | 인덱싱 작업을 수행합니다. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | 인덱싱 작업을 수행합니다. |
|
|  | [delete(String[] documentKeys, DeleteOptions options)](#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-) | 인덱싱된 문서를 삭제합니다. |
|
|  | [optimize(OptimizeOptions options)](#optimize-com.groupdocs.search.options.OptimizeOptions-) | 인덱스 세그먼트 수를 서로 병합하여 최소화합니다. |
|
|  | [synchronize(SynchronizeOptions options)](#synchronize-com.groupdocs.search.options.SynchronizeOptions-) | 인덱싱된 문서 목록을 샤드에 있는 문서와 동기화합니다. |
|
|  | [changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-) | 재인덱싱 없이 지정된 속성 변경 배치를 인덱싱된 문서에 적용합니다. |
|
|  | [getAttributes(String documentKey)](#getAttributes-java.lang.String-) | 지정된 인덱싱된 문서와 연결된 모든 속성을 가져옵니다. |
|
|  | [getDictionary(DictionaryType dictionaryType, int shardIndex)](#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-) | 지정된 샤드에서 사전을 가져옵니다. |
|
|  | [getAlphabet(int shardIndex)](#getAlphabet-int-) | 알파벳 사전을 가져옵니다. |
|
|  | [getAliasDictionary(int shardIndex)](#getAliasDictionary-int-) | 별칭 사전을 가져옵니다. |
|
|  | [getCharacterReplacementDictionary(int shardIndex)](#getCharacterReplacementDictionary-int-) | 문자 교체 사전을 가져옵니다. |
|
|  | [getSynonymDictionary(int shardIndex)](#getSynonymDictionary-int-) | 동의어 사전을 가져옵니다. |
|
|  | [getHomophoneDictionary(int shardIndex)](#getHomophoneDictionary-int-) | 동음이의어 사전을 가져옵니다. |
|
|  | [getSpellingCorrector(int shardIndex)](#getSpellingCorrector-int-) | 맞춤법 교정 사전을 가져옵니다. |
|
|  | [getStopWordDictionary(int shardIndex)](#getStopWordDictionary-int-) | 불용어 사전을 가져옵니다. |
|
|  | [getPasswordDictionary(int shardIndex)](#getPasswordDictionary-int-) | 비밀번호 사전을 가져옵니다. |
|
|  | [setDictionary(DictionaryBase dictionary, int shardIndex)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-) | 지정된 샤드에 사전을 설정합니다. |
|
|  | [setDictionary(DictionaryBase dictionary)](#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-) | 모든 샤드에 사전을 설정합니다. |
|
|  | [deleteAllData()](#deleteAllData--) | 검색 네트워크의 모든 샤드에서 색인된 모든 데이터를 삭제합니다. |
|
### Indexer() {#Indexer--}
```
public Indexer()
```


### add(Document[] documents, String[] passwords, IndexingOptions options) {#add-com.groupdocs.search.Document---java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(Document[] documents, String[] passwords, IndexingOptions options)
```


색인 작업을 수행합니다. 스트림 및 구조에서만 색인이 지원됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | 파일 시스템, 스트림 또는 구조에서 가져온 문서입니다. |
|
|  | 비밀번호 | java.lang.String[] | 문서 비밀번호입니다. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 추가 옵션입니다. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public abstract void add(ExtractedData[] data, IndexingOptions options)
```


색인 작업을 수행합니다. 추출된 데이터를 검색 네트워크에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | 추출된 데이터입니다. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 색인 옵션입니다. |
|

### delete(String[] documentKeys, DeleteOptions options) {#delete-java.lang.String---com.groupdocs.search.options.DeleteOptions-}
```
public abstract void delete(String[] documentKeys, DeleteOptions options)
```


인덱싱된 문서를 삭제합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentKeys | java.lang.String[] | 스트림 또는 구조에서 추가된 문서의 키입니다. |
|
|  | options | [DeleteOptions](../../com.groupdocs.search.options/deleteoptions) | 삭제 옵션입니다. |
|

### optimize(OptimizeOptions options) {#optimize-com.groupdocs.search.options.OptimizeOptions-}
```
public abstract void optimize(OptimizeOptions options)
```


인덱스 세그먼트를 서로 병합하여 수를 최소화합니다. 이 작업은 검색 성능을 향상시킵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | options | [OptimizeOptions](../../com.groupdocs.search.options/optimizeoptions) | 최적화 옵션입니다. |
|

### synchronize(SynchronizeOptions options) {#synchronize-com.groupdocs.search.options.SynchronizeOptions-}
```
public abstract void synchronize(SynchronizeOptions options)
```


샤드에 있는 문서와 색인된 문서 목록을 동기화합니다. 이 작업은 검색 네트워크 노드와의 통신 문제로 인해 발생한 색인 및 문서 삭제 문제를 해결합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | options | [SynchronizeOptions](../../com.groupdocs.search.options/synchronizeoptions) | 동기화 옵션입니다. |
|

### changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-com.groupdocs.search.options.ChangeAttributesOptions-}
```
public abstract void changeAttributes(AttributeChangeBatch batch, ChangeAttributesOptions options)
```


재인덱싱 없이 지정된 속성 변경 배치를 인덱싱된 문서에 적용합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | 속성 변경 배치입니다. |
|
|  | options | [ChangeAttributesOptions](../../com.groupdocs.search.options/changeattributesoptions) | 속성 변경 옵션입니다. |
|

### getAttributes(String documentKey) {#getAttributes-java.lang.String-}
```
public abstract String[] getAttributes(String documentKey)
```


지정된 인덱싱된 문서와 연결된 모든 속성을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentKey | java.lang.String | 문서 키입니다. |
|

**Returns:**
java.lang.String[] - 지정된 색인 문서와 연결된 속성입니다.

### getDictionary(DictionaryType dictionaryType, int shardIndex) {#getDictionary-com.groupdocs.search.dictionaries.DictionaryType-int-}
```
public abstract DictionaryBase getDictionary(DictionaryType dictionaryType, int shardIndex)
```


지정된 샤드에서 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | dictionaryType | [DictionaryType](../../com.groupdocs.search.dictionaries/dictionarytype) | 사전 유형입니다. |
|
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) - The dictionary.

### getAlphabet(int shardIndex) {#getAlphabet-int-}
```
public abstract Alphabet getAlphabet(int shardIndex)
```


알파벳 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[Alphabet](../../com.groupdocs.search.dictionaries/alphabet) - The dictionary.

### getAliasDictionary(int shardIndex) {#getAliasDictionary-int-}
```
public abstract AliasDictionary getAliasDictionary(int shardIndex)
```


별칭 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[AliasDictionary](../../com.groupdocs.search.dictionaries/aliasdictionary) - The dictionary.

### getCharacterReplacementDictionary(int shardIndex) {#getCharacterReplacementDictionary-int-}
```
public abstract CharacterReplacementDictionary getCharacterReplacementDictionary(int shardIndex)
```


문자 교체 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[CharacterReplacementDictionary](../../com.groupdocs.search.dictionaries/characterreplacementdictionary) - The dictionary.

### getSynonymDictionary(int shardIndex) {#getSynonymDictionary-int-}
```
public abstract SynonymDictionary getSynonymDictionary(int shardIndex)
```


동의어 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[SynonymDictionary](../../com.groupdocs.search.dictionaries/synonymdictionary) - The dictionary.

### getHomophoneDictionary(int shardIndex) {#getHomophoneDictionary-int-}
```
public abstract HomophoneDictionary getHomophoneDictionary(int shardIndex)
```


동음이의어 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[HomophoneDictionary](../../com.groupdocs.search.dictionaries/homophonedictionary) - The dictionary.

### getSpellingCorrector(int shardIndex) {#getSpellingCorrector-int-}
```
public abstract SpellingCorrector getSpellingCorrector(int shardIndex)
```


맞춤법 교정 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[SpellingCorrector](../../com.groupdocs.search.dictionaries/spellingcorrector) - The dictionary.

### getStopWordDictionary(int shardIndex) {#getStopWordDictionary-int-}
```
public abstract StopWordDictionary getStopWordDictionary(int shardIndex)
```


불용어 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[StopWordDictionary](../../com.groupdocs.search.dictionaries/stopworddictionary) - The dictionary.

### getPasswordDictionary(int shardIndex) {#getPasswordDictionary-int-}
```
public abstract PasswordDictionary getPasswordDictionary(int shardIndex)
```


비밀번호 사전을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
[PasswordDictionary](../../com.groupdocs.search.dictionaries/passworddictionary) - The dictionary.

### setDictionary(DictionaryBase dictionary, int shardIndex) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-int-}
```
public abstract void setDictionary(DictionaryBase dictionary, int shardIndex)
```


지정된 샤드에 사전을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | 사전입니다. |
|
|  | shardIndex | int | 샤드 인덱스입니다. |
|

### setDictionary(DictionaryBase dictionary) {#setDictionary-com.groupdocs.search.dictionaries.DictionaryBase-}
```
public abstract void setDictionary(DictionaryBase dictionary)
```


모든 샤드에 사전을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | dictionary | [DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase) | 사전입니다. |
|

### deleteAllData() {#deleteAllData--}
```
public abstract void deleteAllData()
```


검색 네트워크의 모든 샤드에서 색인된 모든 데이터를 삭제합니다.


