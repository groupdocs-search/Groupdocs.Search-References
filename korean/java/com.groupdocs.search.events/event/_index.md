---
title: "이벤트"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이 클래스는 이벤트를 구독할 때 상속하도록 설계되었습니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

이 클래스는 이벤트를 구독할 때 상속하도록 설계되었습니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Event()](#Event--) | 새로운  Event  클래스의 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [add(T delegate)](#add-T-) | 이벤트에 대한 리스너를 추가합니다. |
|
|  | [remove(T delegate)](#remove-T-) | 이벤트에 대한 리스너를 제거합니다. |
|
|  | [isEmpty()](#isEmpty--) | 하나 이상의 리스너가 존재하는지 확인합니다. |
|
### Event() {#Event--}
```
public Event()
```


새로운  Event  클래스의 인스턴스를 초기화합니다.


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


이벤트에 대한 리스너를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 대리자 | T | 추가할 이벤트 리스너. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


이벤트에 대한 리스너를 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 대리자 | T | 제거할 이벤트 리스너. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


하나 이상의 리스너가 존재하는지 확인합니다.


**Returns:**
boolean - 이벤트에 하나 이상의 리스너가 추가되었음을 나타내는 값.

