---
title: "DateFormatElement"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili elemen format tanggal."
type: docs
weight: 15
url: /id/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Mewakili elemen format tanggal.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getFormat()](#getFormat--) | Mendapatkan string format. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Mendapatkan string format tunggal. |
|
|  | [toString()](#toString--) | Mengembalikan String yang mewakili  DateFormatElement  saat ini. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Mendapatkan elemen hari dalam bulan, yang direpresentasikan dengan satu atau dua digit. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Mendapatkan elemen hari dalam bulan, yang direpresentasikan dengan dua digit. |
|
|  | [getMonth()](#getMonth--) | Mendapatkan elemen bulan, yang direpresentasikan dengan satu atau dua digit. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Mendapatkan elemen bulan, yang direpresentasikan dengan dua digit. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Mendapatkan elemen bulan, yang direpresentasikan dengan nama singkat. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Mendapatkan elemen bulan, yang direpresentasikan dengan nama lengkap. |
|
|  | [getYear()](#getYear--) | Mendapatkan elemen tahun, yang direpresentasikan dengan satu, dua, tiga, atau empat digit. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Mendapatkan elemen tahun, yang direpresentasikan dengan dua digit. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Mendapatkan elemen tahun, yang direpresentasikan dengan empat digit. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Mendapatkan elemen pemisah tanggal. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Mendapatkan string format.


**Returns:**
java.lang.String - String format.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Mendapatkan string format tunggal.


**Returns:**
java.lang.String - String format tunggal.

### toString() {#toString--}
```
public abstract String toString()
```


Mengembalikan String yang mewakili  DateFormatElement  saat ini.


**Returns:**
java.lang.String - Sebuah String yang mewakili DateFormatElement saat ini.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Mendapatkan elemen hari dalam bulan, yang direpresentasikan dengan satu atau dua digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Mendapatkan elemen hari dalam bulan, yang direpresentasikan dengan dua digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Mendapatkan elemen bulan, yang direpresentasikan dengan satu atau dua digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Mendapatkan elemen bulan, yang direpresentasikan dengan dua digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Mendapatkan elemen bulan, yang direpresentasikan dengan nama singkat.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Mendapatkan elemen bulan, yang direpresentasikan dengan nama lengkap.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Mendapatkan elemen tahun, yang direpresentasikan dengan satu, dua, tiga, atau empat digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Mendapatkan elemen tahun, yang direpresentasikan dengan dua digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Mendapatkan elemen tahun, yang direpresentasikan dengan empat digit.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Mendapatkan elemen pemisah tanggal.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

