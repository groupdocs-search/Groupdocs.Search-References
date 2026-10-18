---
title: "Cancellation"
second_title: "GroupDocs.Search for Java API Reference"
description: "ऑपरेशन रद्द करने के अनुरोध के लिए एक ऑब्जेक्ट का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

ऑपरेशन रद्द करने के अनुरोध के लिए एक ऑब्जेक्ट का प्रतिनिधित्व करता है।


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | नया उदाहरण प्रारंभ करता है |
Cancellation
वर्ग।
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | एक मान प्राप्त करता है जो दर्शाता है कि रद्दीकरण का अनुरोध किया गया है। |
|
|  | [cancel()](#cancel--) | रद्दीकरण के लिए अनुरोध करता है। |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | निर्दिष्ट मिलीसेकंड की अवधि के बाद रद्दीकरण के लिए अनुरोध करता है। |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


नया उदाहरण प्रारंभ करता है
Cancellation
वर्ग।


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


एक मान प्राप्त करता है जो दर्शाता है कि रद्दीकरण का अनुरोध किया गया है।


**Returns:**
boolean - एक मान जो दर्शाता है कि रद्दीकरण का अनुरोध किया गया है।

### cancel() {#cancel--}
```
public final void cancel()
```


रद्दीकरण के लिए अनुरोध करता है।


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


निर्दिष्ट मिलीसेकंड की अवधि के बाद रद्दीकरण के लिए अनुरोध करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | milliseconds | int | मिलीसेकंड की संख्या जिसके बाद कोई ऑपरेशन रद्द किया जाएगा। |
|

