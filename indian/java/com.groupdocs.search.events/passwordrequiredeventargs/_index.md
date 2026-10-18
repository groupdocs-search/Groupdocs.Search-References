---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "जब पासवर्ड द्वारा संरक्षित दस्तावेज़ का अनुक्रमण हो रहा हो, तब होने वाली घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

जब पासवर्ड द्वारा संरक्षित दस्तावेज़ का अनुक्रमण हो रहा हो, तब होने वाली घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | दस्तावेज़ का पूर्ण पथ प्राप्त करता है। |
|
|  | [getPassword()](#getPassword--) | दस्तावेज़ खोलने के लिए पासवर्ड प्राप्त करता है। |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | दस्तावेज़ खोलने के लिए पासवर्ड सेट करता है। |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


दस्तावेज़ का पूर्ण पथ प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ का पूर्ण पथ।

### getPassword() {#getPassword--}
```
public final String getPassword()
```


दस्तावेज़ खोलने के लिए पासवर्ड प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ खोलने के लिए पासवर्ड।

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


दस्तावेज़ खोलने के लिए पासवर्ड सेट करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | java.lang.String | दस्तावेज़ खोलने के लिए पासवर्ड। |
|

