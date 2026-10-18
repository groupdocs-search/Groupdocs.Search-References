---
title: "Metered"
second_title: "GroupDocs.Search for Java API-referentie"
description: 
type: docs
weight: 11
url: /nl/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [Metered()](#Metered--) | Initialiseert een nieuw exemplaar van deze klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Activeert product met Metered-sleutels. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Haalt de hoeveelheid verwerkte MB's op. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Haalt het aantal verbruikte credits op. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Initialiseert een nieuw exemplaar van deze klasse.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Activeert product met Metered-sleutels.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | publicKey | java.lang.String | publieke sleutel |
|
|  | privateKey | java.lang.String | privésleutel |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Haalt de hoeveelheid verwerkte MB's op.


**Returns:**
double - consumptie hoeveelheid

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Haalt het aantal verbruikte credits op.


**Returns:**
double - consumptie credit

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| lengte | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| lengte | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




