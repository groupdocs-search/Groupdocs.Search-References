---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search for Java API Reference"
description: "एट्रिब्यूट परिवर्तनों के लिए एक कंटेनर का प्रतिनिधित्व करता है।"
type: docs
weight: 10
url: /hi/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

एट्रिब्यूट परिवर्तनों के लिए एक कंटेनर का प्रतिनिधित्व करता है।


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | एक नया उदाहरण प्रारंभ करता है  AttributeChangeBatch  क्लास का। |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | एक नया उदाहरण प्रारंभ करता है  AttributeChangeBatch  क्लास का। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ में जोड़ता है। |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ों में जोड़ता है। |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | निर्दिष्ट गुणों को अनुक्रम में सभी दस्तावेज़ों में जोड़ता है। |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ से हटाता है। |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ों से हटाता है। |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | सभी गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ से हटाता है। |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | सभी गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ों से हटाता है। |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | निर्दिष्ट गुणों को अनुक्रम में सभी दस्तावेज़ों से हटाता है। |
|
|  | [clear()](#clear--) | सभी गुणों को अनुक्रम में सभी दस्तावेज़ों से हटाता है। |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


एक नया उदाहरण प्रारंभ करता है  AttributeChangeBatch  क्लास का।


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


एक नया उदाहरण प्रारंभ करता है  AttributeChangeBatch  क्लास का।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | डेटा | java.lang.Object | सीरियलाइज़्ड डेटा। |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | दस्तावेज़ पथ। |
|
|  | गुण | java.lang.String[] | जोड़ने के लिए गुण। |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ों में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पथ | java.lang.String[] | दस्तावेज़ पथ। |
|
|  | गुण | java.lang.String[] | जोड़ने के लिए गुण। |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


निर्दिष्ट गुणों को अनुक्रम में सभी दस्तावेज़ों में जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | गुण | java.lang.String[] | जोड़ने के लिए गुण। |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | दस्तावेज़ पथ। |
|
|  | गुण | java.lang.String[] | हटाने के लिए गुण। |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


निर्दिष्ट गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ों से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पथ | java.lang.String[] | दस्तावेज़ पथ। |
|
|  | गुण | java.lang.String[] | हटाने के लिए गुण। |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


सभी गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | path | java.lang.String | दस्तावेज़ पथ। |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


सभी गुणों को निर्दिष्ट अनुक्रमित दस्तावेज़ों से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | पथ | java.lang.String[] | दस्तावेज़ पथ। |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


निर्दिष्ट गुणों को अनुक्रम में सभी दस्तावेज़ों से हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | गुण | java.lang.String[] | हटाने के लिए गुण। |
|

### clear() {#clear--}
```
public void clear()
```


सभी गुणों को अनुक्रम में सभी दस्तावेज़ों से हटाता है।


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
