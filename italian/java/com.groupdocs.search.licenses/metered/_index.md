---
title: "Metered"
second_title: "GroupDocs.Search for Java Riferimento API"
description: 
type: docs
weight: 11
url: /it/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Metered()](#Metered--) | Inizializza una nuova istanza di questa classe. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Attiva il prodotto con chiavi Metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Recupera la quantità di MB elaborati. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Recupera il conteggio dei crediti consumati. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Inizializza una nuova istanza di questa classe.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Attiva il prodotto con chiavi Metered.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | publicKey | java.lang.String | chiave pubblica |
|
|  | privateKey | java.lang.String | chiave privata |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Recupera la quantità di MB elaborati.


**Returns:**
double - quantità di consumo

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Recupera il conteggio dei crediti consumati.


**Returns:**
double - credito di consumo

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lunghezza | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| lunghezza | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




