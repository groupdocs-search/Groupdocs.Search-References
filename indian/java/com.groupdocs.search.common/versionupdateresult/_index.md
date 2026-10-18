---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स संस्करण अपडेट ऑपरेशन के परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 42
url: /hi/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

इंडेक्स संस्करण अपडेट ऑपरेशन के परिणाम का प्रतिनिधित्व करता है।

## Fields

| Field | विवरण |
| --- | --- |
|  | [Updated](#Updated) | इंडेक्स संस्करण अपडेट किया गया। |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | इंडेक्स संस्करण पहले से ही अद्यतित है। |
|
|  | [Unsupported](#Unsupported) | इंडेक्स संस्करण समर्थित नहीं है या निर्देशिका में वैध इंडेक्स डेटा नहीं है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


इंडेक्स संस्करण अपडेट किया गया।


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


इंडेक्स संस्करण पहले से ही अद्यतित है।


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


इंडेक्स संस्करण समर्थित नहीं है या निर्देशिका में वैध इंडेक्स डेटा नहीं है।


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| नाम | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
