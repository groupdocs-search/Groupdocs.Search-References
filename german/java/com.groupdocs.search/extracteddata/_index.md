---
title: "ExtractedData"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Daten dar, die aus einem Dokument abgerufen und für die Indizierung vorbereitet wurden."
type: docs
weight: 15
url: /de/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Stellt Daten dar, die aus einem Dokument abgerufen und für die Indizierung vorbereitet wurden.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [serialize()](#serialize--) | Serialisiert die aktuelle Instanz in ein Byte-Array. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserialisiert eine Instanz aus einem Byte-Array. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serialisiert die aktuelle Instanz in ein Byte-Array.


**Returns:**
byte[] – Ein Byte-Array, das die aktuelle Instanz darstellt.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Deserialisiert eine Instanz aus einem Byte-Array.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Array | byte[] | Ein Byte-Array, aus dem deserialisiert werden soll. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

