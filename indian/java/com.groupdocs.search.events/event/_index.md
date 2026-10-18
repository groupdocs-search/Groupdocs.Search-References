---
title: "Event"
second_title: "GroupDocs.Search for Java API Reference"
description: "इवेंट्स की सदस्यता लेते समय इस क्लास को विरासत में लेने के लिए अभिप्रेत है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

इवेंट्स की सदस्यता लेते समय इस क्लास को विरासत में लेने के लिए अभिप्रेत है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Event()](#Event--) | Event क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [add(T delegate)](#add-T-) | इवेंट के लिए एक लिस्नर जोड़ता है। |
|
|  | [remove(T delegate)](#remove-T-) | इवेंट के लिए एक लिस्नर हटाता है। |
|
|  | [isEmpty()](#isEmpty--) | कम से कम एक लिस्नर की मौजूदगी की जाँच करता है। |
|
### Event() {#Event--}
```
public Event()
```


Event क्लास की नई इंस्टेंस को इनिशियलाइज़ करता है।


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


इवेंट के लिए एक लिस्नर जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | delegate | T | इवेंट के लिए जोड़ने हेतु एक लिस्नर। |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


इवेंट के लिए एक लिस्नर हटाता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | delegate | T | इवेंट के लिए हटाने हेतु एक लिस्नर। |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


कम से कम एक लिस्नर की मौजूदगी की जाँच करता है।


**Returns:**
boolean - एक मान जो दर्शाता है कि इवेंट के लिए कम से कम एक लिस्नर जोड़ा गया है।

