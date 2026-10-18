---
title: "DateFormatElement"
second_title: "GroupDocs.Search for Java API Reference"
description: "तारीख स्वरूप तत्व को दर्शाता है।"
type: docs
weight: 15
url: /hi/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

तारीख स्वरूप तत्व को दर्शाता है।


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFormat()](#getFormat--) | फ़ॉर्मेट स्ट्रिंग प्राप्त करता है। |
|
|  | [getSingleFormat()](#getSingleFormat--) | एकल फ़ॉर्मेट स्ट्रिंग प्राप्त करता है। |
|
|  | [toString()](#toString--) | वर्तमान DateFormatElement को दर्शाने वाली स्ट्रिंग लौटाता है। |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | दिनांक तत्व प्राप्त करता है, जो एक या दो अंकों से दर्शाया जाता है। |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | दिनांक तत्व प्राप्त करता है, जो दो अंकों से दर्शाया जाता है। |
|
|  | [getMonth()](#getMonth--) | महीना तत्व प्राप्त करता है, जो एक या दो अंकों से दर्शाया जाता है। |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | महीना तत्व प्राप्त करता है, जो दो अंकों से दर्शाया जाता है। |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | महीना तत्व प्राप्त करता है, जो संक्षिप्त नाम से दर्शाया जाता है। |
|
|  | [getMonthFullName()](#getMonthFullName--) | महीना तत्व प्राप्त करता है, जो पूर्ण नाम से दर्शाया जाता है। |
|
|  | [getYear()](#getYear--) | वर्ष तत्व प्राप्त करता है, जो एक, दो, तीन या चार अंकों से दर्शाया जाता है। |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | वर्ष तत्व प्राप्त करता है, जो दो अंकों से दर्शाया जाता है। |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | वर्ष तत्व प्राप्त करता है, जो चार अंकों से दर्शाया जाता है। |
|
|  | [getDateSeparator()](#getDateSeparator--) | डेट सेपरेटर तत्व प्राप्त करता है। |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


फ़ॉर्मेट स्ट्रिंग प्राप्त करता है।


**Returns:**
java.lang.String - फ़ॉर्मेट स्ट्रिंग।

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


एकल फ़ॉर्मेट स्ट्रिंग प्राप्त करता है।


**Returns:**
java.lang.String - एकल फ़ॉर्मेट स्ट्रिंग।

### toString() {#toString--}
```
public abstract String toString()
```


वर्तमान DateFormatElement को दर्शाने वाली स्ट्रिंग लौटाता है।


**Returns:**
java.lang.String - वर्तमान DateFormatElement को दर्शाने वाली स्ट्रिंग।

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


दिनांक तत्व प्राप्त करता है, जो एक या दो अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


दिनांक तत्व प्राप्त करता है, जो दो अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


महीना तत्व प्राप्त करता है, जो एक या दो अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


महीना तत्व प्राप्त करता है, जो दो अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


महीना तत्व प्राप्त करता है, जो संक्षिप्त नाम से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


महीना तत्व प्राप्त करता है, जो पूर्ण नाम से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


वर्ष तत्व प्राप्त करता है, जो एक, दो, तीन या चार अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


वर्ष तत्व प्राप्त करता है, जो दो अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


वर्ष तत्व प्राप्त करता है, जो चार अंकों से दर्शाया जाता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


डेट सेपरेटर तत्व प्राप्त करता है।


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

