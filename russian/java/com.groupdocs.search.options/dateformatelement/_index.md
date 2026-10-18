---
title: "DateFormatElement"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет элемент формата даты."
type: docs
weight: 15
url: /ru/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Представляет элемент формата даты.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [getFormat()](#getFormat--) | Получает строку формата. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Получает одну строку формата. |
|
|  | [toString()](#toString--) | Возвращает строку, представляющую текущий  DateFormatElement . |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Получает элемент дня месяца, представленный одной или двумя цифрами. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Получает элемент дня месяца, представленный двумя цифрами. |
|
|  | [getMonth()](#getMonth--) | Получает элемент месяца, представленный одной или двумя цифрами. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Получает элемент месяца, представленный двумя цифрами. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Получает элемент месяца, представленный сокращённым названием. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Получает элемент месяца, представленный полным названием. |
|
|  | [getYear()](#getYear--) | Получает элемент года, представленный одной, двумя, тремя или четырьмя цифрами. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Получает элемент года, представленный двумя цифрами. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Получает элемент года, представленный четырьмя цифрами. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Получает элемент разделителя даты. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Получает строку формата.


**Returns:**
java.lang.String — строка формата.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Получает одну строку формата.


**Returns:**
java.lang.String - Одна строка формата.

### toString() {#toString--}
```
public abstract String toString()
```


Возвращает строку, представляющую текущий  DateFormatElement .


**Returns:**
java.lang.String - Строка, представляющая текущий DateFormatElement.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Получает элемент дня месяца, представленный одной или двумя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Получает элемент дня месяца, представленный двумя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Получает элемент месяца, представленный одной или двумя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Получает элемент месяца, представленный двумя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Получает элемент месяца, представленный сокращённым названием.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Получает элемент месяца, представленный полным названием.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Получает элемент года, представленный одной, двумя, тремя или четырьмя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Получает элемент года, представленный двумя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Получает элемент года, представленный четырьмя цифрами.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Получает элемент разделителя даты.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

