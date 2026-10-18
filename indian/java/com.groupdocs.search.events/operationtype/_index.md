---
title: "OperationType"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स ऑपरेशन प्रकार को दर्शाता है।"
type: docs
weight: 23
url: /hi/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

इंडेक्स ऑपरेशन प्रकार को दर्शाता है।

## Fields

| Field | विवरण |
| --- | --- |
|  | [Indexing](#Indexing) | इंडेक्स में दस्तावेज़ जोड़ना। |
|
|  | [Updating](#Updating) | इंडेक्स में दस्तावेज़ अपडेट करना। |
|
|  | [Merging](#Merging) | इंडेक्स को मर्ज करना। |
|
|  | [Optimizing](#Optimizing) | इंडेक्स को ऑप्टिमाइज़ करना। |
|
|  | [Deleting](#Deleting) | इंडेक्स से पथ हटाना। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


इंडेक्स में दस्तावेज़ जोड़ना।


### Updating {#Updating}
```
public static final OperationType Updating
```


इंडेक्स में दस्तावेज़ अपडेट करना।


### Merging {#Merging}
```
public static final OperationType Merging
```


इंडेक्स को मर्ज करना।


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


इंडेक्स को ऑप्टिमाइज़ करना।


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


इंडेक्स से पथ हटाना।


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
