---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar resultatet av en operation för uppdatering av indexversion."
type: docs
weight: 42
url: /sv/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Representerar resultatet av en operation för uppdatering av indexversion.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Updated](#Updated) | Index version uppdaterad. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Indexversionen är redan uppdaterad. |
|
|  | [Unsupported](#Unsupported) | Indexversionen stöds inte eller så innehåller katalogen inte giltig indexdata. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Index version uppdaterad.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Indexversionen är redan uppdaterad.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Indexversionen stöds inte eller så innehåller katalogen inte giltig indexdata.


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
