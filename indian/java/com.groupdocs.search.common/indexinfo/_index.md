---
title: "IndexInfo"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक इंडेक्स के बारे में मूलभूत जानकारी शामिल है।"
type: docs
weight: 24
url: /hi/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

इंडेक्स पर मूलभूत जानकारी शामिल करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | इंडेक्स का अद्वितीय पहचानकर्ता प्राप्त करता है। |
|
|  | [getIndexFolder()](#getIndexFolder--) | इंडेक्स जहाँ स्थित है, उस फ़ोल्डर का पूर्ण नाम प्राप्त करता है। |
|
|  | [getIndexStatus()](#getIndexStatus--) | इंडेक्स स्थिति प्राप्त करता है। |
|
|  | [getVersion()](#getVersion--) | इंडेक्स संस्करण प्राप्त करता है। |
|
|  | [getSegmentCount()](#getSegmentCount--) | इंडेक्स खंडों की संख्या प्राप्त करता है। |
|
|  | [getTermCount()](#getTermCount--) | इंडेक्स में शब्दों की संख्या प्राप्त करता है। |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


इंडेक्स का अद्वितीय पहचानकर्ता प्राप्त करता है।


**Returns:**
java.util.UUID - इंडेक्स का अद्वितीय पहचानकर्ता।

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


इंडेक्स जहाँ स्थित है, उस फ़ोल्डर का पूर्ण नाम प्राप्त करता है।


**Returns:**
java.lang.String - इंडेक्स जहाँ स्थित है, उस फ़ोल्डर का पूर्ण नाम।

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


इंडेक्स स्थिति प्राप्त करता है।


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


इंडेक्स संस्करण प्राप्त करता है।


**Returns:**
java.lang.String - इंडेक्स संस्करण।

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


इंडेक्स खंडों की संख्या प्राप्त करता है।


**Returns:**
int - इंडेक्स खंडों की संख्या।

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


इंडेक्स में शब्दों की संख्या प्राप्त करता है।


**Returns:**
int - इंडेक्स में शब्दों की संख्या।

