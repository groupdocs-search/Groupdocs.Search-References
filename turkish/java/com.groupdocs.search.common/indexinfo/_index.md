---
title: "IndexInfo"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir Dizin hakkında temel bilgileri içerir."
type: docs
weight: 24
url: /tr/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Bir indeks hakkında temel bilgileri içerir.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Dizin benzersiz tanımlayıcısını alır. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Dizinin bulunduğu tam klasör adını alır. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Dizin durumunu alır. |
|
|  | [getVersion()](#getVersion--) | Dizin sürümünü alır. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Dizin segment sayısını alır. |
|
|  | [getTermCount()](#getTermCount--) | Dizindeki kelime sayısını alır. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Dizin benzersiz tanımlayıcısını alır.


**Returns:**
java.util.UUID - Dizinin benzersiz tanımlayıcısı.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Dizinin bulunduğu tam klasör adını alır.


**Returns:**
java.lang.String - Dizin'in bulunduğu tam klasör adı.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Dizin durumunu alır.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Dizin sürümünü alır.


**Returns:**
java.lang.String - Dizin sürümü.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Dizin segment sayısını alır.


**Returns:**
int - Dizin segment sayısı.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Dizindeki kelime sayısını alır.


**Returns:**
int - Dizindeki kelime sayısı.

