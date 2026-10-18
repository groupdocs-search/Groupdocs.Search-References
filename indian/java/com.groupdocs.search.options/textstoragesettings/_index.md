---
title: "TextStorageSettings"
second_title: "GroupDocs.Search for Java API Reference"
description: "टेक्स्ट स्टोरेज सेटिंग्स को दर्शाता है।"
type: docs
weight: 42
url: /hi/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

टेक्स्ट स्टोरेज सेटिंग्स को दर्शाता है।


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | TextStorageSettings क्लास की नई इंस्टेंस को प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getCompression()](#getCompression--) | टेक्स्ट स्टोरेज का संपीड़न प्राप्त करता है। |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | टेक्स्ट स्टोरेज का संपीड़न सेट करता है। |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


TextStorageSettings क्लास की नई इंस्टेंस को प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | टेक्स्ट स्टोरेज का संपीड़न। |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


टेक्स्ट स्टोरेज का संपीड़न प्राप्त करता है। डिफ़ॉल्ट मान Compression.Normal है।


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


टेक्स्ट स्टोरेज का संपीड़न सेट करता है। डिफ़ॉल्ट मान Compression.Normal है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | टेक्स्ट स्टोरेज का संपीड़न। |
|

