---
title: "FragmentContainer"
second_title: "GroupDocs.Search for Java API Reference"
description: "एक दस्तावेज़ फ़ील्ड के खोजे गए शब्दों को हाइलाइट किए हुए टेक्स्ट फ्रैगमेंट्स के लिए कंटेनर का प्रतिनिधित्व करता है।"
type: docs
weight: 22
url: /hi/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

एक दस्तावेज़ फ़ील्ड के खोजे गए शब्दों को हाइलाइट किए हुए टेक्स्ट फ्रैगमेंट्स के लिए कंटेनर का प्रतिनिधित्व करता है।


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## निर्माता

| निर्माता | विवरण |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | दस्तावेज़ फ़ील्ड का नाम प्राप्त करता है। |
|
|  | [getCount()](#getCount--) | शामिल टेक्स्ट फ्रैगमेंट्स की संख्या प्राप्त करता है। |
|
|  | [getFragments()](#getFragments--) | शामिल टेक्स्ट फ्रैगमेंट्स का एरे प्राप्त करता है। |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


दस्तावेज़ फ़ील्ड का नाम प्राप्त करता है।


**Returns:**
java.lang.String - दस्तावेज़ फ़ील्ड का नाम।

### getCount() {#getCount--}
```
public abstract int getCount()
```


शामिल टेक्स्ट फ्रैगमेंट्स की संख्या प्राप्त करता है।


**Returns:**
int - शामिल टेक्स्ट फ्रैगमेंट्स की संख्या।

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


शामिल टेक्स्ट फ्रैगमेंट्स का एरे प्राप्त करता है।


**Returns:**
java.lang.String[] - शामिल टेक्स्ट फ्रैगमेंट्स का एरे।

