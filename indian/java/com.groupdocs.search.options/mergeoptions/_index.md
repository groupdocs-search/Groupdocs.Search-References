---
title: "MergeOptions"
second_title: "GroupDocs.Search for Java API Reference"
description: "मर्ज ऑपरेशन के लिए विकल्प प्रदान करता है।"
type: docs
weight: 28
url: /hi/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

मर्ज ऑपरेशन के लिए विकल्प प्रदान करता है।


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | MergeOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [isAsync()](#isAsync--) | ऑपरेशन को असिंक्रोनस रूप से करने के फ़्लैग को प्राप्त करता है। |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | ऑपरेशन को असिंक्रोनस रूप से करने के फ़्लैग को सेट करता है। |
|
|  | [getCancellation()](#getCancellation--) | ऑपरेशन रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | ऑपरेशन रद्द करने वाले ऑब्जेक्ट को सेट करता है। |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


MergeOptions क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग प्राप्त करता है। डिफ़ॉल्ट मान false है।


**Returns:**
boolean - ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग।

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग सेट करता है। डिफ़ॉल्ट मान false है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | मान | boolean | ऑपरेशन को असिंक्रोनस रूप से करने का फ़्लैग। |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


ऑपरेशन रद्द करने वाले ऑब्जेक्ट को प्राप्त करता है। डिफ़ॉल्ट मान null है।


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


ऑपरेशन रद्द करने वाले ऑब्जेक्ट को सेट करता है। डिफ़ॉल्ट मान null है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | ऑपरेशन रद्द करने वाला ऑब्जेक्ट। |
|

