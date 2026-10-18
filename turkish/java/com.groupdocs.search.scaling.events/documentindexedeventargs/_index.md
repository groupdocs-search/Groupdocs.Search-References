---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Belge indeksleme işlemi tamamlandığında olayın argümanlarını temsil eder."
type: docs
weight: 12
url: /tr/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

Belge indeksleme işlemi tamamlandığında olayın argümanlarını temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Parçacık dizinini alır. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Belge anahtarını alır. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Parçacık dizinini alır.


**Returns:**
int - Parçacık dizini.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Belge anahtarını alır.


**Returns:**
java.lang.String - Belge anahtarı.

