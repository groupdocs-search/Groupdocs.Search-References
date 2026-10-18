---
title: "ExtractedData"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt gegevens voor die uit een document zijn opgehaald en voorbereid voor indexering."
type: docs
weight: 15
url: /nl/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Stelt gegevens voor die uit een document zijn opgehaald en voorbereid voor indexering.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [serialize()](#serialize--) | Serialiseert de huidige instantie naar een byte-array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialiseert een instantie vanuit een byte-array. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serialiseert de huidige instantie naar een byte-array.


**Returns:**
byte[] - Een byte-array die de huidige instantie vertegenwoordigt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Deserialiseert een instantie vanuit een byte-array.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | array | byte[] | Een byte-array om van te deserialiseren. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

