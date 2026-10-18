---
title: "DateFormatElement"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un elemento de formato de fecha."
type: docs
weight: 15
url: /es/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Representa un elemento de formato de fecha.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFormat()](#getFormat--) | Obtiene la cadena de formato. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Obtiene la cadena de formato única. |
|
|  | [toString()](#toString--) | Devuelve una cadena que representa el DateFormatElement actual. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Obtiene el elemento del día del mes, representado por uno o dos dígitos. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Obtiene el elemento del día del mes, representado por dos dígitos. |
|
|  | [getMonth()](#getMonth--) | Obtiene el elemento del mes, representado por uno o dos dígitos. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Obtiene el elemento del mes, representado por dos dígitos. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Obtiene el elemento del mes, representado por nombre abreviado. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Obtiene el elemento del mes, representado por nombre completo. |
|
|  | [getYear()](#getYear--) | Obtiene el elemento del año, representado por uno, dos, tres o cuatro dígitos. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Obtiene el elemento del año, representado por dos dígitos. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Obtiene el elemento del año, representado por cuatro dígitos. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Obtiene el elemento separador de fecha. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Obtiene la cadena de formato.


**Returns:**
java.lang.String - La cadena de formato.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Obtiene la cadena de formato única.


**Returns:**
java.lang.String - La cadena de formato única.

### toString() {#toString--}
```
public abstract String toString()
```


Devuelve una cadena que representa el DateFormatElement actual.


**Returns:**
java.lang.String - Una cadena que representa el actual  DateFormatElement .

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Obtiene el elemento del día del mes, representado por uno o dos dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Obtiene el elemento del día del mes, representado por dos dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Obtiene el elemento del mes, representado por uno o dos dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Obtiene el elemento del mes, representado por dos dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Obtiene el elemento del mes, representado por nombre abreviado.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Obtiene el elemento del mes, representado por nombre completo.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Obtiene el elemento del año, representado por uno, dos, tres o cuatro dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Obtiene el elemento del año, representado por dos dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Obtiene el elemento del año, representado por cuatro dígitos.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Obtiene el elemento separador de fecha.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

