---
title: "Metered"
second_title: "GroupDocs.Search for Java API Referansı"
description: 
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Metered()](#Metered--) | Bu sınıfın yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Metered anahtarlarla ürünü etkinleştirir. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | İşlenen MB miktarını alır. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Tüketilen kredi sayısını alır. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Bu sınıfın yeni bir örneğini başlatır.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Metered anahtarlarla ürünü etkinleştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | publicKey | java.lang.String | public anahtar |
|
|  | privateKey | java.lang.String | private anahtar |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


İşlenen MB miktarını alır.


**Returns:**
double - tüketim miktarı

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Tüketilen kredi sayısını alır.


**Returns:**
double - tüketim kredisi

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uzunluk | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uzunluk | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




