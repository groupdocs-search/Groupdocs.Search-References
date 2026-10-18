---
title: "TextStorageSettings"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta le impostazioni di archiviazione del testo."
type: docs
weight: 42
url: /it/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Rappresenta le impostazioni di archiviazione del testo.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Inizializza una nuova istanza della classe  TextStorageSettings . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getCompression()](#getCompression--) | Ottiene la compressione dell'archiviazione del testo. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Imposta la compressione dell'archiviazione del testo. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Inizializza una nuova istanza della classe  TextStorageSettings .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | La compressione dell'archiviazione del testo. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Ottiene la compressione dell'archiviazione del testo. Il valore predefinito è Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Imposta la compressione dell'archiviazione del testo. Il valore predefinito è Compression.Normal.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | La compressione dell'archiviazione del testo. |
|

