---
title: "OperationFinishedEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "अनुक्रमण ऑपरेशन समाप्त होने की घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

अनुक्रमण ऑपरेशन समाप्त होने की घटना के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getMessage()](#getMessage--) | संदेश प्राप्त करता है। |
|
|  | [getOperationType()](#getOperationType--) | ऑपरेशन प्रकार प्राप्त करता है। |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


संदेश प्राप्त करता है।


**Returns:**
java.lang.String - संदेश।

### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


ऑपरेशन प्रकार प्राप्त करता है।


**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.

