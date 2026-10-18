---
title: "SpellingCorrector"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "쿼리 내 용어에 대한 맞춤법 교정기의 인터페이스를 정의합니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

쿼리 내 용어에 대한 맞춤법 교정기의 인터페이스를 정의합니다.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | 이 SpellingCorrector에 포함된 단어 수를 가져옵니다. |
|
|  | [getWords()](#getWords--) | 현재 이 SpellingCorrector에 포함된 단어 컬렉션을 가져옵니다. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | 지정된 단어 컬렉션을 이 SpellingCorrector 인스턴스에 추가합니다. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | 지정된 단어 컬렉션을 이 SpellingCorrector 인스턴스에 추가합니다. |
|
|  | [clear()](#clear--) | SpellingCorrector 객체에서 모든 단어를 제거합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


이 SpellingCorrector에 포함된 단어 수를 가져옵니다.


**Returns:**
int - 이 SpellingCorrector에 포함된 단어 수.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


현재 이 SpellingCorrector에 포함된 단어 컬렉션을 가져옵니다.


**Returns:**
java.lang.String[] - 단어 컬렉션.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


지정된 단어 컬렉션을 이 SpellingCorrector 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.Iterable<java.lang.String> | 사전에 추가할 단어 컬렉션. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


지정된 단어 컬렉션을 이 SpellingCorrector 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String[] | 사전에 추가할 단어 컬렉션. |
|

### clear() {#clear--}
```
public abstract void clear()
```


SpellingCorrector 객체에서 모든 단어를 제거합니다.


