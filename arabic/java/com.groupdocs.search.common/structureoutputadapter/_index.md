---
title: "StructureOutputAdapter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل محول إخراج يجمع الإخراج كهيكل يحتوي على كل حقل على حدة."
type: docs
weight: 33
url: /ar/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

يمثل محول إخراج يجمع الإخراج كهيكل يحتوي على كل حقل على حدة.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | يقوم بإنشاء نسخة جديدة من الفئة StructureOutputAdapter. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getResult()](#getResult--) | يحصل على المصفوفة الناتجة من الحقول. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


يقوم بإنشاء نسخة جديدة من الفئة StructureOutputAdapter.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | تنسيق الإخراج. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


يحصل على المصفوفة الناتجة من الحقول.


**Returns:**
com.groupdocs.search.common.DocumentField[] - المصفوفة الناتجة من الحقول.

