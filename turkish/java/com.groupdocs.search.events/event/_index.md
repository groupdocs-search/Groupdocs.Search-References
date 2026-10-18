---
title: "Event"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bu sınıf, olaylara abone olurken miras alınmak üzere tasarlanmıştır."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Bu sınıf, olaylara abone olurken miras alınmak üzere tasarlanmıştır.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
|  | [Event()](#Event--) | Event sınıfının yeni bir örneğini başlatır. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Olay için bir dinleyici ekler. |
|
|  | [remove(T delegate)](#remove-T-) | Olay için bir dinleyiciyi kaldırır. |
|
|  | [isEmpty()](#isEmpty--) | En az bir dinleyicinin varlığını kontrol eder. |
|
### Event() {#Event--}
```
public Event()
```


Event sınıfının yeni bir örneğini başlatır.


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Olay için bir dinleyici ekler.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | delegate | T | Olayı eklemek için bir dinleyici. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Olay için bir dinleyiciyi kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | delegate | T | Olayı kaldırmak için bir dinleyici. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


En az bir dinleyicinin varlığını kontrol eder.


**Returns:**
boolean - Olay için en az bir dinleyicinin eklendiğini gösteren bir değer.

