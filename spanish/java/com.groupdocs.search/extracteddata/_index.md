---
title: "ExtractedData"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los datos recuperados de un documento y preparados para la indexación."
type: docs
weight: 15
url: /es/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Representa los datos recuperados de un documento y preparados para la indexación.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [serialize()](#serialize--) | Serializa la instancia actual a una matriz de bytes. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializa una instancia a partir de una matriz de bytes. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serializa la instancia actual a una matriz de bytes.


**Returns:**
byte[] - Una matriz de bytes que representa la instancia actual.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Deserializa una instancia a partir de una matriz de bytes.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | matriz | byte[] | Una matriz de bytes desde la cual deserializar. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

