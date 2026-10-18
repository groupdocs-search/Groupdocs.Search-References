---
title: "TextStorageSettings"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar textlagringsinställningarna."
type: docs
weight: 42
url: /sv/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Representerar textlagringsinställningarna.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Initierar en ny instans av klassen  TextStorageSettings  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCompression()](#getCompression--) | Hämtar komprimeringen av textlagring. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Ställer in komprimeringen av textlagring. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Initierar en ny instans av klassen  TextStorageSettings  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Komprimeringen av textlagring. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Hämtar komprimeringen av textlagring. Standardvärdet är Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Ställer in komprimeringen av textlagring. Standardvärdet är Compression.Normal.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | Komprimeringen av textlagring. |
|

