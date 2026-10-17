---
title: "FoundDocument"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مستندًا تم العثور عليه."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

يمثل مستندًا تم العثور عليه.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | يحصل على معلومات المستند. |
|
|  | [getRelevance()](#getRelevance--) | يحصل على ملاءمة نتيجة البحث. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | يحصل على عدد التكرارات التي تم العثور عليها. |
|
|  | [getFoundFields()](#getFoundFields--) | يحصل على حقول المستند التي تم العثور عليها. |
|
|  | [getTerms()](#getTerms--) | يحصل على المصطلحات التي تم العثور عليها. |
|
|  | [getTermSequences()](#getTermSequences--) | يحصل على سلاسل المصطلحات التي تم العثور عليها. |
|
|  | [getAttributes()](#getAttributes--) | يحصل على السمات المرتبطة بالمستند الذي تم العثور عليه. |
|
|  | [toString()](#toString--) | يعيد تمثيل السلسلة للمستند الذي تم العثور عليه. |
|
|  | [serialize()](#serialize--) | يسلسل المثيل الحالي إلى مصفوفة بايت. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | يفك تسلسل مثيل من مصفوفة بايت. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


يحصل على معلومات المستند.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


يحصل على ملاءمة نتيجة البحث.


**Returns:**
double - ملاءمة نتيجة البحث.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


يحصل على عدد التكرارات التي تم العثور عليها.


**Returns:**
int - عدد مرات الظهور التي تم العثور عليها.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


يحصل على حقول المستند التي تم العثور عليها.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - حقول المستند التي تم العثور عليها.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


يحصل على المصطلحات التي تم العثور عليها. يتم تقييم القيمة في كل مرة يتم فيها الوصول إلى الخاصية.


**Returns:**
java.lang.String[] - المصطلحات التي تم العثور عليها.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


يحصل على سلاسل المصطلحات التي تم العثور عليها.


**Returns:**
java.lang.String[][] - سلاسل المصطلحات التي تم العثور عليها.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


يحصل على السمات المرتبطة بالمستند الموجود. يجب تمكين الخيار المقابل في خيارات البحث لاسترجاع السمات.


**Returns:**
java.lang.String[] - السمات المرتبطة بالمستند الموجود.

### toString() {#toString--}
```
public abstract String toString()
```


يعيد تمثيل السلسلة للمستند الذي تم العثور عليه.


**Returns:**
java.lang.String - سلسلة تمثل المستند الموجود.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


يسلسل المثيل الحالي إلى مصفوفة بايت.


**Returns:**
byte[] - مصفوفة بايت تمثل المثيل الحالي.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


يفك تسلسل مثيل من مصفوفة بايت.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مصفوفة | byte[] | مصفوفة بايت للتسلسل العكسي منها. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

