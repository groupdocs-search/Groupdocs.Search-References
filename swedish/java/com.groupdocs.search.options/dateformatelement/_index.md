---
title: "DateFormatElement"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar ett datumformatselement."
type: docs
weight: 15
url: /sv/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Representerar ett datumformatselement.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFormat()](#getFormat--) | Hämtar formatsträngen. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Hämtar den enkla formatsträngen. |
|
|  | [toString()](#toString--) | Returnerar en String som representerar det aktuella DateFormatElement. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Hämtar dag-i-månad-elementet, representerat med en eller två siffror. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Hämtar dag-i-månad-elementet, representerat med två siffror. |
|
|  | [getMonth()](#getMonth--) | Hämtar månads-elementet, representerat med en eller två siffror. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Hämtar månads-elementet, representerat med två siffror. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Hämtar månads-elementet, representerat med förkortat namn. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Hämtar månads-elementet, representerat med fullt namn. |
|
|  | [getYear()](#getYear--) | Hämtar år-elementet, representerat med en, två, tre eller fyra siffror. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Hämtar år-elementet, representerat med två siffror. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Hämtar år-elementet, representerat med fyra siffror. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Hämtar datumseparator-elementet. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Hämtar formatsträngen.


**Returns:**
java.lang.String - Formatsträngen.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Hämtar den enkla formatsträngen.


**Returns:**
java.lang.String - Den enda formatsträngen.

### toString() {#toString--}
```
public abstract String toString()
```


Returnerar en String som representerar det aktuella DateFormatElement.


**Returns:**
java.lang.String - En sträng som representerar det aktuella  DateFormatElement .

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Hämtar dag-i-månad-elementet, representerat med en eller två siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Hämtar dag-i-månad-elementet, representerat med två siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Hämtar månads-elementet, representerat med en eller två siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Hämtar månads-elementet, representerat med två siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Hämtar månads-elementet, representerat med förkortat namn.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Hämtar månads-elementet, representerat med fullt namn.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Hämtar år-elementet, representerat med en, två, tre eller fyra siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Hämtar år-elementet, representerat med två siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Hämtar år-elementet, representerat med fyra siffror.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Hämtar datumseparator-elementet.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

