---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός που ενημερώνεται η πρόοδος της λειτουργίας ευρετηρίασης."
type: docs
weight: 19
url: /el/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός που ενημερώνεται η πρόοδος της λειτουργίας ευρετηρίασης.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Λαμβάνει τον συνολικό αριθμό τμημάτων για επεξεργασία. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Λαμβάνει τον αριθμό των επεξεργασμένων τμημάτων. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Λαμβάνει το ποσοστό της προόδου. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Λαμβάνει τον συνολικό αριθμό τμημάτων για επεξεργασία.


**Returns:**
int - Ο συνολικός αριθμός τμημάτων για επεξεργασία.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Λαμβάνει τον αριθμό των επεξεργασμένων τμημάτων.


**Returns:**
int - Ο αριθμός των επεξεργασμένων τμημάτων.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Λαμβάνει το ποσοστό της προόδου.


**Returns:**
double - Το ποσοστό της προόδου.

