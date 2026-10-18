---
title: "Delegate"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili delegate yang merujuk pada instance kelas yang memiliki metode yang akan dipanggil."
type: docs
weight: 14
url: /id/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Mewakili delegasi, yang merujuk pada instance kelas yang memiliki metode yang akan dipanggil.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Mengembalikan daftar pemanggilan. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Menggabungkan dua delegate menjadi satu. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Menggabungkan beberapa delegate menjadi satu. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Menghapus delegate nilai dari delegate sumber. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Menghapus delegate nilai dari delegate sumber. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Memeriksa dua delegate untuk kesamaan. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Memeriksa dua delegate untuk ketidaksamaan. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Mengembalikan daftar pemanggilan.


**Returns:**
com.groupdocs.search.common.Delegate[] - Daftar pemanggilan.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


Menggabungkan dua delegate menjadi satu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Delegate pertama untuk digabungkan. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi kedua untuk digabungkan. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Menggabungkan beberapa delegate menjadi satu.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Delegasi untuk digabungkan. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Menghapus delegate nilai dari delegate sumber.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi sumber. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi nilai. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Menghapus delegate nilai dari delegate sumber.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi sumber. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi nilai. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


Memeriksa dua delegate untuk kesamaan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi pertama. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi kedua. |
|

**Returns:**
boolean - Hasil memeriksa dua delegasi untuk kesetaraan.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


Memeriksa dua delegate untuk ketidaksamaan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi pertama. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | Delegasi kedua. |
|

**Returns:**
boolean - Hasil memeriksa dua delegasi untuk ketidaksamaan.

