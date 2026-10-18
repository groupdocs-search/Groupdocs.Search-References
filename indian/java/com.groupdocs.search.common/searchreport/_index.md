---
title: "SearchReport"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज ऑपरेशन पर विस्तृत जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 30
url: /hi/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

खोज ऑपरेशन पर विस्तृत जानकारी का प्रतिनिधित्व करता है।


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentsFolder);
// इंडेक्स में खोज
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// खोज रिपोर्ट प्राप्त करना
SearchReport[] reports = index.getSearchReports();
// रिपोर्ट को कंसोल पर प्रिंट कर रहा है
for (SearchReport report : reports) {
System.out.println("क्वेरी: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat(\"MM/dd/yyyy HH:mm:ss\");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("अवधि: " + report.getSearchDuration());
System.out.println("दस्तावेज़: " + report.getDocumentCount());
System.out.println("घटनाएँ: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | खोज की प्रारंभिक समय प्राप्त करता है। |
|
|  | [getEndTime()](#getEndTime--) | खोज का समाप्ति समय प्राप्त करता है। |
|
|  | [getSearchDuration()](#getSearchDuration--) | खोज की अवधि सेकंड में प्राप्त करता है। |
|
|  | [getDocumentCount()](#getDocumentCount--) | पाए गए दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | पाए गए कुल घटनाओं की संख्या प्राप्त करता है। |
|
|  | [getTextQuery()](#getTextQuery--) | खोज क्वेरी को टेक्स्ट रूप में प्राप्त करता है। |
|
|  | [getObjectQuery()](#getObjectQuery--) | खोज क्वेरी को ऑब्जेक्ट रूप में प्राप्त करता है। |
|
|  | [getSearchOptions()](#getSearchOptions--) | खोज विकल्प प्राप्त करता है। |
|
|  | [toString()](#toString--) | वर्तमान SearchReport को दर्शाने वाली स्ट्रिंग लौटाता है। |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


खोज की प्रारंभिक समय प्राप्त करता है।


**Returns:**
java.util.Date - खोज की प्रारंभिक समय।

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


खोज का समाप्ति समय प्राप्त करता है।


**Returns:**
java.util.Date - खोज का समाप्ति समय।

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


खोज की अवधि सेकंड में प्राप्त करता है।


**Returns:**
double - खोज की अवधि सेकंड में।

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


पाए गए दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - पाए गए दस्तावेज़ों की संख्या।

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


पाए गए कुल घटनाओं की संख्या प्राप्त करता है।


**Returns:**
int - पाए गए कुल घटनाओं की संख्या।

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


खोज क्वेरी को टेक्स्ट रूप में प्राप्त करता है।


**Returns:**
java.lang.String - पाठ रूप में खोज क्वेरी।

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


खोज क्वेरी को ऑब्जेक्ट रूप में प्राप्त करता है।


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


खोज विकल्प प्राप्त करता है।


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


वर्तमान SearchReport को दर्शाने वाली स्ट्रिंग लौटाता है।


**Returns:**
java.lang.String - वर्तमान SearchReport को दर्शाने वाली स्ट्रिंग।

