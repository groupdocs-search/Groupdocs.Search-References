---
title: "مقاس"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: 
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Metered()](#Metered--) | يُنشئ مثيلاً جديدًا من هذه الفئة. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | يفعل المنتج باستخدام مفاتيح مقاس. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | يسترجع كمية الميجابايتات المعالجة. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | يسترجع عدد الاعتمادات المستهلكة. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


يُنشئ مثيلاً جديدًا من هذه الفئة.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


يفعل المنتج باستخدام مفاتيح مقاس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | publicKey | java.lang.String | المفتاح العام |
|
|  | privateKey | java.lang.String | المفتاح الخاص |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


يسترجع كمية الميجابايتات المعالجة.


**Returns:**
double - كمية الاستهلاك

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


يسترجع عدد الاعتمادات المستهلكة.


**Returns:**
double - ائتمان الاستهلاك

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الطول | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الطول | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




