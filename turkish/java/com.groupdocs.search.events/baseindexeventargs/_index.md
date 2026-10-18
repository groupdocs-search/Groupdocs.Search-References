---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Olay argümanlarının temel sınıfını temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Olay argümanlarının temel sınıfını temsil eder.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getTime()](#getTime--) | Bir olayın zamanını alır. |
|
|  | [getIndexId()](#getIndexId--) | Dizin kimliğini alır. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Dizin klasörünü alır. |
|
|  | [getStatus()](#getStatus--) | Dizin durumunu alır. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Bir olayın zamanını alır.


**Returns:**
java.util.Date - Bir olayın zamanı.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Dizin kimliğini alır.


**Returns:**
java.util.UUID - Dizin kimliği.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Dizin klasörünü alır.


**Returns:**
java.lang.String - Dizin klasörü.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Dizin durumunu alır.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

