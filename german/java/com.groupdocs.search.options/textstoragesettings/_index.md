---
title: "TextStorageSettings"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt die Einstellungen für die Textspeicherung dar."
type: docs
weight: 42
url: /de/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Stellt die Einstellungen für die Textspeicherung dar.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Initialisiert eine neue Instanz der  TextStorageSettings  Klasse. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCompression()](#getCompression--) | Liest die Kompression der Textspeicherung. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Setzt die Kompression der Textspeicherung. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Initialisiert eine neue Instanz der  TextStorageSettings  Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Die Kompression der Textspeicherung. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Liest die Kompression der Textspeicherung. Der Standardwert ist Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Setzt die Kompression der Textspeicherung. Der Standardwert ist Compression.Normal.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | Die Kompression der Textspeicherung. |
|

