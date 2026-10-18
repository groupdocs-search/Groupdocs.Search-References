---
title: "DateFormatElement"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een datumformaat-element voor."
type: docs
weight: 15
url: /nl/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Stelt een datumformaat-element voor.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFormat()](#getFormat--) | Haalt de opmaakreeks op. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Haalt de enkele opmaakreeks op. |
|
|  | [toString()](#toString--) | Retourneert een String die het huidige DateFormatElement vertegenwoordigt. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Haalt het dag‑van‑maand‑element op, weergegeven door één of twee cijfers. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Haalt het dag‑van‑maand‑element op, weergegeven door twee cijfers. |
|
|  | [getMonth()](#getMonth--) | Haalt het maandelement op, weergegeven door één of twee cijfers. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Haalt het maandelement op, weergegeven door twee cijfers. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Haalt het maandelement op, weergegeven door een afgekorte naam. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Haalt het maandelement op, weergegeven door de volledige naam. |
|
|  | [getYear()](#getYear--) | Haalt het jaarelement op, weergegeven door één, twee, drie of vier cijfers. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Haalt het jaarelement op, weergegeven door twee cijfers. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Haalt het jaarelement op, weergegeven door vier cijfers. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Haalt het datum‑scheidingsteken‑element op. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Haalt de opmaakreeks op.


**Returns:**
java.lang.String - De opmaakreeks.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Haalt de enkele opmaakreeks op.


**Returns:**
java.lang.String - De enkele opmaakstring.

### toString() {#toString--}
```
public abstract String toString()
```


Retourneert een String die het huidige DateFormatElement vertegenwoordigt.


**Returns:**
java.lang.String - Een string die het huidige DateFormatElement vertegenwoordigt.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Haalt het dag‑van‑maand‑element op, weergegeven door één of twee cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Haalt het dag‑van‑maand‑element op, weergegeven door twee cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Haalt het maandelement op, weergegeven door één of twee cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Haalt het maandelement op, weergegeven door twee cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Haalt het maandelement op, weergegeven door een afgekorte naam.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Haalt het maandelement op, weergegeven door de volledige naam.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Haalt het jaarelement op, weergegeven door één, twee, drie of vier cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Haalt het jaarelement op, weergegeven door twee cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Haalt het jaarelement op, weergegeven door vier cijfers.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Haalt het datum‑scheidingsteken‑element op.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

