---
title: "FoundDocumentField"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل حقل مستند تم العثور عليه."
type: docs
weight: 15
url: /ar/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

يمثل حقل مستند تم العثور عليه.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | يحصل على اسم الحقل. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | يحصل على عدد التكرارات التي تم العثور عليها. |
|
|  | [getTerms()](#getTerms--) | يحصل على المصطلحات التي تم العثور عليها. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | يحصل على مرات الظهور للمصطلحات التي تم العثور عليها. |
|
|  | [getTermSequences()](#getTermSequences--) | يحصل على سلاسل المصطلحات التي تم العثور عليها. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | يحصل على مرات الظهور لسلاسل المصطلحات التي تم العثور عليها. |
|
|  | [toString()](#toString--) | يعيد تمثيل السلسلة للحقل المستند الذي تم العثور عليه. |
|
|  | [serialize()](#serialize--) | يسلسل المثيل الحالي إلى مصفوفة بايت. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | يفك تسلسل مثيل من مصفوفة بايت. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


يحصل على اسم الحقل.


**Returns:**
java.lang.String - اسم الحقل.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


يحصل على عدد التكرارات التي تم العثور عليها.


**Returns:**
int - عدد مرات الظهور التي تم العثور عليها.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


يحصل على المصطلحات التي تم العثور عليها.


**Returns:**
java.lang.String[] - المصطلحات التي تم العثور عليها.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


يحصل على مرات الظهور للمصطلحات التي تم العثور عليها.


**Returns:**
int[] - مرات الظهور للمصطلحات التي تم العثور عليها.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


يحصل على سلاسل المصطلحات التي تم العثور عليها.


**Returns:**
java.lang.String[][] - سلاسل المصطلحات التي تم العثور عليها.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


يحصل على مرات الظهور لسلاسل المصطلحات التي تم العثور عليها.


**Returns:**
int[] - مرات الظهور لسلاسل المصطلحات التي تم العثور عليها.

### toString() {#toString--}
```
public abstract String toString()
```


يعيد تمثيل السلسلة للحقل المستند الذي تم العثور عليه.


**Returns:**
java.lang.String - سلسلة تمثل الحقل المستند الذي تم العثور عليه.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


يسلسل المثيل الحالي إلى مصفوفة بايت.


**Returns:**
byte[] - مصفوفة بايت تمثل المثيل الحالي.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


يفك تسلسل مثيل من مصفوفة بايت.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | مصفوفة | byte[] | مصفوفة بايت للتسلسل العكسي منها. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

