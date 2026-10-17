---
title: "CustomExtractorCollection"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يحتوي على مجموعة من المستخرجين المخصصين."
type: docs
weight: 13
url: /ar/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

يحتوي على مجموعة من المستخرجين المخصصين. إذا احتوت المجموعة على مستخرج لامتداد ملف ما يغطيه المستخرجون المدمجون، فسيتم استخدام هذا المستخرج بدلاً من المدمج.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [size()](#size--) | يسترجع عدد المستخرجين الموجودين في المجموعة. |
|
|  | [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت المجموعة للقراءة فقط. |
|
|  | [iterator()](#iterator--) | يرجع مكرراً لهذه المجموعة. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | يضيف مستخرجًا إلى المجموعة. |
|
|  | [clear()](#clear--) | يزيل جميع المستخرجين من المجموعة. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | يحدد ما إذا كانت المجموعة تحتوي على مستخرج معين. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | ينسخ عناصر المجموعة إلى مصفوفة، بدءًا من فهرس مصفوفة معين. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | يزيل مستخرجًا من المجموعة. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


يسترجع عدد المستخرجين الموجودين في المجموعة.


**Returns:**
int - عدد المستخرجين الموجودين في المجموعة.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت المجموعة للقراءة فقط.


**Returns:**
boolean - قيمة تشير إلى ما إذا كانت المجموعة للقراءة فقط.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


يرجع مكرراً لهذه المجموعة.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - كائن مكرّر يمكن استخدامه للتنقل عبر المجموعة.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


يضيف مستخرجًا إلى المجموعة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | المستخرج لإضافته إلى المجموعة. |
|

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع المستخرجين من المجموعة.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


يحدد ما إذا كانت المجموعة تحتوي على مستخرج معين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | المستخرج لتحديد موقعه في المجموعة. |
|

**Returns:**
منطقي -  true  إذا تم العثور على العنصر في المجموعة؛ وإلا  false .

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


ينسخ عناصر المجموعة إلى مصفوفة، بدءًا من فهرس مصفوفة معين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | المصفوفة أحادية البعد التي هي وجهة العناصر المنقولة من المجموعة. يجب أن تكون المصفوفة ذات فهرسة تبدأ من الصفر. |
|
|  | arrayIndex | int | الفهرس الصفري في المصفوفة الذي يبدأ النسخ عنده. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


يزيل مستخرجًا من المجموعة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | المستخرج لإزالته من المجموعة. |
|

**Returns:**
منطقي -  true إذا تم إزالة المستخرج بنجاح من المجموعة؛ وإلا  false . تُعيد هذه الطريقة أيضًا  false  إذا لم يتم العثور على المستخرج في المجموعة الأصلية.

