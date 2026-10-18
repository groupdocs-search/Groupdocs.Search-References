---
title: "DateFormat"
second_title: "GroupDocs.Search for Java API Reference"
description: "तारीख स्वरूप को दर्शाता है।"
type: docs
weight: 13
url: /hi/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

तारीख स्वरूप को दर्शाता है।


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // निर्दिष्ट फ़ोल्डर में एक इंडेक्स बना रहा है
index.add(documentsFolder); // निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स करना
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // डिफ़ॉल्ट तिथि स्वरूप हटाना
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// 'MM/dd/yyyy' पैटर्न बनाते हुए तिथि स्वरूप बनाना
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // इंडेक्स में खोजें
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | DateFormat क्लास की नई इंस्टेंस को प्रारंभ करता है। |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | DateFormat क्लास की नई इंस्टेंस को प्रारंभ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | तिथि विभाजक प्राप्त करता है। |
|
|  | [toString()](#toString--) | वर्तमान  DateFormat  का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है। |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


DateFormat क्लास की नई इंस्टेंस को प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | cultureName | java.lang.String | संस्कृति का नाम। |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | फ़ॉर्मेट तत्व। |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


DateFormat क्लास की नई इंस्टेंस को प्रारंभ करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | फ़ॉर्मेट तत्व। |
|
|  | dateSeparator | java.lang.String | तिथि विभाजक। |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


तिथि विभाजक प्राप्त करता है।


**Returns:**
java.lang.String - तिथि विभाजक।

### toString() {#toString--}
```
public String toString()
```


वर्तमान  DateFormat  का प्रतिनिधित्व करने वाली स्ट्रिंग लौटाता है।


**Returns:**
java.lang.String - वर्तमान  DateFormat  का प्रतिनिधित्व करने वाली स्ट्रिंग।

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
