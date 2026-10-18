---
title: "Metered"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: 
type: docs
weight: 11
url: /es/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [Metered()](#Metered--) | Inicializa una nueva instancia de esta clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Activa el producto con claves Metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Recupera la cantidad de MB procesados. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Recupera el recuento de créditos consumidos. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Inicializa una nueva instancia de esta clase.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Activa el producto con claves Metered.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | publicKey | java.lang.String | clave pública |
|
|  | privateKey | java.lang.String | clave privada |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Recupera la cantidad de MB procesados.


**Returns:**
double - cantidad de consumo

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Recupera el recuento de créditos consumidos.


**Returns:**
double - crédito de consumo

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| longitud | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| longitud | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




