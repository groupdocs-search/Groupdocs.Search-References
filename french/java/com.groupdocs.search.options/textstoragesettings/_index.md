---
title: "TextStorageSettings"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les paramètres de stockage du texte."
type: docs
weight: 42
url: /fr/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Représente les paramètres de stockage du texte.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Initialise une nouvelle instance de la classe  TextStorageSettings . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getCompression()](#getCompression--) | Obtient la compression du stockage de texte. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Définit la compression du stockage de texte. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Initialise une nouvelle instance de la classe  TextStorageSettings .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | La compression du stockage de texte. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Obtient la compression du stockage de texte. La valeur par défaut est Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Définit la compression du stockage de texte. La valeur par défaut est Compression.Normal.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | La compression du stockage de texte. |
|

