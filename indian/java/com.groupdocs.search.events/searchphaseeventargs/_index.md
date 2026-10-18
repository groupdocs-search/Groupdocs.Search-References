---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search for Java API Reference"
description: "खोज चरण परिवर्तन घटनाओं के लिए तर्क दर्शाता है।"
type: docs
weight: 21
url: /hi/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

खोज चरण परिवर्तन घटनाओं के लिए तर्क दर्शाता है।


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | खोज चरण को प्राप्त करता है। |
|
|  | [getQuery()](#getQuery--) | वर्तमान खोज की प्रारंभिक क्वेरी को प्राप्त करता है। |
|
|  | [getWords()](#getWords--) | वर्तमान चरण में प्राप्त शब्दों को प्राप्त करता है। |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


खोज चरण को प्राप्त करता है।


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


वर्तमान खोज की प्रारंभिक क्वेरी को प्राप्त करता है।


**Returns:**
java.lang.String - वर्तमान खोज की प्रारंभिक क्वेरी।

### getWords() {#getWords--}
```
public final String[] getWords()
```


वर्तमान चरण में प्राप्त शब्दों को प्राप्त करता है।


**Returns:**
java.lang.String[] - वर्तमान चरण में प्राप्त शब्द।

