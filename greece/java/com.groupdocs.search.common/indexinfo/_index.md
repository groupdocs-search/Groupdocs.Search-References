---
title: "IndexInfo"
second_title: "GroupDocs.Search για Java API Reference"
description: "Περιέχει βασικές πληροφορίες για ένα Ευρετήριο."
type: docs
weight: 24
url: /el/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Περιέχει βασικές πληροφορίες για ένα Ευρετήριο.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Λαμβάνει το μοναδικό αναγνωριστικό του ευρετηρίου. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Λαμβάνει το πλήρες όνομα φακέλου όπου βρίσκεται το ευρετήριο. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Λαμβάνει την κατάσταση του ευρετηρίου. |
|
|  | [getVersion()](#getVersion--) | Λαμβάνει την έκδοση του ευρετηρίου. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Λαμβάνει τον αριθμό των τμημάτων του ευρετηρίου. |
|
|  | [getTermCount()](#getTermCount--) | Λαμβάνει τον αριθμό των λέξεων στο ευρετήριο. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Λαμβάνει το μοναδικό αναγνωριστικό του ευρετηρίου.


**Returns:**
java.util.UUID - Το μοναδικό αναγνωριστικό του ευρετηρίου.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Λαμβάνει το πλήρες όνομα φακέλου όπου βρίσκεται το ευρετήριο.


**Returns:**
java.lang.String - Το πλήρες όνομα φακέλου όπου βρίσκεται το ευρετήριο.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Λαμβάνει την κατάσταση του ευρετηρίου.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Λαμβάνει την έκδοση του ευρετηρίου.


**Returns:**
java.lang.String - Η έκδοση του ευρετηρίου.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Λαμβάνει τον αριθμό των τμημάτων του ευρετηρίου.


**Returns:**
int - Ο αριθμός των τμημάτων του ευρετηρίου.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Λαμβάνει τον αριθμό των λέξεων στο ευρετήριο.


**Returns:**
int - Ο αριθμός των λέξεων στο ευρετήριο.

