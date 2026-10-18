---
title: "Cancellation"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir işlemin iptalini talep etmek için bir nesneyi temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Bir işlemin iptalini talep etmek için bir nesneyi temsil eder.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Yeni bir örnek başlatır |
Cancellation
sınıf.
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | İptalin istendiğini gösteren bir değer alır. |
|
|  | [cancel()](#cancel--) | İptal isteği yapar. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Belirtilen milisaniye sayısının süresi dolduktan sonra iptal isteği yapar. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Yeni bir örnek başlatır
Cancellation
sınıf.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


İptalin istendiğini gösteren bir değer alır.


**Returns:**
boolean - İptalin istendiğini gösteren bir değer.

### cancel() {#cancel--}
```
public final void cancel()
```


İptal isteği yapar.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Belirtilen milisaniye sayısının süresi dolduktan sonra iptal isteği yapar.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | milisaniye | int | Bir işlemin iptal edileceği milisaniye sayısı. |
|

