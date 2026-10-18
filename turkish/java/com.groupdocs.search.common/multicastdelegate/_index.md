---
title: "MulticastDelegate"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Çağrılacak yönteme sahip sınıf örneklerine referans veren bir temsilciyi temsil eder."
type: docs
weight: 26
url: /tr/java/com.groupdocs.search.common/multicastdelegate/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate)
```
public abstract class MulticastDelegate extends Delegate
```

Çağrılacak bir metoda sahip sınıf örneklerine referans veren bir temsilciyi temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [MulticastDelegate()](#MulticastDelegate--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getInvocationList()](#getInvocationList--) | Bir çağrı listesini döndürür. |
|
|  | [getDelegateId()](#getDelegateId--) | Bir temsilci kimliği döndürür. |
|
|  | [op_Equality(MulticastDelegate d1, MulticastDelegate d2)](#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | İki delegenin eşitliğini kontrol eder. |
|
|  | [op_Inequality(MulticastDelegate d1, MulticastDelegate d2)](#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-) | İki delegenin eşitsizliğini kontrol eder. |
|
### MulticastDelegate() {#MulticastDelegate--}
```
public MulticastDelegate()
```


### getInvocationList() {#getInvocationList--}
```
public final Delegate[] getInvocationList()
```


Bir çağrı listesini döndürür.


**Returns:**
com.groupdocs.search.common.Delegate[] - Bir çağrı listesi.

### getDelegateId() {#getDelegateId--}
```
public String getDelegateId()
```


Bir temsilci kimliği döndürür.


**Returns:**
java.lang.String - Bir temsilci kimliği.

### op_Equality(MulticastDelegate d1, MulticastDelegate d2) {#op-Equality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Equality(MulticastDelegate d1, MulticastDelegate d2)
```


İki delegenin eşitliğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | İlk delegate. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | İkinci delegate. |
|

**Returns:**
boolean - İki delegenin eşitliğini kontrol etme sonucunu.

### op_Inequality(MulticastDelegate d1, MulticastDelegate d2) {#op-Inequality-com.groupdocs.search.common.MulticastDelegate-com.groupdocs.search.common.MulticastDelegate-}
```
public static boolean op_Inequality(MulticastDelegate d1, MulticastDelegate d2)
```


İki delegenin eşitsizliğini kontrol eder.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | d1 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | İlk delegate. |
|
|  | d2 | [MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate) | İkinci delegate. |
|

**Returns:**
boolean - İki temsilcinin eşitsizliğini kontrol etmenin sonucu.

