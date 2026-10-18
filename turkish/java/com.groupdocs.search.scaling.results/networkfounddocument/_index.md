---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağında bulunan bir belgeyi temsil eder."
type: docs
weight: 11
url: /tr/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Arama ağında bulunan bir belgeyi temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Bulunan belgeyi alır. |
|
|  | [getShardIndex()](#getShardIndex--) | Parçacık dizinini alır. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Bulunan belgeyi alır.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Parçacık dizinini alır.


**Returns:**
int - Parçacık dizini.

