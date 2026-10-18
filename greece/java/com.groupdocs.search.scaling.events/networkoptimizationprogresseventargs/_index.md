---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τα ορίσματα για το γεγονός αλλαγής προόδου της λειτουργίας βελτιστοποίησης."
type: docs
weight: 15
url: /el/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Αναπαριστά τα ορίσματα για το γεγονός αλλαγής προόδου της λειτουργίας βελτιστοποίησης.

## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Λαμβάνει τον δείκτη της υπηρεσίας κόμβου δικτύου αναζήτησης. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Λαμβάνει τον αριθμό των επεξεργασμένων τμημάτων. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Λαμβάνει τον συνολικό αριθμό τμημάτων για επεξεργασία. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Λαμβάνει το ποσοστό της προόδου. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης του κόμβου δικτύου αναζήτησης.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Λαμβάνει τον δείκτη της υπηρεσίας κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης της υπηρεσίας κόμβου δικτύου αναζήτησης.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Λαμβάνει τον αριθμό των επεξεργασμένων τμημάτων.


**Returns:**
int - Ο αριθμός των επεξεργασμένων τμημάτων.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Λαμβάνει τον συνολικό αριθμό τμημάτων για επεξεργασία.


**Returns:**
int - Ο συνολικός αριθμός τμημάτων για επεξεργασία.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Λαμβάνει το ποσοστό της προόδου.


**Returns:**
double - Το ποσοστό της προόδου.

