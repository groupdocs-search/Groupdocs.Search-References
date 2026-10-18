---
title: "DateFormatElement"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir tarih biçimi öğesini temsil eder."
type: docs
weight: 15
url: /tr/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Bir tarih biçimi öğesini temsil eder.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getFormat()](#getFormat--) | Biçim dizesini alır. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Tek biçim dizesini alır. |
|
|  | [toString()](#toString--) | Geçerli DateFormatElement öğesini temsil eden bir String döndürür. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Bir veya iki basamakla temsil edilen ay günü öğesini alır. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | İki basamakla temsil edilen ay günü öğesini alır. |
|
|  | [getMonth()](#getMonth--) | Bir veya iki basamakla temsil edilen ay öğesini alır. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | İki basamakla temsil edilen ay öğesini alır. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Kısaltılmış adla temsil edilen ay öğesini alır. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Tam adla temsil edilen ay öğesini alır. |
|
|  | [getYear()](#getYear--) | Bir, iki, üç veya dört basamakla temsil edilen yıl öğesini alır. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | İki basamakla temsil edilen yıl öğesini alır. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Dört basamakla temsil edilen yıl öğesini alır. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Tarih ayırıcı öğesini alır. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Biçim dizesini alır.


**Returns:**
java.lang.String - Biçim dizesi.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Tek biçim dizesini alır.


**Returns:**
java.lang.String - Tek biçim dizesi.

### toString() {#toString--}
```
public abstract String toString()
```


Geçerli DateFormatElement öğesini temsil eden bir String döndürür.


**Returns:**
java.lang.String - Geçerli DateFormatElement öğesini temsil eden bir String.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Bir veya iki basamakla temsil edilen ay günü öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


İki basamakla temsil edilen ay günü öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Bir veya iki basamakla temsil edilen ay öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


İki basamakla temsil edilen ay öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Kısaltılmış adla temsil edilen ay öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Tam adla temsil edilen ay öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Bir, iki, üç veya dört basamakla temsil edilen yıl öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


İki basamakla temsil edilen yıl öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Dört basamakla temsil edilen yıl öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Tarih ayırıcı öğesini alır.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

