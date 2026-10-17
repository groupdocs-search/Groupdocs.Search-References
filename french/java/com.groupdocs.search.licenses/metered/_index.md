---
title: "Metered"
second_title: "GroupDocs.Search pour Java Référence API"
description: 
type: docs
weight: 11
url: /fr/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [Metered()](#Metered--) | Initialise une nouvelle instance de cette classe. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Active le produit avec des clés Metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Récupère la quantité de Mo traités. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Récupère le nombre de crédits consommés. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Initialise une nouvelle instance de cette classe.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Active le produit avec des clés Metered.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | publicKey | java.lang.String | clé publique |
|
|  | privateKey | java.lang.String | clé privée |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Récupère la quantité de Mo traités.


**Returns:**
double - quantité de consommation

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Récupère le nombre de crédits consommés.


**Returns:**
double - crédit de consommation

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| longueur | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| longueur | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




