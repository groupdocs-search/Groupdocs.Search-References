---
title: "DateFormatElement"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt ein Datumsformatelement dar."
type: docs
weight: 15
url: /de/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Stellt ein Datumsformatelement dar.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFormat()](#getFormat--) | Gibt die Formatzeichenfolge zurück. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Gibt die einzelne Formatzeichenfolge zurück. |
|
|  | [toString()](#toString--) | Gibt einen String zurück, der das aktuelle  DateFormatElement  darstellt. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Gibt das Tag-des-Monats-Element zurück, dargestellt durch ein oder zwei Ziffern. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Gibt das Tag-des-Monats-Element zurück, dargestellt durch zwei Ziffern. |
|
|  | [getMonth()](#getMonth--) | Gibt das Monats-Element zurück, dargestellt durch ein oder zwei Ziffern. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Gibt das Monats-Element zurück, dargestellt durch zwei Ziffern. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Gibt das Monats-Element zurück, dargestellt durch einen abgekürzten Namen. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Gibt das Monats-Element zurück, dargestellt durch den vollen Namen. |
|
|  | [getYear()](#getYear--) | Gibt das Jahres-Element zurück, dargestellt durch ein, zwei, drei oder vier Ziffern. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Gibt das Jahres-Element zurück, dargestellt durch zwei Ziffern. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Gibt das Jahres-Element zurück, dargestellt durch vier Ziffern. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Gibt das Datums-Trennzeichen-Element zurück. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Gibt die Formatzeichenfolge zurück.


**Returns:**
java.lang.String - Die Formatzeichenfolge.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Gibt die einzelne Formatzeichenfolge zurück.


**Returns:**
java.lang.String - Der einzelne Format-String.

### toString() {#toString--}
```
public abstract String toString()
```


Gibt einen String zurück, der das aktuelle  DateFormatElement  darstellt.


**Returns:**
java.lang.String - Ein String, der das aktuelle DateFormatElement darstellt.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Gibt das Tag-des-Monats-Element zurück, dargestellt durch ein oder zwei Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Gibt das Tag-des-Monats-Element zurück, dargestellt durch zwei Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Gibt das Monats-Element zurück, dargestellt durch ein oder zwei Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Gibt das Monats-Element zurück, dargestellt durch zwei Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Gibt das Monats-Element zurück, dargestellt durch einen abgekürzten Namen.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Gibt das Monats-Element zurück, dargestellt durch den vollen Namen.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Gibt das Jahres-Element zurück, dargestellt durch ein, zwei, drei oder vier Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Gibt das Jahres-Element zurück, dargestellt durch zwei Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Gibt das Jahres-Element zurück, dargestellt durch vier Ziffern.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Gibt das Datums-Trennzeichen-Element zurück.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

