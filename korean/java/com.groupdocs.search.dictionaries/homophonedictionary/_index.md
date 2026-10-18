---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이형동음 동음어 사전의 인터페이스를 정의합니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

이형동음 동음어 사전의 인터페이스를 정의합니다.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | 이  HomophoneDictionary  에 포함된 단어 수를 가져옵니다. |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | 지정된 동음어 그룹 컬렉션을 이  HomophoneDictionary  인스턴스에 추가합니다. |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | 지정된 동음어 그룹 컬렉션을 이  HomophoneDictionary  인스턴스에 추가합니다. |
|
|  | [clear()](#clear--) | HomophoneDictionary 객체에서 모든 단어를 제거합니다. |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | 지정된 단어에 대한 동음어를 가져옵니다. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | 지정된 단어가 속한 모든 동음어 그룹을 가져옵니다. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | 이 사전에 포함된 모든 동음어 그룹을 가져옵니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


이  HomophoneDictionary  에 포함된 단어 수를 가져옵니다.


**Returns:**
int - 단어 수입니다.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


지정된 동음어 그룹 컬렉션을 이  HomophoneDictionary  인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | 사전에 추가할 동음어 그룹 컬렉션입니다. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


지정된 동음어 그룹 컬렉션을 이  HomophoneDictionary  인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | 사전에 추가할 동음어 그룹 컬렉션입니다. |
|

### clear() {#clear--}
```
public abstract void clear()
```


HomophoneDictionary 객체에서 모든 단어를 제거합니다.


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


지정된 단어에 대한 동음어를 가져옵니다. 결과 배열에는 원래 단어가 포함되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String | 동음이의어를 제안할 단어. |
|

**Returns:**
java.lang.String[] - 지정된 단어에 대한 동음이의어 배열, 혹은  HomophoneDictionary  객체에 지정된 단어가 없을 경우 빈 배열.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


지정된 단어가 속한 모든 동음어 그룹을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String | 동음이의어 그룹을 가져오기 위한 단어. |
|

**Returns:**
java.lang.String[][] - 지정된 단어가 속한 모든 동음이의어 그룹.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


이 사전에 포함된 모든 동음어 그룹을 가져옵니다.


**Returns:**
java.lang.String[][] - 모든 동음이의어 그룹.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.String> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

