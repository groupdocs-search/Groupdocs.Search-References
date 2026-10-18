---
title: "FileLogger"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक लॉगर का प्रतिनिधित्व करता है जो घटनाओं और त्रुटियों को स्थानीय फ़ाइल में लॉग करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

एक लॉगर का प्रतिनिधित्व करता है जो घटनाओं और त्रुटियों को स्थानीय फ़ाइल में लॉग करता है।


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // लॉग फ़ाइल का पथ और अधिकतम 4 MB लंबाई निर्दिष्ट कर रहा है
Index index = new Index(indexFolder, settings); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchResult result = index.search(query); // इंडेक्स में खोजें
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | FileLogger क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | इंडेक्स में हुई त्रुटि को लॉग करता है। |
|
|  | [trace(String message)](#trace-java.lang.String-) | इंडेक्स में हुए इवेंट को लॉग करता है। |
|
|  | [getFilePath()](#getFilePath--) | लॉग फ़ाइल पथ प्राप्त करता है। |
|
|  | [getMaxSize()](#getMaxSize--) | लॉग फ़ाइल का अधिकतम आकार मेगाबाइट में प्राप्त करता है। |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


FileLogger क्लास का एक नया उदाहरण प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | फ़ाइलपथ | java.lang.String | लॉग फ़ाइल पथ। |
|
|  | maxSize | double | लॉग फ़ाइल का अधिकतम आकार मेगाबाइट में। मान 0.1 से 1000 की सीमा में होना चाहिए। |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


इंडेक्स में हुई त्रुटि को लॉग करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | संदेश | java.lang.String | त्रुटि संदेश। |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


इंडेक्स में हुए इवेंट को लॉग करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | संदेश | java.lang.String | इवेंट संदेश। |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


लॉग फ़ाइल पथ प्राप्त करता है।


**Returns:**
java.lang.String - लॉग फ़ाइल पथ।

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


लॉग फ़ाइल का अधिकतम आकार मेगाबाइट में प्राप्त करता है।


**Returns:**
double - मेगाबाइट में लॉग फ़ाइल का अधिकतम आकार।

