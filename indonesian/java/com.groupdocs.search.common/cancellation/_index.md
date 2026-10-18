---
title: "Pembatalan"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili objek untuk meminta pembatalan operasi."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Mewakili objek untuk meminta pembatalan operasi.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Menginisialisasi instance baru dari |
Pembatalan
kelas.
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Mengambil nilai yang menunjukkan bahwa pembatalan telah diminta. |
|
|  | [cancel()](#cancel--) | Membuat permintaan pembatalan. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Membuat permintaan pembatalan setelah berakhirnya sejumlah milidetik yang ditentukan. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Menginisialisasi instance baru dari
Pembatalan
kelas.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Mengambil nilai yang menunjukkan bahwa pembatalan telah diminta.


**Returns:**
boolean - Nilai yang menunjukkan bahwa pembatalan telah diminta.

### cancel() {#cancel--}
```
public final void cancel()
```


Membuat permintaan pembatalan.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Membuat permintaan pembatalan setelah berakhirnya sejumlah milidetik yang ditentukan.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | milidetik | int | Jumlah milidetik setelah mana operasi akan dibatalkan. |
|

