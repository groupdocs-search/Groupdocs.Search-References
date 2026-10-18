---
title: "Configuration"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक खोज नेटवर्क कॉन्फ़िगरेशन का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

एक खोज नेटवर्क कॉन्फ़िगरेशन का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | इस कॉन्फ़िगरेशन को फ़ाइल में सहेजता है। |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | इस कॉन्फ़िगरेशन को स्ट्रीम में सहेजता है। |
|
|  | [load(String filePath)](#load-java.lang.String-) | फ़ाइल से खोज नेटवर्क कॉन्फ़िगरेशन लोड करता है। |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | स्ट्रीम से खोज नेटवर्क कॉन्फ़िगरेशन लोड करता है। |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


इस कॉन्फ़िगरेशन को फ़ाइल में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | सहेजने के लिए फ़ाइल। |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


इस कॉन्फ़िगरेशन को स्ट्रीम में सहेजता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्ट्रीम | java.io.OutputStream | सहेजने के लिए स्ट्रीम। |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


फ़ाइल से खोज नेटवर्क कॉन्फ़िगरेशन लोड करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | लोड करने के लिए फ़ाइल। |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


स्ट्रीम से खोज नेटवर्क कॉन्फ़िगरेशन लोड करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | स्ट्रीम | java.io.InputStream | लोड करने के लिए स्ट्रीम। |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

