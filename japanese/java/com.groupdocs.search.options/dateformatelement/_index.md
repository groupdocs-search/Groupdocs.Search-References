---
title: "DateFormatElement"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "日付形式要素を表します。"
type: docs
weight: 15
url: /ja/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

日付形式要素を表します。


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFormat()](#getFormat--) | フォーマット文字列を取得します。 |
|
|  | [getSingleFormat()](#getSingleFormat--) | 単一のフォーマット文字列を取得します。 |
|
|  | [toString()](#toString--) | 現在の DateFormatElement を表す文字列を返します。 |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | 1桁または2桁で表される月の日要素を取得します。 |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | 2桁で表される月の日要素を取得します。 |
|
|  | [getMonth()](#getMonth--) | 1桁または2桁で表される月要素を取得します。 |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | 2桁で表される月要素を取得します。 |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | 省略形の名前で表される月要素を取得します。 |
|
|  | [getMonthFullName()](#getMonthFullName--) | 完全な名前で表される月要素を取得します。 |
|
|  | [getYear()](#getYear--) | 1桁、2桁、3桁、または4桁で表される年要素を取得します。 |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | 2桁で表される年要素を取得します。 |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | 4桁で表される年要素を取得します。 |
|
|  | [getDateSeparator()](#getDateSeparator--) | 日付区切り文字要素を取得します。 |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


フォーマット文字列を取得します。


**Returns:**
java.lang.String - フォーマット文字列。

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


単一のフォーマット文字列を取得します。


**Returns:**
java.lang.String - 単一のフォーマット文字列。

### toString() {#toString--}
```
public abstract String toString()
```


現在の DateFormatElement を表す文字列を返します。


**Returns:**
java.lang.String - 現在の DateFormatElement を表す文字列。

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


1桁または2桁で表される月の日要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


2桁で表される月の日要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


1桁または2桁で表される月要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


2桁で表される月要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


省略形の名前で表される月要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


完全な名前で表される月要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


1桁、2桁、3桁、または4桁で表される年要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


2桁で表される年要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


4桁で表される年要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


日付区切り文字要素を取得します。


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

