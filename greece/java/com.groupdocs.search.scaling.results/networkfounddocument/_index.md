---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα βρεθέν έγγραφο στο δίκτυο αναζήτησης."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

Αντιπροσωπεύει ένα βρεθέν έγγραφο στο δίκτυο αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | Λαμβάνει το ευρεθέν έγγραφο. |
|
|  | [getShardIndex()](#getShardIndex--) | Λαμβάνει τον δείκτη του τμήματος. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


Λαμβάνει το ευρεθέν έγγραφο.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


Λαμβάνει τον δείκτη του τμήματος.


**Returns:**
int - Ο δείκτης του τμήματος.

