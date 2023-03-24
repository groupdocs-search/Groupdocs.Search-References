---
title: DateFormat
second_title: GroupDocs.Search for Java API Reference
description: Represents a date format.
type: docs
weight: 12
url: /java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

Represents a date format.

**Learn more**

 *  [Date range search][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "daterange(2017-01-01 ~~ 2019-12-31)";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.getDateFormats().clear(); // Removing default date formats
 DateFormatElement[] elements = new DateFormatElement[] {
     DateFormatElement.getMonthTwoDigits(),
     DateFormatElement.getDateSeparator(),
     DateFormatElement.getDayOfMonthTwoDigits(),
     DateFormatElement.getDateSeparator(),
     DateFormatElement.getYearFourDigits(),
 };
 // Creating a date format pattern 'MM/dd/yyyy'
 com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
 options.getDateFormats().addItem(dateFormat);
 SearchResult result = index.search(query, options); // Search in index
 
```


[Date range search]: https://docs.groupdocs.com/display/searchjava/Date+range+search
## Constructors

| Constructor | Description |
| --- | --- |
| [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | Initializes a new instance of the  DateFormat  class. |
| [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | Initializes a new instance of the  DateFormat  class. |
## Methods

| Method | Description |
| --- | --- |
| [getDateSeparator()](#getDateSeparator--) | Gets the date separator. |
| [toString()](#toString--) | Returns a String that represents the current  DateFormat . |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


Initializes a new instance of the  DateFormat  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cultureName | java.lang.String | The culture name. |
| formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | The format elements. |

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


Initializes a new instance of the  DateFormat  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | The format elements. |
| dateSeparator | java.lang.String | The date separator. |

### getDateSeparator() {#getDateSeparator--}
```
public final String getDateSeparator()
```


Gets the date separator.

**Returns:**
java.lang.String - The date separator.
### toString() {#toString--}
```
public String toString()
```


Returns a String that represents the current  DateFormat .

**Returns:**
java.lang.String - A String that represents the current  DateFormat .
