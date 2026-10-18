---
title: "StopWordDictionary"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "불용어 사전의 인터페이스를 정의합니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

불용어 사전의 인터페이스를 정의합니다.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | StopWordDictionary에 포함된 불용어 수를 가져옵니다. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | 지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에 추가합니다. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | 지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에 추가합니다. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | 지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에서 제거합니다. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | 지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에서 제거합니다. |
|
|  | [contains(String word)](#contains-java.lang.String-) | StopWordDictionary 객체가 지정된 단어를 포함하는지 확인합니다. |
|
|  | [clear()](#clear--) | StopWordDictionary 객체에서 모든 단어를 제거합니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


StopWordDictionary에 포함된 불용어 수를 가져옵니다.


**Returns:**
int - 사전의 불용어 수.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.Iterable<java.lang.String> | 사전에 추가할 단어 컬렉션. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String[] | 사전에 추가할 단어 컬렉션. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에서 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.Iterable<java.lang.String> | 제거할 단어 컬렉션. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


지정된 단어 컬렉션을 이 StopWordDictionary 인스턴스에서 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String[] | 제거할 단어 컬렉션. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


StopWordDictionary 객체가 지정된 단어를 포함하는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String | StopWordDictionary 객체에서 찾을 단어. |
|

**Returns:**
boolean - StopWordDictionary 객체가 지정된 단어를 포함하면 true; 그렇지 않으면 false.

### clear() {#clear--}
```
public abstract void clear()
```


StopWordDictionary 객체에서 모든 단어를 제거합니다.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.String> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

