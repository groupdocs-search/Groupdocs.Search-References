---
title: "ExtractedItemInfo"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل معلومات عنصر الحاوية."
type: docs
weight: 18
url: /ar/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

يمثل معلومات عنصر الحاوية.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | يُنشئ مثلاً جديداً من الفئة ExtractedItemInfo. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | يحصل على نوع المستند. |
|
|  | [getFields()](#getFields--) | يحصل على الحقول المستخرجة. |
|
|  | [getItemInfo()](#getItemInfo--) | يحصل على معلومات العنصر. |
|
|  | [getInnerPath()](#getInnerPath--) | يحصل على المسار الداخلي. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


يُنشئ مثلاً جديداً من الفئة ExtractedItemInfo.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | عائلة تنسيق المستند. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | الحقول المستخرجة. |
|
|  | itemInfo | java.lang.String | معلومات العنصر. |
|
|  | innerPath | java.lang.String | المسار إلى العنصر في الحاوية. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


يحصل على نوع المستند.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


يحصل على الحقول المستخرجة.


**Returns:**
com.groupdocs.search.common.DocumentField[] - الحقول المستخرجة.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


يحصل على معلومات العنصر.


**Returns:**
java.lang.String - معلومات العنصر.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


يحصل على المسار الداخلي.


**Returns:**
java.lang.String - المسار الداخلي.

