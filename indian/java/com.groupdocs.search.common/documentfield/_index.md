---
title: "DocumentField"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक दस्तावेज़ फ़ील्ड डेटा का प्रतिनिधित्व करता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search.common/documentfield/
---
**Inheritance:**
java.lang.Object
```
public class DocumentField
```

एक दस्तावेज़ फ़ील्ड डेटा का प्रतिनिधित्व करता है।


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)
* [Indexing additional fields](../https://docs.groupdocs.com/display/searchjava/Indexing+additional+fields)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [DocumentField(String name, String value)](#DocumentField-java.lang.String-java.lang.String-) | DocumentField क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
|  | [DocumentField(Object data)](#DocumentField-java.lang.Object-) | DocumentField क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getName()](#getName--) | फ़ील्ड का नाम प्राप्त करता है। |
|
|  | [getValue()](#getValue--) | फ़ील्ड का मान प्राप्त करता है। |
|
| [getCore()](#getCore--) |  |
### DocumentField(String name, String value) {#DocumentField-java.lang.String-java.lang.String-}
```
public DocumentField(String name, String value)
```


DocumentField क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | नाम | java.lang.String | फ़ील्ड का नाम। |
|
|  | मान | java.lang.String | फ़ील्ड का मान। |
|

### DocumentField(Object data) {#DocumentField-java.lang.Object-}
```
public DocumentField(Object data)
```


DocumentField क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### getName() {#getName--}
```
public String getName()
```


फ़ील्ड का नाम प्राप्त करता है।


**Returns:**
java.lang.String - फ़ील्ड नाम।

### getValue() {#getValue--}
```
public String getValue()
```


फ़ील्ड का मान प्राप्त करता है।


**Returns:**
java.lang.String - फ़ील्ड का मान।

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
