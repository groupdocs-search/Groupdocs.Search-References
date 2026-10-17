---
title: "MetadataIndexingOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لفهرسة حقول البيانات الوصفية."
type: docs
weight: 29
url: /ar/java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class MetadataIndexingOptions
```

يوفر خيارات لفهرسة حقول البيانات الوصفية.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MetadataIndexingOptions()](#MetadataIndexingOptions--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getIndexingEmptyValues()](#getIndexingEmptyValues--) | يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة قيم الحقول الفارغة أم لا. |
|
|  | [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة قيم الحقول الفارغة أم لا. |
|
|  | [getIndexingEmptyNames()](#getIndexingEmptyNames--) | يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة أسماء الحقول الفارغة أم لا. |
|
|  | [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة أسماء الحقول الفارغة أم لا. |
|
|  | [getDefaultFieldName()](#getDefaultFieldName--) | يحصل على اسم الحقل الافتراضي المستخدم لفهرسة أسماء الحقول الفارغة. |
|
|  | [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | يضبط اسم الحقل الافتراضي المستخدم لفهرسة أسماء الحقول الفارغة. |
|
|  | [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | يحصل على الفاصل في الاسم المركب لحقل. |
|
|  | [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | يضبط الفاصل في الاسم المركب لحقل. |
|
|  | [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع byte لفهرسة الحقل. |
|
|  | [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع byte لفهرسة الحقل. |
|
|  | [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع int لفهرسة الحقل. |
|
|  | [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع int لفهرسة الحقل. |
|
|  | [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع long لفهرسة الحقل. |
|
|  | [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع long لفهرسة الحقل. |
|
|  | [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع double لفهرسة الحقل. |
|
|  | [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع double لفهرسة الحقل. |
|
|  | [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | يحصل على الفاصل بين القيم في حقل من النوع array. |
|
|  | [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | يضبط الفاصل بين القيم في حقل من النوع array. |
|
### MetadataIndexingOptions() {#MetadataIndexingOptions--}
```
public MetadataIndexingOptions()
```


### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public abstract boolean getIndexingEmptyValues()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة قيم الحقول الفارغة أم لا. القيمة الافتراضية هي true.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان سيتم فهرسة قيم الحقول الفارغة أم لا.

### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public abstract void setIndexingEmptyValues(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة قيم الحقول الفارغة أم لا. القيمة الافتراضية هي true.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم فهرسة قيم الحقول الفارغة أم لا. |
|

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public abstract boolean getIndexingEmptyNames()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم فهرسة أسماء الحقول الفارغة أم لا. القيمة الافتراضية هي true.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان سيتم فهرسة أسماء الحقول الفارغة أم لا.

### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public abstract void setIndexingEmptyNames(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم فهرسة أسماء الحقول الفارغة أم لا. القيمة الافتراضية هي true.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم فهرسة أسماء الحقول الفارغة أم لا. |
|

### getDefaultFieldName() {#getDefaultFieldName--}
```
public abstract String getDefaultFieldName()
```


يحصل على اسم الحقل الافتراضي المستخدم لفهرسة أسماء الحقول الفارغة. القيمة الافتراضية هي "unknown".


**Returns:**
java.lang.String - الاسم الافتراضي للحقل المستخدم لفهرسة أسماء الحقول الفارغة.

### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public abstract void setDefaultFieldName(String value)
```


يضبط الاسم الافتراضي للحقل المستخدم لفهرسة أسماء الحقول الفارغة. القيمة الافتراضية هي "unknown".


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | الاسم الافتراضي للحقل المستخدم لفهرسة أسماء الحقول الفارغة. |
|

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public abstract String getSeparatorInCompoundName()
```


يحصل على الفاصل في الاسم المركب لحقل. القيمة الافتراضية هي ".".


**Returns:**
java.lang.String - الفاصل في الاسم المركب لحقل.

### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public abstract void setSeparatorInCompoundName(String value)
```


يضبط الفاصل في الاسم المركب لحقل. القيمة الافتراضية هي ".".


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | الفاصل في الاسم المركب لحقل. |
|

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public abstract int getMaxBytesToIndexField()
```


يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع byte لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Returns:**
int - الحد الأقصى لعدد القيم في مصفوفة من النوع byte لفهرسة الحقل.

### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public abstract void setMaxBytesToIndexField(int value)
```


يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع byte لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد القيم في مصفوفة من النوع byte لفهرسة الحقل. |
|

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public abstract int getMaxIntsToIndexField()
```


يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع int لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Returns:**
int - الحد الأقصى لعدد القيم في مصفوفة من النوع int لفهرسة الحقل.

### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public abstract void setMaxIntsToIndexField(int value)
```


يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع int لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد القيم في مصفوفة من النوع int لفهرسة الحقل. |
|

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public abstract int getMaxLongsToIndexField()
```


يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع long لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Returns:**
int - الحد الأقصى لعدد القيم في مصفوفة من النوع long لفهرسة الحقل.

### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public abstract void setMaxLongsToIndexField(int value)
```


يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع long لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد القيم في مصفوفة من النوع long لفهرسة الحقل. |
|

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public abstract int getMaxDoublesToIndexField()
```


يحصل على الحد الأقصى لعدد القيم في مصفوفة من النوع double لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Returns:**
int - الحد الأقصى لعدد القيم في مصفوفة من النوع double لفهرسة الحقل.

### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public abstract void setMaxDoublesToIndexField(int value)
```


يضبط الحد الأقصى لعدد القيم في مصفوفة من النوع double لفهرسة الحقل. القيمة الافتراضية هي Integer.MAX_VALUE.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | الحد الأقصى لعدد القيم في مصفوفة من النوع double لفهرسة الحقل. |
|

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public abstract String getSeparatorBetweenValues()
```


يحصل على الفاصل بين القيم في حقل من النوع array. القيمة الافتراضية هي علامة المسافة.


**Returns:**
java.lang.String - الفاصل بين القيم في حقل من النوع array.

### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public abstract void setSeparatorBetweenValues(String value)
```


يضبط الفاصل بين القيم في حقل من نوع المصفوفة. القيمة الافتراضية هي علامة المسافة.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | الفاصل بين القيم في حقل من نوع المصفوفة. |
|

