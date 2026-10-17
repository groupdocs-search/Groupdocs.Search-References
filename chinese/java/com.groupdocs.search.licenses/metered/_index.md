---
title: "计量"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: 
type: docs
weight: 11
url: /zh/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [Metered()](#Metered--) | 初始化此类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | 使用计量密钥激活产品。 |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | 检索已处理的 MB 数量。 |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | 检索已消耗的积分数量。 |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


初始化此类的新实例。


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


使用计量密钥激活产品。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | publicKey | java.lang.String | 公钥 |
|
|  | privateKey | java.lang.String | 私钥 |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


检索已处理的 MB 数量。


**Returns:**
double - 消耗数量

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


检索已消耗的积分数量。


**Returns:**
double - 消耗积分

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 长度 | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 长度 | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




