---
title: "IndexType"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स प्रकार निर्दिष्ट करता है।"
type: docs
weight: 49
url: /hi/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

इंडेक्स प्रकार निर्दिष्ट करता है।


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | विवरण |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | सामान्य सूचकांक जिसमें दस्तावेज़ मेटाडेटा और दस्तावेज़ सामग्री होती है और जो सभी खोज सुविधाओं का समर्थन करता है। |
|
|  | [MetadataIndex](#MetadataIndex) | एक सूचकांक जिसमें केवल दस्तावेज़ों का मेटाडेटा होता है, बिना सामग्री के। |
|
|  | [CompactIndex](#CompactIndex) | ऐसा सूचकांक प्रकार जो बहुत कम डिस्क स्थान लेता है लेकिन वाक्यांश खोज और तिथि सीमा खोज सुविधाओं का समर्थन नहीं करता। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


सामान्य सूचकांक जिसमें दस्तावेज़ मेटाडेटा और दस्तावेज़ सामग्री होती है और जो सभी खोज सुविधाओं का समर्थन करता है।


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


एक सूचकांक जिसमें केवल दस्तावेज़ों का मेटाडेटा होता है, बिना सामग्री के।


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


ऐसा सूचकांक प्रकार जो बहुत कम डिस्क स्थान लेता है लेकिन वाक्यांश खोज और तिथि सीमा खोज सुविधाओं का समर्थन नहीं करता।


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
