---
title: "Event"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Kelas ini dimaksudkan untuk diwarisi saat berlangganan peristiwa."
type: docs
weight: 11
url: /id/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Kelas ini dimaksudkan untuk diwarisi saat berlangganan peristiwa.

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [Event()](#Event--) | Menginisialisasi instance baru dari kelas Event. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Menambahkan pendengar untuk peristiwa. |
|
|  | [remove(T delegate)](#remove-T-) | Menghapus pendengar untuk peristiwa. |
|
|  | [isEmpty()](#isEmpty--) | Memeriksa keberadaan setidaknya satu pendengar. |
|
### Event() {#Event--}
```
public Event()
```


Menginisialisasi instance baru dari kelas Event.


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Menambahkan pendengar untuk peristiwa.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | delegate | T | Pendengar untuk peristiwa yang akan ditambahkan. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Menghapus pendengar untuk peristiwa.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | delegate | T | Pendengar untuk peristiwa yang akan dihapus. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Memeriksa keberadaan setidaknya satu pendengar.


**Returns:**
boolean - Nilai yang menunjukkan bahwa setidaknya satu pendengar telah ditambahkan untuk peristiwa.

