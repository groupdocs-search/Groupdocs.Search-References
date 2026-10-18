---
title: "IndexInfo"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Enthält grundlegende Informationen zu einem Index."
type: docs
weight: 24
url: /de/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Enthält grundlegende Informationen zu einem Index.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Liefert die eindeutige Kennung des Index. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Liefert den vollständigen Ordnernamen, in dem sich der Index befindet. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Ermittelt den Indexstatus. |
|
|  | [getVersion()](#getVersion--) | Liefert die Indexversion. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Liefert die Anzahl der Indexsegmente. |
|
|  | [getTermCount()](#getTermCount--) | Liefert die Anzahl der Wörter im Index. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Liefert die eindeutige Kennung des Index.


**Returns:**
java.util.UUID - Die eindeutige Kennung des Index.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Liefert den vollständigen Ordnernamen, in dem sich der Index befindet.


**Returns:**
java.lang.String - Der vollständige Ordnername, in dem sich der Index befindet.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Ermittelt den Indexstatus.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Liefert die Indexversion.


**Returns:**
java.lang.String - Die Indexversion.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Liefert die Anzahl der Indexsegmente.


**Returns:**
int - Die Anzahl der Indexsegmente.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Liefert die Anzahl der Wörter im Index.


**Returns:**
int - Die Anzahl der Wörter im Index.

