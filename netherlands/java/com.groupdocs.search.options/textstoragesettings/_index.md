---
title: "TextStorageSettings"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de tekstopslaginstellingen voor."
type: docs
weight: 42
url: /nl/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Stelt de tekstopslaginstellingen voor.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Initialiseert een nieuw exemplaar van de  TextStorageSettings  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCompression()](#getCompression--) | Haalt de compressie van tekstopslag op. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Stelt de compressie van tekstopslag in. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Initialiseert een nieuw exemplaar van de  TextStorageSettings  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | De compressie van tekstopslag. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Haalt de compressie van tekstopslag op. De standaardwaarde is Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Stelt de compressie van tekstopslag in. De standaardwaarde is Compression.Normal.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | De compressie van tekstopslag. |
|

