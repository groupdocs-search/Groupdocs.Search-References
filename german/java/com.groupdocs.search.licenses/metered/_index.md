---
title: "Metered"
second_title: "GroupDocs.Search für Java API-Referenz"
description: 
type: docs
weight: 11
url: /de/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [Metered()](#Metered--) | Initialisiert eine neue Instanz dieser Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Aktiviert das Produkt mit Metered-Schlüsseln. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Ruft die Menge der verarbeiteten MBs ab. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Ruft die Anzahl der verbrauchten Credits ab. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Initialisiert eine neue Instanz dieser Klasse.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Aktiviert das Produkt mit Metered-Schlüsseln.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | publicKey | java.lang.String | öffentlicher Schlüssel |
|
|  | privateKey | java.lang.String | privater Schlüssel |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Ruft die Menge der verarbeiteten MBs ab.


**Returns:**
double - Verbrauchsmenge

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Ruft die Anzahl der verbrauchten Credits ab.


**Returns:**
double - Verbrauchsgutschrift

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Länge | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Länge | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




