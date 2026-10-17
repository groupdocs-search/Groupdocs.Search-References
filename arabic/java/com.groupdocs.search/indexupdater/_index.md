---
title: "IndexUpdater"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مُحدّث الفهرس."
type: docs
weight: 20
url: /ar/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

يمثل محدث الفهرس. تقوم هذه الفئة بإعادة فهرسة المستندات في فهرس نسخة قديمة.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String sourceIndexFolder = "c:\\MyOldIndex\\";
String targetIndexFolder = "c:\\MyNewIndex\\";
IndexUpdater updater = new IndexUpdater();
if (updater.canUpdateVersion(sourceIndexFolder)) {
int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
}
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | يقوم بتهيئة نسخة جديدة من الفئة  IndexUpdater . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | يتحقق مما إذا كان الدليل المحدد يحتوي على فهرس بأحدث نسخة. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | يتحقق مما إذا كان الفهرس في الدليل المحدد يمكن تحديثه إلى أحدث نسخة. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | ينفذ إعادة فهرسة المستندات في فهرس نسخة قديمة. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


يقوم بتهيئة نسخة جديدة من الفئة  IndexUpdater .


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


يتحقق مما إذا كان الدليل المحدد يحتوي على فهرس بأحدث نسخة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexPath | java.lang.String | مسار دليل الفهرس. |
|

**Returns:**
منطقي -  true  إذا كان الدليل المحدد يحتوي على فهرس بأحدث نسخة؛ وإلا  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


يتحقق مما إذا كان الفهرس في الدليل المحدد يمكن تحديثه إلى أحدث نسخة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexPath | java.lang.String | مسار دليل الفهرس. |
|

**Returns:**
منطقي -  true  إذا كان الفهرس في الدليل المحدد يمكن تحديثه إلى أحدث نسخة؛ وإلا  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


ينفذ إعادة فهرسة المستندات في فهرس نسخة قديمة. سيتم وضع الفهرس المحدث في دليل  newIndexPath . الفهرس في دليل  indexPath  لن يتغير.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | indexPath | java.lang.String | مسار دليل الفهرس. |
|
|  | newIndexPath | java.lang.String | الدليل الخاص بالفهرس المحدث. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

