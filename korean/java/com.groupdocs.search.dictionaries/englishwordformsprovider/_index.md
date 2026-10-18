---
title: "EnglishWordFormsProvider"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "영어 단어 형태 제공자를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.dictionaries/englishwordformsprovider/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider)
```
public class EnglishWordFormsProvider implements IWordFormsProvider
```

영어 단어 형태 제공자를 나타냅니다.


**Learn more**

* [Search for different word forms](../https://docs.groupdocs.com/display/searchjava/Search+for+different+word+forms)
* [Word forms provider](../https://docs.groupdocs.com/display/searchjava/Word+forms+provider)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [EnglishWordFormsProvider()](#EnglishWordFormsProvider--) | 새 인스턴스를 초기화합니다 |
EnglishWordFormsProvider
클래스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getWordForms(String word)](#getWordForms-java.lang.String-) | 지정된 단어에 대한 단어 형태를 가져옵니다. |
|
### EnglishWordFormsProvider() {#EnglishWordFormsProvider--}
```
public EnglishWordFormsProvider()
```


새 인스턴스를 초기화합니다
EnglishWordFormsProvider
클래스.


### getWordForms(String word) {#getWordForms-java.lang.String-}
```
public final String[] getWordForms(String word)
```


지정된 단어에 대한 단어 형태를 가져옵니다.
결과 배열에는 원본 단어가 포함되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 단어 | java.lang.String | 단어 형태를 제안할 단어. |
|

**Returns:**
java.lang.String[] - 지정된 단어에 대한 단어 형태 또는 IWordFormsProvider가 지정된 단어에 대한 단어 형태를 제공하지 않을 경우 빈 배열.

