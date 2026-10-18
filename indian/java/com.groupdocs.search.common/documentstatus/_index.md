---
title: "DocumentStatus"
second_title: "GroupDocs.Search for Java API Reference"
description: "दस्तावेज़ प्रोसेसिंग स्थिति का प्रतिनिधित्व करता है।"
type: docs
weight: 40
url: /hi/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

दस्तावेज़ प्रोसेसिंग स्थिति का प्रतिनिधित्व करता है।

## Fields

| Field | विवरण |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | दस्तावेज़ सफलतापूर्वक अनुक्रमित किया गया। |
|
|  | [Skipped](#Skipped) | दस्तावेज़ छोड़ दिया गया। |
|
|  | [ProcessedWithError](#ProcessedWithError) | दस्तावेज़ अनुक्रमण के दौरान त्रुटि हुई। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


दस्तावेज़ सफलतापूर्वक अनुक्रमित किया गया।


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


दस्तावेज़ छोड़ दिया गया।


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


दस्तावेज़ अनुक्रमण के दौरान त्रुटि हुई।


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
