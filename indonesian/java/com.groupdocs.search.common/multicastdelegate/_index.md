---
title: "MulticastDelegate"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili delegasi yang merujuk pada instance kelas yang memiliki metode yang akan dipanggil."
type: docs
weight: 26
url: /id/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Mewakili delegasi, yang merujuk pada instance kelas yang memiliki metode yang akan dipanggil.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Mengembalikan daftar pemanggilan. |
|
|  | [getDelegateId()](#getDelegateId--) | Mengembalikan ID delegasi. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Memeriksa dua delegate untuk kesamaan. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | Memeriksa dua delegate untuk ketidaksamaan. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Mengembalikan daftar pemanggilan.


**Returns:**
com.groupdocs.search.common.Delegate[] - Daftar pemanggilan.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Mengembalikan ID delegasi.


**Returns:**
java.lang.String - ID delegasi.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


Memeriksa dua delegate untuk kesamaan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Delegasi pertama. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Delegasi kedua. |
|

**Returns:**
boolean - Hasil memeriksa dua delegasi untuk kesetaraan.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


Memeriksa dua delegate untuk ketidaksamaan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Delegasi pertama. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | Delegasi kedua. |
|

**Returns:**
boolean - Hasil memeriksa dua delegasi untuk ketidaksamaan.

