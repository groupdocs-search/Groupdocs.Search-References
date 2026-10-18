---
title: "IndexingReport"
second_title: "GroupDocs.Search for Java API Reference"
description: "इंडेक्सिंग ऑपरेशन पर विस्तृत जानकारी का प्रतिनिधित्व करता है।"
type: docs
weight: 25
url: /hi/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

इंडेक्सिंग ऑपरेशन पर विस्तृत जानकारी का प्रतिनिधित्व करता है।


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// निर्दिष्ट फ़ोल्डर में इंडेक्स बनाना
Index index = new Index(indexFolder);
// दस्तावेज़ों को इंडेक्स करना
index.add(documentsFolder1);
index.add(documentsFolder2);
// इंडेक्सिंग रिपोर्ट प्राप्त कर रहा है
IndexingReport[] reports = index.getIndexingReports();
// रिपोर्ट को कंसोल पर प्रिंट कर रहा है
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat(\"MM/dd/yyyy HH:mm:ss\");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | इंडेक्स में कुल दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | इंडेक्स में कुल शब्दों की संख्या प्राप्त करता है। |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | इंडेक्स किए गए दस्तावेज़ों की कुल लंबाई (MB) प्राप्त करता है। |
|
|  | [getSegmentCount()](#getSegmentCount--) | इंडेक्स खंडों की संख्या प्राप्त करता है। |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | कुल इंडेक्स आकार बाइट्स में प्राप्त करता है। |
|
|  | [getStartTime()](#getStartTime--) | इंडेक्सिंग शुरू होने का समय प्राप्त करता है। |
|
|  | [getEndTime()](#getEndTime--) | इंडेक्सिंग समाप्त होने का समय प्राप्त करता है। |
|
|  | [getIndexingTime()](#getIndexingTime--) | इंडेक्सिंग अवधि (सेकंड) प्राप्त करता है। |
|
|  | [getErrors()](#getErrors--) | त्रुटियों की सूची प्राप्त करता है। |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | इंडेक्स किए गए दस्तावेज़ों की सूची प्राप्त करता है। |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | अपडेटेड दस्तावेज़ों की सूची प्राप्त करता है। |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | इंडेक्स से हटाए गए दस्तावेज़ों की सूची प्राप्त करता है। |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


इंडेक्स में कुल दस्तावेज़ों की संख्या प्राप्त करता है।


**Returns:**
int - इंडेक्स में कुल दस्तावेज़ों की संख्या।

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


इंडेक्स में कुल शब्दों की संख्या प्राप्त करता है।


**Returns:**
int - इंडेक्स में कुल शब्दों की संख्या।

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


इंडेक्स किए गए दस्तावेज़ों की कुल लंबाई (MB) प्राप्त करता है।


**Returns:**
double - इंडेक्स किए गए दस्तावेज़ों की कुल लंबाई MB में।

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


इंडेक्स खंडों की संख्या प्राप्त करता है।


**Returns:**
int - इंडेक्स खंडों की संख्या।

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


कुल इंडेक्स आकार बाइट्स में प्राप्त करता है।


**Returns:**
long - कुल इंडेक्स आकार बाइट्स में।

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


इंडेक्सिंग शुरू होने का समय प्राप्त करता है।


**Returns:**
java.util.Date - इंडेक्सिंग शुरू होने का समय।

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


इंडेक्सिंग समाप्त होने का समय प्राप्त करता है।


**Returns:**
java.util.Date - इंडेक्सिंग समाप्त होने का समय।

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


इंडेक्सिंग अवधि (सेकंड) प्राप्त करता है।


**Returns:**
double - सेकंड में इंडेक्सिंग अवधि।

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


त्रुटियों की सूची प्राप्त करता है।


**Returns:**
java.lang.String[] - त्रुटियों की सूची।

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


इंडेक्स किए गए दस्तावेज़ों की सूची प्राप्त करता है।


**Returns:**
java.lang.String[] - इंडेक्स किए गए दस्तावेज़ों की सूची।

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


अपडेटेड दस्तावेज़ों की सूची प्राप्त करता है।


**Returns:**
java.lang.String[] - अपडेटेड दस्तावेज़ों की सूची।

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


इंडेक्स से हटाए गए दस्तावेज़ों की सूची प्राप्त करता है।


**Returns:**
java.lang.String[] - इंडेक्स से हटाए गए दस्तावेज़ों की सूची।

