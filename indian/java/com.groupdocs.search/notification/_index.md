---
title: "सूचना"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स को सभी सूचनाओं के लिए आधार वर्ग।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

इंडेक्स के सभी सूचनाओं के लिए आधार वर्ग। यह वर्ग सूचना वस्तुओं को बनाने के लिए विधियों को भी शामिल करता है।


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [Notification()](#Notification--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | एक सूचना वस्तु बनाता है जो एक पुनःनामित किए गए अनुक्रमित दस्तावेज़ को पुनःनामित करती है और जिसे पुनः अनुक्रमित करने की आवश्यकता नहीं है। |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


एक सूचना वस्तु बनाता है जो एक पुनःनामित किए गए अनुक्रमित दस्तावेज़ को पुनःनामित करती है और जिसे पुनः अनुक्रमित करने की आवश्यकता नहीं है। पुनःनामित दस्तावेज़ अगले अद्यतन संचालन के दौरान पुनः अनुक्रमित नहीं किया जाएगा, भले ही उसकी सामग्री बदल गई हो।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | oldPath | java.lang.String | अनुक्रमित दस्तावेज़ का पुराना पथ। |
|
|  | newPath | java.lang.String | अनुक्रमित दस्तावेज़ का नया पथ। |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

