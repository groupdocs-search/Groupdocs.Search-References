---
title: "SearchResult"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक खोज क्वेरी से मेल खाने वाले सर्च परिणाम का प्रतिनिधित्व करता है।"
type: docs
weight: 19
url: /hi/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

एक खोज क्वेरी से मेल खाने वाले सर्च परिणाम का प्रतिनिधित्व करता है।


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


उदाहरण क्लास के सामान्य उपयोग को दर्शाता है।

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// एक सूचकांक बना रहा है
Index index = new Index(indexFolder);
// निर्दिष्ट फ़ोल्डर से दस्तावेज़ों को इंडेक्स कर रहा है
index.add(documentFolder);
// खोज विकल्प सेट कर रहा है
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // फज़ी खोज को सक्षम करना
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // अधिकतम अंतर की संख्या को 3 पर सेट कर रहा है
// उन दस्तावेज़ों को खोजें जिनमें शब्द 'Einstein' या वाक्यांश 'Theory of Relativity' हो
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// परिणाम प्रिंट कर रहा है
System.out.println("Documents: " + result.getDocumentCount());
System.out.println("Total occurrences: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocument: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOccurrences: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tField: " + field.getFieldName());
System.out.println("\t\tOccurrences: " + document.getOccurrenceCount());
// पाए गए शब्दों को प्रिंट कर रहा है
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// पाए गए वाक्यांशों को प्रिंट कर रहा है
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | पाए गए दस्तावेज़ों की संख्या प्राप्त करता है। |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | पाए गए कुल घटनाओं की संख्या प्राप्त करता है। |
|
|  | [getTruncated()](#getTruncated--) | परिणाम के कटे हुए होने को दर्शाने वाला मान प्राप्त करता है। |
|
|  | [getWarnings()](#getWarnings--) | परिणाम का वर्णन करने वाली चेतावनी प्राप्त करता है। |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | अगले भाग की खोज के लिए एक चंक सर्च टोकन प्राप्त करता है। |
|
|  | [getStartTime()](#getStartTime--) | खोज की प्रारंभिक समय प्राप्त करता है। |
|
|  | [getEndTime()](#getEndTime--) | खोज का समाप्ति समय प्राप्त करता है। |
|
|  | [getSearchDuration()](#getSearchDuration--) | खोज की अवधि सेकंड में प्राप्त करता है। |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | सूचकांक द्वारा पाए गए दस्तावेज़ को प्राप्त करता है। |
|
|  | [iterator()](#iterator--) | पाए गए दस्तावेज़ों के संग्रह के माध्यम से इटरेट करने वाला इटरेटर लौटाता है। |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


परिणाम के कटे हुए होने को दर्शाने वाला मान प्राप्त करता है।


**Returns:**
boolean - परिणाम के कटे हुए होने को दर्शाने वाला मान।

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


परिणाम का वर्णन करने वाली चेतावनी प्राप्त करता है।


**Returns:**
java.lang.String - परिणाम का वर्णन करने वाली चेतावनी।

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


अगले भाग की खोज के लिए एक चंक सर्च टोकन प्राप्त करता है।


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


सूचकांक द्वारा पाए गए दस्तावेज़ को प्राप्त करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | इंडेक्स | int | पाए गए दस्तावेज़ का सूचकांक। |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


पाए गए दस्तावेज़ों के संग्रह के माध्यम से इटरेट करने वाला इटरेटर लौटाता है।


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - एक इटररेटर जिसका उपयोग पाए गए दस्तावेज़ों के संग्रह के माध्यम से इटररेट करने के लिए किया जा सकता है।

