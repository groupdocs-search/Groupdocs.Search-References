---
title: "ExtractedData"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ से प्राप्त डेटा और इंडेक्सिंग के लिए तैयार किया गया डेटा का प्रतिनिधित्व करता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search/extracteddata/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedData
```

दस्तावेज़ से प्राप्त डेटा और इंडेक्सिंग के लिए तैयार किया गया डेटा का प्रतिनिधित्व करता है।

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [serialize()](#serialize--) | वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है। |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है। |
|
### serialize() {#serialize--}
```
public final byte[] serialize()
```


वर्तमान इंस्टेंस को बाइट एरे में सीरियलाइज़ करता है।


**Returns:**
byte[] - वर्तमान इंस्टेंस को दर्शाने वाला बाइट एरे।

### deserialize(byte[] array) {#deserialize-byte---}
```
public static ExtractedData deserialize(byte[] array)
```


बाइट एरे से एक इंस्टेंस को डीसीरियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | एरे | byte[] | डीसीरियलाइज़ करने के लिए बाइट एरे। |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - An instance deserialized from a byte array.

