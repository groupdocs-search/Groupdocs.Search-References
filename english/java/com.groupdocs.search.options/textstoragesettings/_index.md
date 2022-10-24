---
title: TextStorageSettings
second_title: GroupDocs.Search for Java API Reference
description: Represents the text storage settings.
type: docs
weight: 38
url: /java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Represents the text storage settings.

**Learn more**

 *  [Storing text of indexed documents][]
 *  [Search index settings][]


[Storing text of indexed documents]: https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents
[Search index settings]: https://docs.groupdocs.com/display/searchjava/Search+index+settings
## Constructors

| Constructor | Description |
| --- | --- |
| [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Initializes a new instance of the  TextStorageSettings  class. |
## Methods

| Method | Description |
| --- | --- |
| [getCompression()](#getCompression--) | Gets the compression of text storage. |
| [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Sets the compression of text storage. |
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Initializes a new instance of the  TextStorageSettings  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compression | [Compression](../../com.groupdocs.search.options/compression) | The compression of text storage. |

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Gets the compression of text storage. The default value is Compression.Normal.

**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.
### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Sets the compression of text storage. The default value is Compression.Normal.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Compression](../../com.groupdocs.search.options/compression) | The compression of text storage. |

