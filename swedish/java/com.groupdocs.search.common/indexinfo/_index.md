---
title: "IndexInfo"
second_title: "GroupDocs.Search för Java API-referens"
description: "Innehåller grundläggande information om ett index."
type: docs
weight: 24
url: /sv/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Innehåller grundläggande information om ett index.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Hämtar indexets unika identifierare. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Hämtar det fullständiga mappnamnet där indexet är placerat. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Hämtar index‑statusen. |
|
|  | [getVersion()](#getVersion--) | Hämtar indexversionen. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Hämtar antalet indexsegment. |
|
|  | [getTermCount()](#getTermCount--) | Hämtar antalet ord i indexet. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Hämtar indexets unika identifierare.


**Returns:**
java.util.UUID - Indexets unika identifierare.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Hämtar det fullständiga mappnamnet där indexet är placerat.


**Returns:**
java.lang.String - Det fullständiga mappnamnet där indexet är placerat.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Hämtar index‑statusen.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Hämtar indexversionen.


**Returns:**
java.lang.String - Indexversionen.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Hämtar antalet indexsegment.


**Returns:**
int - Antalet indexsegment.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Hämtar antalet ord i indexet.


**Returns:**
int - Antalet ord i indexet.

