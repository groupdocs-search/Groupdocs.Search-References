---
title: "Metered"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: 
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Metered()](#Metered--) | 이 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Metered 키로 제품을 활성화합니다. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 처리된 MB 양을 검색합니다. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 소모된 크레딧 수를 검색합니다. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


이 클래스의 새 인스턴스를 초기화합니다.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Metered 키로 제품을 활성화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 공개 키 |
|
|  | privateKey | java.lang.String | 비공개 키 |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


처리된 MB 양을 검색합니다.


**Returns:**
double - 소비량

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


소모된 크레딧 수를 검색합니다.


**Returns:**
double - 소비 크레딧

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 길이 | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 길이 | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




