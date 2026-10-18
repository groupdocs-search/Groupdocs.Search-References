---
title: "ImageSearchResult"
second_title: "GroupDocs.Search for Java API Reference"
description: "रिवर्स इमेज सर्च के परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 17
url: /hi/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

रिवर्स इमेज सर्च के परिणाम का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | पाए गए चित्रों की संख्या प्राप्त करता है। |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | सूचकांक द्वारा पाए गए चित्र को प्राप्त करता है। |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


पाए गए चित्रों की संख्या प्राप्त करता है।


**Returns:**
int - पाए गए चित्रों की संख्या।

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


सूचकांक द्वारा पाए गए चित्र को प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | पाए गए चित्र का सूचकांक। |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

