---
title: "CharacterType"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문자를 인덱싱하는 방식에 따라 문자의 유형을 나타냅니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

인덱싱 방식에 따라 문자 유형을 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Separator](#Separator) | 구분자 문자. |
|
|  | [Letter](#Letter) | 유효한 문자. |
|
|  | [Blended](#Blended) | 구분자와 유효한 문자 모두. |
|
|  | [SeparateWord](#SeparateWord) | 전체 단어를 나타내는 문자. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


구분자 문자.


### Letter {#Letter}
```
public static final CharacterType Letter
```


유효한 문자.


### Blended {#Blended}
```
public static final CharacterType Blended
```


구분자와 유효한 문자 모두.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


전체 단어를 나타내는 문자.


### values() {#values--}
```
public static CharacterType[] values()
```




**Returns:**
com.groupdocs.search.dictionaries.CharacterType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static CharacterType valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
