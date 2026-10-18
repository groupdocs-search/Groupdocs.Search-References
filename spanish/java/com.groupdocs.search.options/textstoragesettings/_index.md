---
title: "TextStorageSettings"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa la configuración de almacenamiento de texto."
type: docs
weight: 42
url: /es/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Representa la configuración de almacenamiento de texto.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Inicializa una nueva instancia de la  TextStorageSettings  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCompression()](#getCompression--) | Obtiene la compresión del almacenamiento de texto. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Establece la compresión del almacenamiento de texto. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Inicializa una nueva instancia de la  TextStorageSettings  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | La compresión del almacenamiento de texto. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Obtiene la compresión del almacenamiento de texto. El valor predeterminado es Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Establece la compresión del almacenamiento de texto. El valor predeterminado es Compression.Normal.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | La compresión del almacenamiento de texto. |
|

