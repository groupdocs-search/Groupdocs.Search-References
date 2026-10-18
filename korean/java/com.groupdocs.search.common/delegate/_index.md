---
title: "Delegate"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "호출될 메서드를 가진 클래스 인스턴스를 참조하는 대리자를 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

호출될 메서드를 가진 클래스 인스턴스를 참조하는 대리자를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | 호출 목록을 반환합니다. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 두 대리자를 하나로 결합합니다. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | 여러 대리자를 하나로 결합합니다. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 소스 대리자에서 값 대리자를 제거합니다. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 소스 대리자에서 값 대리자를 제거합니다. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 두 대리자가 같은지 확인합니다. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | 두 대리자가 다른지 확인합니다. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


호출 목록을 반환합니다.


**Returns:**
com.groupdocs.search.common.Delegate[] - 호출 목록.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


두 대리자를 하나로 결합합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | 결합할 첫 번째 대리자. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | 두 번째 대리자를 결합합니다. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


여러 대리자를 하나로 결합합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | 결합할 대리자들. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


소스 대리자에서 값 대리자를 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | 소스 대리자. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | 값 대리자. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


소스 대리자에서 값 대리자를 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | 소스 대리자. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | 값 대리자. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


두 대리자가 같은지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | 첫 번째 대리자. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | 두 번째 대리자. |
|

**Returns:**
boolean - 두 대리자의 동등성을 검사한 결과.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


두 대리자가 다른지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | 첫 번째 대리자. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | 두 번째 대리자. |
|

**Returns:**
boolean - 두 대리자의 불일치를 검사한 결과.

