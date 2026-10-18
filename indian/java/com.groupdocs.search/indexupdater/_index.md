---
title: "IndexUpdater"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्स अपडेटर का प्रतिनिधित्व करता है।"
type: docs
weight: 20
url: /hi/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

एक इंडेक्स अपडेटर को दर्शाता है। यह क्लास पुराने संस्करण के इंडेक्स में दस्तावेज़ों का पुनःइंडेक्सिंग करती है।


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

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


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | IndexUpdater क्लास का एक नया उदाहरण प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | जाँचता है कि निर्दिष्ट डायरेक्टरी में नवीनतम संस्करण का इंडेक्स मौजूद है या नहीं। |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | जाँचता है कि निर्दिष्ट डायरेक्टरी में मौजूद इंडेक्स को नवीनतम संस्करण में अपडेट किया जा सकता है या नहीं। |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | पुराने संस्करण के इंडेक्स में दस्तावेज़ों का पुनःइंडेक्सिंग करता है। |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


IndexUpdater क्लास का एक नया उदाहरण प्रारंभ करता है।


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


जाँचता है कि निर्दिष्ट डायरेक्टरी में नवीनतम संस्करण का इंडेक्स मौजूद है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexPath | java.lang.String | इंडेक्स डायरेक्टरी पाथ। |
|

**Returns:**
boolean -  true  यदि निर्दिष्ट डायरेक्टरी में नवीनतम संस्करण का इंडेक्स मौजूद है; अन्यथा  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


जाँचता है कि निर्दिष्ट डायरेक्टरी में मौजूद इंडेक्स को नवीनतम संस्करण में अपडेट किया जा सकता है या नहीं।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexPath | java.lang.String | इंडेक्स डायरेक्टरी पाथ। |
|

**Returns:**
boolean -  true  यदि निर्दिष्ट डायरेक्टरी में इंडेक्स को नवीनतम संस्करण में अपडेट किया जा सकता है; अन्यथा  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


पुराने संस्करण के इंडेक्स में दस्तावेज़ों का पुनःइंडेक्सिंग करता है। अपडेट किया गया इंडेक्स  newIndexPath  डायरेक्टरी में रखा जाएगा।  indexPath  डायरेक्टरी में मौजूद इंडेक्स नहीं बदलेगा।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | indexPath | java.lang.String | इंडेक्स डायरेक्टरी पाथ। |
|
|  | newIndexPath | java.lang.String | अपडेट किए गए इंडेक्स के लिए डायरेक्टरी। |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

