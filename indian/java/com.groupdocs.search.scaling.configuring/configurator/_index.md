---
title: "Configurator"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज नेटवर्क कॉन्फ़िगरेटर का प्रतिनिधित्व करता है।"
type: docs
weight: 11
url: /hi/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

खोज नेटवर्क कॉन्फ़िगरेटर का प्रतिनिधित्व करता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [Configurator()](#Configurator--) | Configurator क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है। |
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | खोज नेटवर्क में प्रत्येक शार्ड के लिए इंडेक्स सेटिंग्स को कॉन्फ़िगर करना शुरू करता है। |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | खोज नेटवर्क कॉन्फ़िगरेशन में एक नोड जोड़ता है। |
|
|  | [completeConfiguration()](#completeConfiguration--) | कॉन्फ़िगरेशन प्रक्रिया पूरी करता है और खोज नेटवर्क कॉन्फ़िगरेशन का एक इंस्टेंस रिटर्न करता है। |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Configurator क्लास का एक नया इंस्टेंस इनिशियलाइज़ करता है।


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


खोज नेटवर्क में प्रत्येक शार्ड के लिए इंडेक्स सेटिंग्स को कॉन्फ़िगर करना शुरू करता है।


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


खोज नेटवर्क कॉन्फ़िगरेशन में एक नोड जोड़ता है।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | nodeIndex | int | नोड इंडेक्स। |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


कॉन्फ़िगरेशन प्रक्रिया पूरी करता है और खोज नेटवर्क कॉन्फ़िगरेशन का एक इंस्टेंस रिटर्न करता है।


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
