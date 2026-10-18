---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağında indekslenmiş bir belge için bir tanımlayıcıyı temsil eder."
type: docs
weight: 10
url: /tr/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Arama ağında indekslenmiş bir belge için bir tanımlayıcıyı temsil eder.

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Dizinlenmiş bir belge için tanımlayıcıyı alır. |
|
|  | [getShardIndex()](#getShardIndex--) | Parçacık dizinini alır. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Dizinlenmiş bir belge için tanımlayıcıyı alır.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Parçacık dizinini alır.


**Returns:**
int - Parçacık dizini.

