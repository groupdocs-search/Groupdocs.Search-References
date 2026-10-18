---
title: "IndexInfo"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Bevat basisinformatie over een index."
type: docs
weight: 24
url: /nl/java/com.groupdocs.search.common/indexinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexInfo
```

Bevat basisinformatie over een Index.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [IndexInfo()](#IndexInfo--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getIndexId()](#getIndexId--) | Haalt de unieke identifier van de index op. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Haalt de volledige mapnaam op waar de index zich bevindt. |
|
|  | [getIndexStatus()](#getIndexStatus--) | Haalt de indexstatus op. |
|
|  | [getVersion()](#getVersion--) | Haalt de versie van de index op. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Haalt het aantal indexsegmenten op. |
|
|  | [getTermCount()](#getTermCount--) | Haalt het aantal woorden in de index op. |
|
### IndexInfo() {#IndexInfo--}
```
public IndexInfo()
```


### getIndexId() {#getIndexId--}
```
public abstract UUID getIndexId()
```


Haalt de unieke identifier van de index op.


**Returns:**
java.util.UUID - De unieke identifier van de index.

### getIndexFolder() {#getIndexFolder--}
```
public abstract String getIndexFolder()
```


Haalt de volledige mapnaam op waar de index zich bevindt.


**Returns:**
java.lang.String - De volledige mapnaam waar de index zich bevindt.

### getIndexStatus() {#getIndexStatus--}
```
public abstract IndexStatus getIndexStatus()
```


Haalt de indexstatus op.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

### getVersion() {#getVersion--}
```
public abstract String getVersion()
```


Haalt de versie van de index op.


**Returns:**
java.lang.String - De versie van de index.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Haalt het aantal indexsegmenten op.


**Returns:**
int - Het aantal indexsegmenten.

### getTermCount() {#getTermCount--}
```
public abstract int getTermCount()
```


Haalt het aantal woorden in de index op.


**Returns:**
int - Het aantal woorden in de index.

