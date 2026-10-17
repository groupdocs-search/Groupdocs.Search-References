---
title: "IContainerItemExtractor"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر طرقًا لاستخراج العناصر من المستندات الحاوية."
type: docs
weight: 35
url: /ar/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

يوفر طرقًا لاستخراج العناصر من المستندات الحاوية.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | يسترجع عائلة تنسيق المستند. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | يستخرج العناصر من مستند الحاوية. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | يستخرج العناصر من مستند الحاوية. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


يسترجع عائلة تنسيق المستند.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


يستخرج العناصر من مستند الحاوية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار الملف. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - مصفوفة من العناصر المستخرجة.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


يستخرج العناصر من مستند الحاوية.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | stream | java.io.InputStream | تيار المستند. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - مصفوفة من العناصر المستخرجة.

