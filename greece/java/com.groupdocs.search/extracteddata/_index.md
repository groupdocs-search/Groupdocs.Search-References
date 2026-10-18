---
title: "ExtractedData"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει δεδομένα που ανακτώνται από ένα έγγραφο και προετοιμάζονται για ευρετηρίαση."
type: docs
weight: 15
url: /el/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

Αντιπροσωπεύει δεδομένα που ανακτώνται από ένα έγγραφο και προετοιμάζονται για ευρετηρίαση.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [serialize()](#serialize--) | Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Αποσειριοποιεί μια παρουσία από έναν πίνακα byte. |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Σειριοποιεί την τρέχουσα παρουσία σε έναν πίνακα byte.


**Returns:**
byte[] - Ένας πίνακας byte που αντιπροσωπεύει την τρέχουσα παρουσία.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


Αποσειριοποιεί μια παρουσία από έναν πίνακα byte.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | πίνακας | byte[] | Ένας πίνακας byte για αποσειριοποίηση. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

