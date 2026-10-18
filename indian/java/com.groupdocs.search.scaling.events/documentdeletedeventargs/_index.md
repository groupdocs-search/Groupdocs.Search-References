---
title: "DocumentDeletedEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ विलोपन समाप्त होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

दस्तावेज़ विलोपन समाप्त होने की घटना के लिए तर्क दर्शाता है।

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | शार्ड इंडेक्स प्राप्त करता है। |
|
|  | [getDocumentKey()](#getDocumentKey--) | दस्तावेज़ कुंजी प्राप्त करता है। |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


शार्ड इंडेक्स प्राप्त करता है।


**Returns:**
int - शार्ड इंडेक्स।

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


दस्तावेज़ कुंजी प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ कुंजी।

