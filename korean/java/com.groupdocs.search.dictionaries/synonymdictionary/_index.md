---
title: "SynonymDictionary"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "동의어 사전의 인터페이스를 정의합니다."
type: docs
weight: 23
url: /ko/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

동의어 사전의 인터페이스를 정의합니다.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | 이 SynonymDictionary에 포함된 단어 수를 가져옵니다. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | 지정된 동의어 그룹 컬렉션을 이 SynonymDictionary 인스턴스에 추가합니다. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | 지정된 동의어 그룹 컬렉션을 이 SynonymDictionary 인스턴스에 추가합니다. |
|
|  | [clear()](#clear--) | 이 SynonymDictionary 객체에서 모든 단어를 제거합니다. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | 지정된 단어에 대한 동의어를 가져옵니다. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | 지정된 단어가 속한 모든 동의어 그룹을 가져옵니다. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | 이 사전에 포함된 모든 동의어 그룹을 가져옵니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


이 SynonymDictionary에 포함된 단어 수를 가져옵니다.


**Returns:**
int - 이 SynonymDictionary에 포함된 단어 수.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


지정된 동의어 그룹 컬렉션을 이 SynonymDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | synonyms | java.lang.Iterable<java.lang.String[]> | 사전에 추가할 동의어 그룹 컬렉션. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


지정된 동의어 그룹 컬렉션을 이 SynonymDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | synonyms | java.lang.String[][] | 사전에 추가할 동의어 그룹 컬렉션. |
|

### clear() {#clear--}
```
public abstract void clear()
```


이 SynonymDictionary 객체에서 모든 단어를 제거합니다.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


지정된 단어에 대한 동의어를 가져옵니다. 결과 배열에는 원본 단어가 포함되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String | 동의어를 제안할 단어. |
|

**Returns:**
java.lang.String[] - 지정된 단어에 대한 동의어 또는 SynonymDictionary 객체에 지정된 단어가 없을 경우 빈 배열.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


지정된 단어가 속한 모든 동의어 그룹을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String | 동의어 그룹을 가져오는 단어. |
|

**Returns:**
java.lang.String[][] - 지정된 단어가 속한 모든 동의어 그룹.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


이 사전에 포함된 모든 동의어 그룹을 가져옵니다.


**Returns:**
java.lang.String[][] - 모든 동의어 그룹.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.String> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

