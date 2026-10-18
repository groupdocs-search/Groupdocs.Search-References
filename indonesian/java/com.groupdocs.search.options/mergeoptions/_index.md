---
title: "MergeOptions"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Menyediakan opsi untuk operasi penggabungan."
type: docs
weight: 28
url: /id/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Menyediakan opsi untuk operasi penggabungan.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Menginisialisasi sebuah instance baru dari kelas MergeOptions. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isAsync()](#isAsync--) | Mendapatkan flag pelaksanaan operasi secara asinkron. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Mengatur flag pelaksanaan operasi secara asinkron. |
|
|  | [getCancellation()](#getCancellation--) | Mendapatkan objek pembatalan operasi. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Mengatur objek pembatalan operasi. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Menginisialisasi sebuah instance baru dari kelas MergeOptions.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Mendapatkan flag pelaksanaan operasi secara asynchronous. Nilai defaultnya adalah false.


**Returns:**
boolean - Flag pelaksanaan operasi secara asynchronous.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Mengatur flag pelaksanaan operasi secara asynchronous. Nilai defaultnya adalah false.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | nilai | boolean | Flag pelaksanaan operasi secara asynchronous. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Mendapatkan objek pembatalan operasi. Nilai defaultnya adalah null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Mengatur objek pembatalan operasi. Nilai defaultnya adalah null.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Objek pembatalan operasi. |
|

