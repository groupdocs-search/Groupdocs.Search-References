---
title: "Notification"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "الفئة الأساسية لجميع الإشعارات إلى الفهرس."
type: docs
weight: 22
url: /ar/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

الفئة الأساسية لجميع الإشعارات إلى الفهرس. تحتوي هذه الفئة أيضًا على طرق لإنشاء كائنات الإشعار.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [Notification()](#Notification--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | ينشئ كائن إشعار لإعادة تسمية مستند مفهرس تم إعادة تسميته ولا يحتاج إلى إعادة فهرسة. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


ينشئ كائن إشعار لإعادة تسمية مستند مفهرس تم إعادة تسميته ولا يحتاج إلى إعادة فهرسة. لن يتم إعادة فهرسة المستند المعاد تسميته أثناء عملية التحديث التالية، حتى إذا تم تغيير محتوياته.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | oldPath | java.lang.String | المسار القديم للمستند المفهرس. |
|
|  | newPath | java.lang.String | المسار الجديد للمستند المفهرس. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

