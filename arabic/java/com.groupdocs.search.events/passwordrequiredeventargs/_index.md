---
title: "PasswordRequiredEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات للحدث الذي يحدث عندما يتم فهرسة مستند محمي بكلمة مرور."
type: docs
weight: 20
url: /ar/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات للحدث الذي يحدث عندما يتم فهرسة مستند محمي بكلمة مرور.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | يحصل على المسار الكامل للمستند. |
|
|  | [getPassword()](#getPassword--) | يحصل على كلمة المرور لفتح المستند. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | يضبط كلمة المرور لفتح المستند. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


يحصل على المسار الكامل للمستند.


**Returns:**
java.lang.String - المسار الكامل للمستند.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


يحصل على كلمة المرور لفتح المستند.


**Returns:**
java.lang.String - كلمة المرور لفتح المستند.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


يضبط كلمة المرور لفتح المستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | كلمة المرور لفتح المستند. |
|

