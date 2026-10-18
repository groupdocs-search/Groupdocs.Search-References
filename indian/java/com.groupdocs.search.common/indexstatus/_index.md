---
title: "IndexStatus"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स स्थिति को निर्दिष्ट करता है।"
type: docs
weight: 41
url: /hi/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

इंडेक्स स्थिति को निर्दिष्ट करता है।

## Fields

| Field | विवरण |
| --- | --- |
|  | [Ready](#Ready) | सूचक (इंडेक्स) मुक्त है और परिवर्तन के लिए तैयार है। |
|
|  | [Failed](#Failed) | त्रुटि के कारण सूचक को पुनः लोड करने की आवश्यकता है। |
|
|  | [Indexing](#Indexing) | सूचक एक अनुक्रमण ऑपरेशन करता है। |
|
|  | [Updating](#Updating) | सूचक एक अद्यतन ऑपरेशन करता है। |
|
|  | [Merging](#Merging) | सूचक एक मर्जिंग ऑपरेशन करता है। |
|
|  | [Optimizing](#Optimizing) | सूचक एक अनुकूलन ऑपरेशन करता है। |
|
|  | [Deleting](#Deleting) | Index एक हटाने का ऑपरेशन करता है। |
|
|  | [Renaming](#Renaming) | Index एक नाम बदलने का ऑपरेशन करता है। |
|
|  | [ChangingAttributes](#ChangingAttributes) | Index गुण बदलता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


सूचक (इंडेक्स) मुक्त है और परिवर्तन के लिए तैयार है।


### Failed {#Failed}
```
public static final IndexStatus Failed
```


त्रुटि के कारण सूचक को पुनः लोड करने की आवश्यकता है।


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


सूचक एक अनुक्रमण ऑपरेशन करता है।


### Updating {#Updating}
```
public static final IndexStatus Updating
```


सूचक एक अद्यतन ऑपरेशन करता है।


### Merging {#Merging}
```
public static final IndexStatus Merging
```


सूचक एक मर्जिंग ऑपरेशन करता है।


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


सूचक एक अनुकूलन ऑपरेशन करता है।


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Index एक हटाने का ऑपरेशन करता है।


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Index एक नाम बदलने का ऑपरेशन करता है।


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Index गुण बदलता है।


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
