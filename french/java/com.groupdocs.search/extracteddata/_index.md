---
title: "ExtractedData"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les données récupérées d'un document et préparées pour l'indexation."
type: docs
weight: 15
url: /fr/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Représente les données récupérées d'un document et préparées pour l'indexation.

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [serialize()](#serialize--) | Sérialise l'instance actuelle en un tableau d'octets. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Désérialise une instance à partir d'un tableau d'octets. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Sérialise l'instance actuelle en un tableau d'octets.


**Returns:**
byte[] - Un tableau d'octets représentant l'instance actuelle.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Désérialise une instance à partir d'un tableau d'octets.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | tableau | byte[] | Un tableau d'octets à désérialiser. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

