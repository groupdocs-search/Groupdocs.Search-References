---
title: "Delegate"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Çağrılacak bir metoda sahip sınıf örneğine referans veren bir delegeyi temsil eder."
type: docs
weight: 14
url: /tr/java/com.groupdocs.search.common/delegate/
---
**Inheritance:**
java.lang.Object
```
public abstract class Delegate
```

Çağrılacak bir metoda sahip sınıf örneğine referans veren bir temsilciyi temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Delegate()](#Delegate--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Bir çağrı listesini döndürür. |
|
|  | [combine(Delegate a, Delegate b)](#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | İki delegeyi tek bir delegede birleştirir. |
|
|  | [combine(Delegate[] delegates)](#combine-com.groupdocs.search.common.Delegate...-) | Birçok delegeyi tek bir delegede birleştirir. |
|
|  | [remove(Delegate source, Delegate value)](#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Değer delegesini kaynak delegeden kaldırır. |
|
|  | [removeAll(Delegate source, Delegate value)](#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | Değer delegesini kaynak delegeden kaldırır. |
|
|  | [op_Equality(Delegate d1, Delegate d2)](#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | İki delegenin eşitliğini kontrol eder. |
|
|  | [op_Inequality(Delegate d1, Delegate d2)](#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-) | İki delegenin eşitsizliğini kontrol eder. |
|
### Delegate() {#Delegate--}
```
public Delegate()
```


### getInvocationList() {#getInvocationList--}
```
public Delegate[] getInvocationList()
```


Bir çağrı listesini döndürür.


**Returns:**
com.groupdocs.search.common.Delegate[] - Bir çağrı listesi.

### combine(Delegate a, Delegate b) {#combine-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate combine(Delegate a, Delegate b)
```


İki delegeyi tek bir delegede birleştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | a | [Delegate](../../com.groupdocs.search.common/delegate) | Birleştirilecek ilk delegate. |
|
|  | b | [Delegate](../../com.groupdocs.search.common/delegate) | Birleştirilecek ikinci delegate. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### combine(Delegate[] delegates) {#combine-com.groupdocs.search.common.Delegate...-}
```
public static Delegate combine(Delegate[] delegates)
```


Birçok delegeyi tek bir delegede birleştirir.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | delegates | [Delegate\[\]](../../com.groupdocs.search.common/delegate) | Birleştirilecek delegeler. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new combined delegate.

### remove(Delegate source, Delegate value) {#remove-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate remove(Delegate source, Delegate value)
```


Değer delegesini kaynak delegeden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Kaynak delegate. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Değer delegate. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### removeAll(Delegate source, Delegate value) {#removeAll-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static Delegate removeAll(Delegate source, Delegate value)
```


Değer delegesini kaynak delegeden kaldırır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | source | [Delegate](../../com.groupdocs.search.common/delegate) | Kaynak delegate. |
|
|  | value | [Delegate](../../com.groupdocs.search.common/delegate) | Değer delegate. |
|

**Returns:**
[Delegate](../../com.groupdocs.search.common/delegate) - A new delegate that is a result of removing.

### op_Equality(Delegate d1, Delegate d2) {#op-Equality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Equality(Delegate d1, Delegate d2)
```


İki delegenin eşitliğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | İlk delegate. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | İkinci delegate. |
|

**Returns:**
boolean - İki delegenin eşitliğini kontrol etme sonucunu.

### op_Inequality(Delegate d1, Delegate d2) {#op-Inequality-com.groupdocs.search.common.Delegate-com.groupdocs.search.common.Delegate-}
```
public static boolean op_Inequality(Delegate d1, Delegate d2)
```


İki delegenin eşitsizliğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | d1 | [Delegate](../../com.groupdocs.search.common/delegate) | İlk delegate. |
|
|  | d2 | [Delegate](../../com.groupdocs.search.common/delegate) | İkinci delegate. |
|

**Returns:**
boolean - İki temsilcinin eşitsizliğini kontrol etmenin sonucu.

