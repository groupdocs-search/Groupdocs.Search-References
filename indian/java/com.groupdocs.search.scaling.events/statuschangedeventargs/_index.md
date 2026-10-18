---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज नेटवर्क स्थिति परिवर्तन घटना के लिए तर्क दर्शाता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

खोज नेटवर्क स्थिति परिवर्तन घटना के लिए तर्क दर्शाता है।

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | पुरानी सर्च नेटवर्क स्थिति प्राप्त करता है। |
|
|  | [getNewStatus()](#getNewStatus--) | नई सर्च नेटवर्क स्थिति प्राप्त करता है। |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


पुरानी सर्च नेटवर्क स्थिति प्राप्त करता है।


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


नई सर्च नेटवर्क स्थिति प्राप्त करता है।


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

