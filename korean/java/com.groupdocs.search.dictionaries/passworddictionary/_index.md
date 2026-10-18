---
title: "PasswordDictionary"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 비밀번호 사전의 인터페이스를 정의합니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

문서 비밀번호 사전의 인터페이스를 정의합니다.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | 사전에 포함된 요소 수를 가져옵니다. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | 파일의 비밀번호를 가져옵니다. |
|
|  | [clear()](#clear--) | 이  PasswordDictionary  객체에서 모든 비밀번호를 제거합니다. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | 지정된 문서에 대한 비밀번호가 사전에 포함되어 있는지 확인합니다. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | 문서에 대한 비밀번호를 사전에 추가합니다. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | 지정된 문서의 비밀번호를 사전에서 제거합니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


사전에 포함된 요소 수를 가져옵니다.


**Returns:**
int - 사전에 포함된 요소 수.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


파일의 비밀번호를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로. |
|

**Returns:**
java.lang.String - 파일의 비밀번호.

### clear() {#clear--}
```
public abstract void clear()
```


이  PasswordDictionary  객체에서 모든 비밀번호를 제거합니다.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


지정된 문서에 대한 비밀번호가 사전에 포함되어 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 문서 파일 경로입니다. |
|

**Returns:**
boolean - 문서에 대한 비밀번호가 사전에 포함되어 있으면  true , 그렇지 않으면  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


문서에 대한 비밀번호를 사전에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 문서 파일 경로입니다. |
|
|  | 비밀번호 | java.lang.String | 문서 비밀번호. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


지정된 문서의 비밀번호를 사전에서 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 문서 파일 경로입니다. |
|

**Returns:**
boolean - 비밀번호가 성공적으로 제거되면  true , 그렇지 않으면  false . 파일 경로가 사전에 없을 경우에도  false 를 반환합니다.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.String> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

