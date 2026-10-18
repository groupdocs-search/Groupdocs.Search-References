---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "इवेंट तर्कों की बेस क्लास को दर्शाता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

इवेंट तर्कों की बेस क्लास को दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getTime()](#getTime--) | एक घटना का समय प्राप्त करता है। |
|
|  | [getIndexId()](#getIndexId--) | इंडेक्स आईडी प्राप्त करता है। |
|
|  | [getIndexFolder()](#getIndexFolder--) | इंडेक्स फ़ोल्डर प्राप्त करता है। |
|
|  | [getStatus()](#getStatus--) | इंडेक्स स्थिति प्राप्त करता है। |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


एक घटना का समय प्राप्त करता है।


**Returns:**
java.util.Date - एक घटना का समय।

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


इंडेक्स आईडी प्राप्त करता है।


**Returns:**
java.util.UUID - इंडेक्स आईडी।

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


इंडेक्स फ़ोल्डर प्राप्त करता है।


**Returns:**
java.lang.String - इंडेक्स फ़ोल्डर।

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


इंडेक्स स्थिति प्राप्त करता है।


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

