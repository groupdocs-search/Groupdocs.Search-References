---
title: "Metered"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: 
type: docs
weight: 11
url: /id/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Metered()](#Metered--) | Menginisialisasi instance baru dari kelas ini. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Mengaktifkan produk dengan kunci Metered. |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | Mengambil jumlah MB yang diproses. |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | Mengambil jumlah kredit yang dikonsumsi. |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


Menginisialisasi instance baru dari kelas ini.


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Mengaktifkan produk dengan kunci Metered.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | publicKey | java.lang.String | kunci publik |
|
|  | privateKey | java.lang.String | kunci pribadi |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


Mengambil jumlah MB yang diproses.


**Returns:**
double - kuantitas konsumsi

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


Mengambil jumlah kredit yang dikonsumsi.


**Returns:**
double - kredit konsumsi

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| panjang | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| panjang | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




