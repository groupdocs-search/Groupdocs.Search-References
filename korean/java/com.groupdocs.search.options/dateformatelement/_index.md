---
title: "DateFormatElement"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "날짜 형식 요소를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

날짜 형식 요소를 나타냅니다.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFormat()](#getFormat--) | 포맷 문자열을 가져옵니다. |
|
|  | [getSingleFormat()](#getSingleFormat--) | 단일 포맷 문자열을 가져옵니다. |
|
|  | [toString()](#toString--) | 현재 DateFormatElement를 나타내는 문자열을 반환합니다. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | 한 자리 또는 두 자리 숫자로 표시되는 일(day) 요소를 가져옵니다. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | 두 자리 숫자로 표시되는 일(day) 요소를 가져옵니다. |
|
|  | [getMonth()](#getMonth--) | 한 자리 또는 두 자리 숫자로 표시되는 월 요소를 가져옵니다. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | 두 자리 숫자로 표시되는 월 요소를 가져옵니다. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | 약어 형태의 이름으로 표시되는 월 요소를 가져옵니다. |
|
|  | [getMonthFullName()](#getMonthFullName--) | 전체 이름으로 표시되는 월 요소를 가져옵니다. |
|
|  | [getYear()](#getYear--) | 한 자리, 두 자리, 세 자리 또는 네 자리 숫자로 표시되는 연도 요소를 가져옵니다. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | 두 자리 숫자로 표시되는 연도 요소를 가져옵니다. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | 네 자리 숫자로 표시되는 연도 요소를 가져옵니다. |
|
|  | [getDateSeparator()](#getDateSeparator--) | 날짜 구분자 요소를 가져옵니다. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


포맷 문자열을 가져옵니다.


**Returns:**
java.lang.String - 포맷 문자열.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


단일 포맷 문자열을 가져옵니다.


**Returns:**
java.lang.String - 단일 형식 문자열.

### toString() {#toString--}
```
public abstract String toString()
```


현재 DateFormatElement를 나타내는 문자열을 반환합니다.


**Returns:**
java.lang.String - 현재  DateFormatElement 를 나타내는 문자열.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


한 자리 또는 두 자리 숫자로 표시되는 일(day) 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


두 자리 숫자로 표시되는 일(day) 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


한 자리 또는 두 자리 숫자로 표시되는 월 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


두 자리 숫자로 표시되는 월 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


약어 형태의 이름으로 표시되는 월 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


전체 이름으로 표시되는 월 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


한 자리, 두 자리, 세 자리 또는 네 자리 숫자로 표시되는 연도 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


두 자리 숫자로 표시되는 연도 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


네 자리 숫자로 표시되는 연도 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


날짜 구분자 요소를 가져옵니다.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

