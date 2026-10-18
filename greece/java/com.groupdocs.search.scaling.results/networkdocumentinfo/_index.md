---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν περιγραφέα για ένα ευρετηριασμένο έγγραφο στο δίκτυο αναζήτησης."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

Αντιπροσωπεύει έναν περιγραφέα για ένα ευρετηριασμένο έγγραφο στο δίκτυο αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Λαμβάνει τον περιγραφέα για ένα ευρετηριασμένο έγγραφο. |
|
|  | [getShardIndex()](#getShardIndex--) | Λαμβάνει τον δείκτη του τμήματος. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Λαμβάνει τον περιγραφέα για ένα ευρετηριασμένο έγγραφο.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Λαμβάνει τον δείκτη του τμήματος.


**Returns:**
int - Ο δείκτης του τμήματος.

