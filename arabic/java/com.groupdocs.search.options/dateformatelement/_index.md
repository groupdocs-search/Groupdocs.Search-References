---
title: "DateFormatElement"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل عنصر تنسيق تاريخ."
type: docs
weight: 15
url: /ar/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

يمثل عنصر تنسيق تاريخ.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFormat()](#getFormat--) | يحصل على سلسلة التنسيق. |
|
|  | [getSingleFormat()](#getSingleFormat--) | يحصل على سلسلة التنسيق المفردة. |
|
|  | [toString()](#toString--) | يرجع سلسلة تمثل عنصر DateFormatElement الحالي. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | يحصل على عنصر يوم الشهر، الممثَّل برقم أو رقمين. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | يحصل على عنصر يوم الشهر، الممثَّل برقمين. |
|
|  | [getMonth()](#getMonth--) | يحصل على عنصر الشهر، الممثَّل برقم أو رقمين. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | يحصل على عنصر الشهر، الممثَّل برقمين. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | يحصل على عنصر الشهر، الممثَّل باسم مختصر. |
|
|  | [getMonthFullName()](#getMonthFullName--) | يحصل على عنصر الشهر، الممثَّل بالاسم الكامل. |
|
|  | [getYear()](#getYear--) | يحصل على عنصر السنة، الممثَّل برقم واحد أو رقمين أو ثلاثة أو أربعة أرقام. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | يحصل على عنصر السنة، الممثَّل برقمين. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | يحصل على عنصر السنة، الممثَّل بأربعة أرقام. |
|
|  | [getDateSeparator()](#getDateSeparator--) | يحصل على عنصر فاصل التاريخ. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


يحصل على سلسلة التنسيق.


**Returns:**
java.lang.String - سلسلة التنسيق.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


يحصل على سلسلة التنسيق المفردة.


**Returns:**
java.lang.String - سلسلة التنسيق المفردة.

### toString() {#toString--}
```
public abstract String toString()
```


يرجع سلسلة تمثل عنصر DateFormatElement الحالي.


**Returns:**
java.lang.String - سلسلة تمثل عنصر DateFormatElement الحالي.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


يحصل على عنصر يوم الشهر، الممثَّل برقم أو رقمين.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


يحصل على عنصر يوم الشهر، الممثَّل برقمين.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


يحصل على عنصر الشهر، الممثَّل برقم أو رقمين.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


يحصل على عنصر الشهر، الممثَّل برقمين.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


يحصل على عنصر الشهر، الممثَّل باسم مختصر.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


يحصل على عنصر الشهر، الممثَّل بالاسم الكامل.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


يحصل على عنصر السنة، الممثَّل برقم واحد أو رقمين أو ثلاثة أو أربعة أرقام.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


يحصل على عنصر السنة، الممثَّل برقمين.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


يحصل على عنصر السنة، الممثَّل بأربعة أرقام.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


يحصل على عنصر فاصل التاريخ.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

