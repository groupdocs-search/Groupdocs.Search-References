---
title: "알파벳"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 중 문자 유형을 감지하기 위해 사용되는 문자 사전의 인터페이스를 정의합니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

인덱싱 중 문자 유형을 감지하기 위해 사용되는 문자 사전의 인터페이스를 정의합니다. 각 문자는 구분자, 문자, 혹은 둘 다로 처리될 수 있습니다.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | 문자의 유형을 가져옵니다. |
|
|  | [getCount()](#getCount--) | Alphabet에 포함된 문자 수를 가져옵니다. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | 이 Alphabet 인스턴스에서 지정된 컬렉션의 각 문자에 대한 유형을 설정합니다. |
|
|  | [clear()](#clear--) | 이 Alphabet의 모든 문자에 대해  CharacterType.Separator  유형을 설정합니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


문자의 유형을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 문자 | char | 유형을 가져올 문자. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Alphabet에 포함된 문자 수를 가져옵니다.


**Returns:**
int - 사전의 문자 수.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


이 Alphabet 인스턴스에서 지정된 컬렉션의 각 문자에 대한 유형을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 문자들 | char[] | 유형을 설정할 문자 컬렉션. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | 문자 유형. |
|

### clear() {#clear--}
```
public abstract void clear()
```


이 Alphabet의 모든 문자에 대해  CharacterType.Separator  유형을 설정합니다.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.Character> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

