---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 과정에서 사용되는 문자 대체 사전의 인터페이스를 정의합니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

인덱싱 과정에서 사용되는 문자 교체 사전의 인터페이스를 정의합니다. 예를 들어, 문자 교체는 억양이 있는 문자에서 악센트를 제거하거나 대소문자를 구분하지 않는 인덱스를 만들 때 사용할 수 있습니다.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | 이  CharacterReplacementDictionary  에 포함된 문자 수를 가져옵니다. |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | 지정된 문자 교체 컬렉션을 이  CharacterReplacementDictionary  인스턴스에 추가합니다. |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | 지정된 문자 교체 컬렉션을 이  CharacterReplacementDictionary  인스턴스에 추가합니다. |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | 이 CharacterReplacementDictionary 인스턴스에서 지정된 문자 교체 컬렉션을 제거합니다. |
|
|  | [contains(char character)](#contains-char-) | 지정된 문자에 대한 교체가 CharacterReplacementDictionary 객체에 포함되어 있는지 확인합니다. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | 지정된 문자에 대한 교체를 가져옵니다. |
|
|  | [clear()](#clear--) | CharacterReplacementDictionary 객체에서 모든 문자 교체를 제거합니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


이  CharacterReplacementDictionary  에 포함된 문자 수를 가져옵니다.


**Returns:**
int - 사전의 문자 수.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


지정된 문자 교체 컬렉션을 이  CharacterReplacementDictionary  인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | 사전에 추가할 문자 교체 컬렉션입니다. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


지정된 문자 교체 컬렉션을 이  CharacterReplacementDictionary  인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | 사전에 추가할 문자 교체 컬렉션입니다. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


이 CharacterReplacementDictionary 인스턴스에서 지정된 문자 교체 컬렉션을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 문자들 | char[] | 제거할 문자 컬렉션입니다. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


지정된 문자에 대한 교체가 CharacterReplacementDictionary 객체에 포함되어 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 문자 | char | CharacterReplacementDictionary 객체에서 찾을 문자입니다. |
|

**Returns:**
boolean - 지정된 문자를 CharacterReplacementDictionary 객체가 포함하고 있으면 true, 그렇지 않으면 false.

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


지정된 문자에 대한 교체를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 문자 | char | 교체를 가져올 문자입니다. |
|

**Returns:**
char - 지정된 문자에 대한 교체입니다.

### clear() {#clear--}
```
public abstract void clear()
```


CharacterReplacementDictionary 객체에서 모든 문자 교체를 제거합니다.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.Character> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

