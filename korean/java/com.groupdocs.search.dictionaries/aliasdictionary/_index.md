---
title: "AliasDictionary"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "별칭 사전의 인터페이스를 정의합니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

별칭 사전의 인터페이스를 정의합니다.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCount()](#getCount--) | AliasDictionary에 포함된 별칭 수를 가져옵니다. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | 지정된 별칭/대체 쌍 컬렉션을 이 AliasDictionary 인스턴스에 추가합니다. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | 지정된 별칭/대체 쌍 컬렉션을 이 AliasDictionary 인스턴스에 추가합니다. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | 지정된 별칭과 연결된 텍스트 쌍을 이 AliasDictionary 인스턴스에 추가합니다. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | AliasDictionary 객체에서 지정된 별칭을 제거합니다. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | AliasDictionary 객체에 지정된 별칭이 포함되어 있는지 확인합니다. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | 지정된 별칭과 연결된 텍스트를 가져옵니다. |
|
|  | [clear()](#clear--) | AliasDictionary 객체에서 모든 별칭을 제거합니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 반복자를 반환합니다. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


AliasDictionary에 포함된 별칭 수를 가져옵니다.


**Returns:**
int - AliasDictionary에 포함된 별칭 수.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


지정된 별칭/대체 쌍 컬렉션을 이 AliasDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 쌍 | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | 사전에 추가할 별칭/대체 쌍 컬렉션. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


지정된 별칭/대체 쌍 컬렉션을 이 AliasDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | 사전에 추가할 별칭/대체 쌍 컬렉션. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


지정된 별칭과 연결된 텍스트 쌍을 이 AliasDictionary 인스턴스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 별칭 | java.lang.String | 사전에 추가할 별칭. |
|
|  | 텍스트 | java.lang.String | 별칭과 연결될 텍스트. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


AliasDictionary 객체에서 지정된 별칭을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 별칭 | java.lang.String | 제거할 별칭. |
|

**Returns:**
boolean - 이 메서드는 별칭이 성공적으로 찾아져 제거되면  true  를 반환합니다. 별칭이 AliasDictionary 객체에서 찾을 수 없으면  false  를 반환합니다.

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


AliasDictionary 객체에 지정된 별칭이 포함되어 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 별칭 | java.lang.String | AliasDictionary 객체에서 찾을 별칭. |
|

**Returns:**
boolean - AliasDictionary 객체가 지정된 별칭을 포함하면  true , 그렇지 않으면  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


지정된 별칭과 연결된 텍스트를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 별칭 | java.lang.String | AliasDictionary 객체에서 찾을 별칭. |
|

**Returns:**
java.lang.String - 지정된 별칭과 연결된 텍스트 또는  null .

### clear() {#clear--}
```
public abstract void clear()
```


AliasDictionary 객체에서 모든 별칭을 제거합니다.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<java.lang.String> - 컬렉션을 순회하는 데 사용할 수 있는 반복자.

