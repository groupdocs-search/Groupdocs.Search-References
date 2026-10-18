---
title: "ExtractedData"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir belgeden alınan ve indeksleme için hazırlanan verileri temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Bir belgeden alınan ve indeksleme için hazırlanan verileri temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [serialize()](#serialize--) | Geçerli örneği bir bayt dizisine serileştirir. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Bir örneği bayt dizisinden seriden çıkarır. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Geçerli örneği bir bayt dizisine serileştirir.


**Returns:**
byte[] - Geçerli örneği temsil eden bir bayt dizisi.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Bir örneği bayt dizisinden seriden çıkarır.


**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
|  | dizi | byte[] | Serileştirilecek bir bayt dizisi. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

