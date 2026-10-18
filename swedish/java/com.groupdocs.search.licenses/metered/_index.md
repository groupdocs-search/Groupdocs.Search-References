---
title: "Metered"
second_title: "GroupDocs.Search för Java API-referens"
description: 
type: docs
weight: 11
url: /sv/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [Metered()](#Metered--) | Initierar en ny instans av den här klassen. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Aktiverar produkt med Metered-nycklar. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Hämtar mängden MB som har bearbetats. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Hämtar antalet förbrukade krediter. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Initierar en ny instans av den här klassen.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Aktiverar produkt med Metered-nycklar.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | publicKey | java.lang.String | offentlig nyckel |
|
|  | privateKey | java.lang.String | privat nyckel |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Hämtar mängden MB som har bearbetats.


**Returns:**
double - förbrukningsmängd

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Hämtar antalet förbrukade krediter.


**Returns:**
double - förbrukningskredit

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| längd | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| längd | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




