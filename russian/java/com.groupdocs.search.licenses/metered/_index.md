---
title: "Metered"
second_title: "GroupDocs.Search для Java API Reference"
description: 
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Metered()](#Metered--) | Инициализирует новый экземпляр этого класса. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Активирует продукт с Metered-ключами. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Получает количество обработанных мегабайт. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Получает количество использованных кредитов. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Инициализирует новый экземпляр этого класса.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Активирует продукт с Metered-ключами.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | publicKey | java.lang.String | публичный ключ |
|
|  | privateKey | java.lang.String | закрытый ключ |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Получает количество обработанных мегабайт.


**Returns:**
double - количество потребления

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Получает количество использованных кредитов.


**Returns:**
double - потребляемый кредит

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| длина | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| длина | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




