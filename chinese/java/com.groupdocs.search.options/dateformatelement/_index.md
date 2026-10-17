---
title: "DateFormatElement"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示日期格式元素。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

表示日期格式元素。


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFormat()](#getFormat--) | 获取格式字符串。 |
|
|  | [getSingleFormat()](#getSingleFormat--) | 获取单个格式字符串。 |
|
|  | [toString()](#toString--) | 返回一个表示当前 DateFormatElement 的字符串。 |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | 获取月份天元素，以一位或两位数字表示。 |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | 获取月份天元素，以两位数字表示。 |
|
|  | [getMonth()](#getMonth--) | 获取月份元素，以一位或两位数字表示。 |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | 获取月份元素，以两位数字表示。 |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | 获取月份元素，以缩写名称表示。 |
|
|  | [getMonthFullName()](#getMonthFullName--) | 获取月份元素，以全称表示。 |
|
|  | [getYear()](#getYear--) | 获取年份元素，以一位、二位、三位或四位数字表示。 |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | 获取年份元素，以两位数字表示。 |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | 获取年份元素，以四位数字表示。 |
|
|  | [getDateSeparator()](#getDateSeparator--) | 获取日期分隔符元素。 |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


获取格式字符串。


**Returns:**
java.lang.String - 格式字符串。

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


获取单个格式字符串。


**Returns:**
java.lang.String - 单个格式字符串。

### toString() {#toString--}
```
public abstract String toString()
```


返回一个表示当前 DateFormatElement 的字符串。


**Returns:**
java.lang.String - 表示当前 DateFormatElement 的字符串。

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


获取月份天元素，以一位或两位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


获取月份天元素，以两位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


获取月份元素，以一位或两位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


获取月份元素，以两位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


获取月份元素，以缩写名称表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


获取月份元素，以全称表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


获取年份元素，以一位、二位、三位或四位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


获取年份元素，以两位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


获取年份元素，以四位数字表示。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


获取日期分隔符元素。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

