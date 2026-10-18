---
title: "ExtractedData"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar data som hämtas från ett dokument och förbereds för indexering."
type: docs
weight: 15
url: /sv/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Representerar data som hämtas från ett dokument och förbereds för indexering.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [serialize()](#serialize--) | Serialiserar den aktuella instansen till en bytearray. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiserar en instans från en bytearray. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serialiserar den aktuella instansen till en bytearray.


**Returns:**
byte[] - En bytearray som representerar den aktuella instansen.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Deserialiserar en instans från en bytearray.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | array | byte[] | En bytearray att deserialisera från. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

