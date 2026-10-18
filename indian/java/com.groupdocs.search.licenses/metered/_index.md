---
title: "Metered"
second_title: "GroupDocs.Search for Java API Reference"
description: 
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.licenses/metered/
---
**Inheritance:**
java.lang.Object
```
public class Metered
```
## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Metered()](#Metered--) | इस क्लास का नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [setMeteredKey(String publicKey, String privateKey)](#setMeteredKey-java.lang.String-java.lang.String-) | Metered कुंजियों के साथ उत्पाद को सक्रिय करता है। |
|
|  | [getConsumptionQuantity()](#getConsumptionQuantity--) | प्रोसेस किए गए MBs की मात्रा प्राप्त करता है। |
|
|  | [getConsumptionCredit()](#getConsumptionCredit--) | उपयोग किए गए क्रेडिट्स की गिनती प्राप्त करता है। |
|
| [increaseBytesCount(double length)](#increaseBytesCount-double-) |  |
| [increaseCreditsByBytesCount(double length)](#increaseCreditsByBytesCount-double-) |  |
| [increaseCreditsByOne()](#increaseCreditsByOne--) |  |
### Metered() {#Metered--}
```
public Metered()
```


इस क्लास का नया इंस्टेंस इनिशियलाइज़ करता है।


### setMeteredKey(String publicKey, String privateKey) {#setMeteredKey-java.lang.String-java.lang.String-}
```
public final void setMeteredKey(String publicKey, String privateKey)
```


Metered कुंजियों के साथ उत्पाद को सक्रिय करता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | publicKey | java.lang.String | सार्वजनिक कुंजी |
|
|  | privateKey | java.lang.String | निजी कुंजी |
|

### getConsumptionQuantity() {#getConsumptionQuantity--}
```
public static double getConsumptionQuantity()
```


प्रोसेस किए गए MBs की मात्रा प्राप्त करता है।


**Returns:**
double - उपभोग मात्रा

### getConsumptionCredit() {#getConsumptionCredit--}
```
public static double getConsumptionCredit()
```


उपयोग किए गए क्रेडिट्स की गिनती प्राप्त करता है।


**Returns:**
double - उपभोग क्रेडिट

### increaseBytesCount(double length) {#increaseBytesCount-double-}
```
public static void increaseBytesCount(double length)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| लंबाई | double |  |

### increaseCreditsByBytesCount(double length) {#increaseCreditsByBytesCount-double-}
```
public static void increaseCreditsByBytesCount(double length)
```




**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| लंबाई | double |  |

### increaseCreditsByOne() {#increaseCreditsByOne--}
```
public static void increaseCreditsByOne()
```




