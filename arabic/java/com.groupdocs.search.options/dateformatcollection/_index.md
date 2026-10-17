---
title: "DateFormatCollection"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مجموعة من كائنات DateFormat."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

يمثل مجموعة من كائنات DateFormat.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | يضيف كائن تنسيق تاريخ إلى المجموعة. |
|
|  | [clear()](#clear--) | يزيل جميع العناصر من المجموعة. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | يحدد ما إذا كانت المجموعة تحتوي على عنصر محدد. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | ينسخ عناصر المجموعة إلى مصفوفة Array، بدءًا من فهرس Array معين. |
|
|  | [size()](#size--) | يحصل على عدد العناصر الموجودة في المجموعة. |
|
|  | [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كانت المجموعة للقراءة فقط. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | يزيل أول ظهور لعنصر محدد من المجموعة. |
|
|  | [iterator()](#iterator--) | يعيد مُعدِّدًا يتنقل عبر المجموعة. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


يضيف كائن تنسيق تاريخ إلى المجموعة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | كائن تنسيق التاريخ لإضافته إلى المجموعة. |
|

### clear() {#clear--}
```
public abstract void clear()
```


يزيل جميع العناصر من المجموعة.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


يحدد ما إذا كانت المجموعة تحتوي على عنصر محدد.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | العنصر لتحديد موقعه في المجموعة. |
|

**Returns:**
boolean - true إذا تم العثور على العنصر في المجموعة؛ وإلا false.

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


ينسخ عناصر المجموعة إلى مصفوفة Array، بدءًا من فهرس Array معين.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | المصفوفة الأحادية البعد Array التي هي وجهة العناصر المنسوخة من المجموعة. |
|
|  | arrayIndex | int | الفهرس الصفري في المصفوفة الذي يبدأ النسخ عنده. |
|

### size() {#size--}
```
public abstract int size()
```


يحصل على عدد العناصر الموجودة في المجموعة.


**Returns:**
int - عدد العناصر الموجودة في المجموعة.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كانت المجموعة للقراءة فقط.


**Returns:**
boolean -  true  إذا كانت المجموعة للقراءة فقط؛ وإلا،  false .

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


يزيل أول ظهور لعنصر محدد من المجموعة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | العنصر المراد إزالته من المجموعة. |
|

**Returns:**
boolean -  true  إذا تم إزالة العنصر بنجاح من المجموعة؛ وإلا،  false . تُعيد هذه الطريقة أيضًا  false  إذا لم يُعثر على العنصر في المجموعة.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


يعيد مُعدِّدًا يتنقل عبر المجموعة.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - عداد يمكن استخدامه للتنقل عبر المجموعة.

