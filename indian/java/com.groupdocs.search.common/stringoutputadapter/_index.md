---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को System.String के रूप में एकत्र करता है।"
type: docs
weight: 32
url: /hi/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को System.String के रूप में एकत्र करता है।


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
DocumentInfo[] documents = index.getIndexedDocuments(); // इंडेक्स किए गए दस्तावेज़ों की जानकारी प्राप्त कर रहा है
StringOutputAdapter adapter = new StringOutputAdapter(); // एक स्ट्रिंग आउटपुट एडाप्टर बना रहा है
index.getDocumentText(documents[0], adapter); // एडाप्टर में दस्तावेज़ टेक्स्ट उत्पन्न कर रहा है
String result = adapter.getResult(); // परिणाम प्राप्त कर रहा है
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StringOutputAdapter क्लास का नया इंस्टेंस प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getResult()](#getResult--) | परिणामी स्ट्रिंग प्राप्त करता है। |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


StringOutputAdapter क्लास का नया इंस्टेंस प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | आउटपुट फ़ॉर्मेट। |
|

### getResult() {#getResult--}
```
public final String getResult()
```


परिणामी स्ट्रिंग प्राप्त करता है।


**Returns:**
java.lang.String - परिणामी स्ट्रिंग।

