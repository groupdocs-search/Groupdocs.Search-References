---
title: "MulticastDelegate"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "호출될 메서드를 가진 클래스 인스턴스를 참조하는 대리자를 나타냅니다."
type: docs
weight: 26
url: /ko/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

호출될 메서드를 가진 클래스 인스턴스를 참조하는 대리자를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | 호출 목록을 반환합니다. |
|
|  | [getDelegateId()](#getDelegateId--) | 대리자 ID를 반환합니다. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | 두 대리자가 같은지 확인합니다. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | 두 대리자가 다른지 확인합니다. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


호출 목록을 반환합니다.


**Returns:**
com.groupdocs.search.common.Delegate[] - 호출 목록.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


대리자 ID를 반환합니다.


**Returns:**
java.lang.String - 대리자 ID입니다.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


두 대리자가 같은지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 첫 번째 대리자. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 두 번째 대리자. |
|

**Returns:**
boolean - 두 대리자의 동등성을 검사한 결과.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


두 대리자가 다른지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 첫 번째 대리자. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | 두 번째 대리자. |
|

**Returns:**
boolean - 두 대리자의 불일치를 검사한 결과.

