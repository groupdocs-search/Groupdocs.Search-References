---
title: "SearchImage"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज के लिए एक छवि का प्रतिनिधित्व करता है।"
type: docs
weight: 29
url: /hi/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

खोज के लिए एक छवि का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | फ़ाइल से खोज के लिए एक इमेज बनाता है। |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | फ़ाइल से खोज के लिए एक इमेज बनाता है। |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | स्ट्रीम से खोज के लिए एक इमेज बनाता है। |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | स्ट्रीम से खोज के लिए एक इमेज बनाता है। |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


फ़ाइल से खोज के लिए एक इमेज बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | इमेज फ़ाइल पथ। |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


फ़ाइल से खोज के लिए एक इमेज बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | इमेज फ़ाइल पथ। |
|
|  | imageIndex | int | बहु-पृष्ठ इमेज में इमेज इंडेक्स। |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


स्ट्रीम से खोज के लिए एक इमेज बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्ट्रीम | java.io.InputStream | इमेज स्ट्रीम। |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


स्ट्रीम से खोज के लिए एक इमेज बनाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्ट्रीम | java.io.InputStream | इमेज स्ट्रीम। |
|
|  | imageIndex | int | बहु-पृष्ठ इमेज में इमेज इंडेक्स। |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

