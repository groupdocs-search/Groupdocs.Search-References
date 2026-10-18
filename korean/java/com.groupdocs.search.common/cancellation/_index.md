---
title: "취소"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "작업 취소를 요청하기 위한 객체를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

작업 취소를 요청하기 위한 객체를 나타냅니다.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | 새 인스턴스를 초기화합니다 |
취소
클래스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | 취소가 요청되었음을 나타내는 값을 가져옵니다. |
|
|  | [cancel()](#cancel--) | 취소 요청을 합니다. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | 지정된 밀리초가 경과한 후 취소 요청을 합니다. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


새 인스턴스를 초기화합니다
취소
클래스.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


취소가 요청되었음을 나타내는 값을 가져옵니다.


**Returns:**
boolean - 취소가 요청되었음을 나타내는 값.

### cancel() {#cancel--}
```
public final void cancel()
```


취소 요청을 합니다.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


지정된 밀리초가 경과한 후 취소 요청을 합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 밀리초 | int | 작업이 취소될 때까지의 밀리초 수. |
|

