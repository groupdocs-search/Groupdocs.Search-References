---
title: "SearchPhaseEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για τα γεγονότα αλλαγής φάσης αναζήτησης."
type: docs
weight: 21
url: /el/java/com.groupdocs.search.events/searchphaseeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class SearchPhaseEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για τα γεγονότα αλλαγής φάσης αναζήτησης.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getSearchPhase()](#getSearchPhase--) | Λαμβάνει τη φάση αναζήτησης. |
|
|  | [getQuery()](#getQuery--) | Λαμβάνει το αρχικό ερώτημα της τρέχουσας αναζήτησης. |
|
|  | [getWords()](#getWords--) | Λαμβάνει τις λέξεις που προέκυψαν στην τρέχουσα φάση. |
|
### getSearchPhase() {#getSearchPhase--}
```
public final SearchPhase getSearchPhase()
```


Λαμβάνει τη φάση αναζήτησης.


**Returns:**
[SearchPhase](../../com.groupdocs.search.events/searchphase) - The search phase.

### getQuery() {#getQuery--}
```
public final String getQuery()
```


Λαμβάνει το αρχικό ερώτημα της τρέχουσας αναζήτησης.


**Returns:**
java.lang.String - Το αρχικό ερώτημα της τρέχουσας αναζήτησης.

### getWords() {#getWords--}
```
public final String[] getWords()
```


Λαμβάνει τις λέξεις που προέκυψαν στην τρέχουσα φάση.


**Returns:**
java.lang.String[] - Οι λέξεις που προέκυψαν στην τρέχουσα φάση.

