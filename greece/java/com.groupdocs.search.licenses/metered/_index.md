---
title: "Μετρημένο"
second_title: "GroupDocs.Search για Java API Reference"
description: 
type: docs
weight: 11
url: /el/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Metered()](#Metered--) | Αρχικοποιεί ένα νέο στιγμιότυπο αυτής της κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Ενεργοποιεί το προϊόν με Μετρημένα κλειδιά. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Ανακτά το ποσό των επεξεργασμένων MB. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Ανακτά τον αριθμό των καταναλωμένων πιστώσεων. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Αρχικοποιεί ένα νέο στιγμιότυπο αυτής της κλάσης.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Ενεργοποιεί το προϊόν με Μετρημένα κλειδιά.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | publicKey | java.lang.String | δημόσιο κλειδί |
|
|  | privateKey | java.lang.String | ιδιωτικό κλειδί |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Ανακτά το ποσό των επεξεργασμένων MB.


**Returns:**
double - ποσότητα κατανάλωσης

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Ανακτά τον αριθμό των καταναλωμένων πιστώσεων.


**Returns:**
double - πίστωση κατανάλωσης

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μήκος | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μήκος | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




