---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक आउटपुट एडाप्टर को दर्शाता है जो आउटपुट को java.io.OutputStream में एकत्र करता है।"
type: docs
weight: 31
url: /hi/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को java.io.OutputStream में एकत्र करता है।


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // आउटपुट स्ट्रीम बना रहा है
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // स्ट्रीम आउटपुट एडाप्टर बना रहा है
index.getDocumentText(documents[0], adapter); // दस्तावेज़ का पाठ स्ट्रीम में उत्पन्न कर रहा है
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | StreamOutputAdapter क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getStream()](#getStream--) | एक आउटपुट स्ट्रीम प्राप्त करता है। |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


StreamOutputAdapter क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | आउटपुट फ़ॉर्मेट। |
|
|  | स्ट्रीम | java.io.OutputStream | आउटपुट स्ट्रीम। |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


एक आउटपुट स्ट्रीम प्राप्त करता है।


**Returns:**
java.io.OutputStream - आउटपुट स्ट्रीम।

