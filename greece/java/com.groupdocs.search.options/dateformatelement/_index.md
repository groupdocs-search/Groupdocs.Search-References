---
title: "DateFormatElement"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά ένα στοιχείο μορφής ημερομηνίας."
type: docs
weight: 15
url: /el/java/com.groupdocs.search.options/dateformatelement/
---
**Inheritance:**
java.lang.Object
```
public abstract class DateFormatElement
```

Αναπαριστά ένα στοιχείο μορφής ημερομηνίας.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DateFormatElement()](#DateFormatElement--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFormat()](#getFormat--) | Λαμβάνει τη συμβολοσειρά μορφής. |
|
|  | [getSingleFormat()](#getSingleFormat--) | Λαμβάνει τη μοναδική συμβολοσειρά μορφής. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον DateFormatElement. |
|
|  | [getDayOfMonth()](#getDayOfMonth--) | Λαμβάνει το στοιχείο ημέρας του μήνα, που αντιπροσωπεύεται από ένα ή δύο ψηφία. |
|
|  | [getDayOfMonthTwoDigits()](#getDayOfMonthTwoDigits--) | Λαμβάνει το στοιχείο ημέρας του μήνα, που αντιπροσωπεύεται από δύο ψηφία. |
|
|  | [getMonth()](#getMonth--) | Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από ένα ή δύο ψηφία. |
|
|  | [getMonthTwoDigits()](#getMonthTwoDigits--) | Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από δύο ψηφία. |
|
|  | [getMonthAbbreviatedName()](#getMonthAbbreviatedName--) | Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από συντομογραφημένο όνομα. |
|
|  | [getMonthFullName()](#getMonthFullName--) | Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από πλήρες όνομα. |
|
|  | [getYear()](#getYear--) | Λαμβάνει το στοιχείο έτους, που αντιπροσωπεύεται από ένα, δύο, τρία ή τέσσερα ψηφία. |
|
|  | [getYearTwoDigits()](#getYearTwoDigits--) | Λαμβάνει το στοιχείο έτους, που αντιπροσωπεύεται από δύο ψηφία. |
|
|  | [getYearFourDigits()](#getYearFourDigits--) | Λαμβάνει το στοιχείο έτους, που αντιπροσωπεύεται από τέσσερα ψηφία. |
|
|  | [getDateSeparator()](#getDateSeparator--) | Λαμβάνει το στοιχείο διαχωριστικού ημερομηνίας. |
|
### DateFormatElement() {#DateFormatElement--}
```
public DateFormatElement()
```


### getFormat() {#getFormat--}
```
public abstract String getFormat()
```


Λαμβάνει τη συμβολοσειρά μορφής.


**Returns:**
java.lang.String - Η συμβολοσειρά μορφής.

### getSingleFormat() {#getSingleFormat--}
```
public abstract String getSingleFormat()
```


Λαμβάνει τη μοναδική συμβολοσειρά μορφής.


**Returns:**
java.lang.String - Η μοναδική συμβολοσειρά μορφής.

### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον DateFormatElement.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει το τρέχον DateFormatElement.

### getDayOfMonth() {#getDayOfMonth--}
```
public static DateFormatElement getDayOfMonth()
```


Λαμβάνει το στοιχείο ημέρας του μήνα, που αντιπροσωπεύεται από ένα ή δύο ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by one or two digits.

### getDayOfMonthTwoDigits() {#getDayOfMonthTwoDigits--}
```
public static DateFormatElement getDayOfMonthTwoDigits()
```


Λαμβάνει το στοιχείο ημέρας του μήνα, που αντιπροσωπεύεται από δύο ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The day of month element, represented by two digits.

### getMonth() {#getMonth--}
```
public static DateFormatElement getMonth()
```


Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από ένα ή δύο ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by one or two digits.

### getMonthTwoDigits() {#getMonthTwoDigits--}
```
public static DateFormatElement getMonthTwoDigits()
```


Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από δύο ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by two digits.

### getMonthAbbreviatedName() {#getMonthAbbreviatedName--}
```
public static DateFormatElement getMonthAbbreviatedName()
```


Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από συντομογραφημένο όνομα.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by abbreviated name.

### getMonthFullName() {#getMonthFullName--}
```
public static DateFormatElement getMonthFullName()
```


Λαμβάνει το στοιχείο μήνα, που αντιπροσωπεύεται από πλήρες όνομα.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The month element, represented by full name.

### getYear() {#getYear--}
```
public static DateFormatElement getYear()
```


Λαμβάνει το στοιχείο έτους, που αντιπροσωπεύεται από ένα, δύο, τρία ή τέσσερα ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by one, two, three, or four digits.

### getYearTwoDigits() {#getYearTwoDigits--}
```
public static DateFormatElement getYearTwoDigits()
```


Λαμβάνει το στοιχείο έτους, που αντιπροσωπεύεται από δύο ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by two digits.

### getYearFourDigits() {#getYearFourDigits--}
```
public static DateFormatElement getYearFourDigits()
```


Λαμβάνει το στοιχείο έτους, που αντιπροσωπεύεται από τέσσερα ψηφία.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The year element, represented by four digits.

### getDateSeparator() {#getDateSeparator--}
```
public static DateFormatElement getDateSeparator()
```


Λαμβάνει το στοιχείο διαχωριστικού ημερομηνίας.


**Returns:**
[DateFormatElement](../../com.groupdocs.search.options/dateformatelement) - The date separator element.

