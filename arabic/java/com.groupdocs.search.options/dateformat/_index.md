---
title: "DateFormat"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل تنسيق تاريخ."
type: docs
weight: 13
url: /ar/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

يمثل تنسيق تاريخ.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // إزالة تنسيقات التاريخ الافتراضية
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// إنشاء نمط تنسيق تاريخ 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // بحث في الفهرس
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | يُنشئ مثيلاً جديداً من الفئة DateFormat. |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | يُنشئ مثيلاً جديداً من الفئة DateFormat. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | يحصل على فاصل التاريخ. |
|
|  | [toString()](#toString--) | يعيد String تمثل تنسيق DateFormat الحالي. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


يُنشئ مثيلاً جديداً من الفئة DateFormat.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | cultureName | java.lang.String | اسم الثقافة. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | عناصر التنسيق. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


يُنشئ مثيلاً جديداً من الفئة DateFormat.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | عناصر التنسيق. |
|
|  | dateSeparator | java.lang.String | فاصل التاريخ. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


يحصل على فاصل التاريخ.


**Returns:**
java.lang.String - فاصل التاريخ.

### toString() {#toString--}
```
public String toString()
```


يعيد String تمثل تنسيق DateFormat الحالي.


**Returns:**
java.lang.String - String تمثل تنسيق DateFormat الحالي.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
