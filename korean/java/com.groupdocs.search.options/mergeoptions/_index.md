---
title: "MergeOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "병합 작업에 대한 옵션을 제공합니다."
type: docs
weight: 28
url: /ko/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

병합 작업에 대한 옵션을 제공합니다.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | MergeOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isAsync()](#isAsync--) | 작업을 비동기적으로 수행하는 플래그를 가져옵니다. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 작업을 비동기적으로 수행하는 플래그를 설정합니다. |
|
|  | [getCancellation()](#getCancellation--) | 작업 취소 객체를 가져옵니다. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 작업 취소 객체를 설정합니다. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


MergeOptions 클래스의 새 인스턴스를 초기화합니다.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


작업을 비동기적으로 수행하는 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 작업을 비동기적으로 수행하는 플래그.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


작업을 비동기적으로 수행하는 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 작업을 비동기적으로 수행하는 플래그. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


작업 취소 객체를 가져옵니다. 기본값은 null입니다.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


작업 취소 객체를 설정합니다. 기본값은 null입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 작업 취소 객체. |
|

