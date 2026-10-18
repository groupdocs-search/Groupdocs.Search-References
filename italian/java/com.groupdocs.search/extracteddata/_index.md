---
title: "ExtractedData"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta i dati recuperati da un documento e preparati per l'indicizzazione."
type: docs
weight: 15
url: /it/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Rappresenta i dati recuperati da un documento e preparati per l'indicizzazione.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [serialize()](#serialize--) | Serializza l'istanza corrente in un array di byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Deserializza un'istanza da un array di byte. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serializza l'istanza corrente in un array di byte.


**Returns:**
byte[] - Un array di byte che rappresenta l'istanza corrente.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Deserializza un'istanza da un array di byte.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | array | byte[] | Un array di byte da cui deserializzare. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

