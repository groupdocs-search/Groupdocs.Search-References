---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स त्रुटि उत्पन्न होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 16
url: /hi/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

इंडेक्स त्रुटि उत्पन्न होने की घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getMessage()](#getMessage--) | त्रुटि संदेश प्राप्त करता है। |
|
|  | [isCritical()](#isCritical--) | एक फ़्लैग प्राप्त करता है जो दर्शाता है कि त्रुटि गंभीर है और इंडेक्स को पुनः शुरू किया जाना चाहिए। |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


त्रुटि संदेश प्राप्त करता है।


**Returns:**
java.lang.String - त्रुटि संदेश।

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


एक फ़्लैग प्राप्त करता है जो दर्शाता है कि त्रुटि गंभीर है और इंडेक्स को पुनः शुरू किया जाना चाहिए।


**Returns:**
boolean - वह फ़्लैग जो दर्शाता है कि त्रुटि गंभीर है और इंडेक्स को पुनः शुरू किया जाना चाहिए।

