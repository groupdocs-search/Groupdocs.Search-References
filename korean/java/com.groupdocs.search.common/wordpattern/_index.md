---
title: "WordPattern"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "단어 와일드카드 검색에 사용할 단어 패턴을 나타냅니다."
type: docs
weight: 34
url: /ko/java/com.groupdocs.search.common/wordpattern/
---
**Inheritance:**
java.lang.Object
```
public class WordPattern
```

단어 와일드카드 검색에 사용할 단어 패턴을 나타냅니다.


**Learn more**

* [Wildcard search](../https://docs.groupdocs.com/display/searchjava/Wildcard+search)
* [Phrase search](../https://docs.groupdocs.com/display/searchjava/Phrase+search)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [WordPattern()](#WordPattern--) | WordPattern 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [appendString(String text)](#appendString-java.lang.String-) | 단어 패턴에 문자열을 추가합니다. |
|
|  | [appendCharacter(char character)](#appendCharacter-char-) | 단어 패턴에 문자를 추가합니다. |
|
|  | [appendOneCharacterWildcard()](#appendOneCharacterWildcard--) | 단어 패턴에 한 문자 와일드카드를 추가합니다. |
|
|  | [appendZeroOrOneCharacterWildcard()](#appendZeroOrOneCharacterWildcard--) | 단어 패턴에 0개 또는 1개의 문자 와일드카드를 추가합니다. |
|
|  | [appendZeroOrMoreCharactersWildcard()](#appendZeroOrMoreCharactersWildcard--) | 단어 패턴에 0개 이상의 문자 와일드카드를 추가합니다. |
|
|  | [appendOneOrMoreCharactersWildcard()](#appendOneOrMoreCharactersWildcard--) | 단어 패턴에 1개 이상의 문자 와일드카드를 추가합니다. |
|
|  | [appendWildcard(int min, int max)](#appendWildcard-int-int-) | 단어 패턴에 와일드카드를 추가합니다. |
|
|  | [toString()](#toString--) | 현재 WordPattern을 나타내는 System.String을 반환합니다. |
|
| [getCore()](#getCore--) |  |
### WordPattern() {#WordPattern--}
```
public WordPattern()
```


WordPattern 클래스의 새 인스턴스를 초기화합니다.


### appendString(String text) {#appendString-java.lang.String-}
```
public void appendString(String text)
```


단어 패턴에 문자열을 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 텍스트 | java.lang.String | 추가할 문자열입니다. |
|

### appendCharacter(char character) {#appendCharacter-char-}
```
public void appendCharacter(char character)
```


단어 패턴에 문자를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 문자 | char | 추가할 문자입니다. |
|

### appendOneCharacterWildcard() {#appendOneCharacterWildcard--}
```
public void appendOneCharacterWildcard()
```


단어 패턴에 한 문자 와일드카드를 추가합니다.


### appendZeroOrOneCharacterWildcard() {#appendZeroOrOneCharacterWildcard--}
```
public void appendZeroOrOneCharacterWildcard()
```


단어 패턴에 0개 또는 1개의 문자 와일드카드를 추가합니다.


### appendZeroOrMoreCharactersWildcard() {#appendZeroOrMoreCharactersWildcard--}
```
public void appendZeroOrMoreCharactersWildcard()
```


단어 패턴에 0개 이상의 문자 와일드카드를 추가합니다.


### appendOneOrMoreCharactersWildcard() {#appendOneOrMoreCharactersWildcard--}
```
public void appendOneOrMoreCharactersWildcard()
```


단어 패턴에 1개 이상의 문자 와일드카드를 추가합니다.


### appendWildcard(int min, int max) {#appendWildcard-int-int-}
```
public void appendWildcard(int min, int max)
```


단어 패턴에 와일드카드를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 최소 | int | 문자의 최소 개수입니다. |
|
|  | 최대 | int | 문자의 최대 개수입니다. |
|

### toString() {#toString--}
```
public String toString()
```


현재 WordPattern을 나타내는 System.String을 반환합니다.


**Returns:**
java.lang.String - 현재 WordPattern을 나타내는 System.String입니다.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
