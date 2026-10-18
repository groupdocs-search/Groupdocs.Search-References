---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को फ़ाइल में एकत्र करता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

एक आउटपुट एडाप्टर का प्रतिनिधित्व करता है जो आउटपुट को फ़ाइल में एकत्र करता है।


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // फ़ाइल आउटपुट एडाप्टर बना रहा है
index.getDocumentText(documents[0], adapter); // आउटपुट फ़ाइल में दस्तावेज़ टेक्स्ट उत्पन्न कर रहा है
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | FileOutputAdapter क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | एक आउटपुट फ़ाइल पथ प्राप्त करता है। |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


FileOutputAdapter क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | आउटपुट फ़ॉर्मेट। |
|
|  | फ़ाइलपथ | java.lang.String | आउटपुट फ़ाइल पथ। |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


एक आउटपुट फ़ाइल पथ प्राप्त करता है।


**Returns:**
java.lang.String - आउटपुट फ़ाइल पथ।

