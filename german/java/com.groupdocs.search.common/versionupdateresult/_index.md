---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt das Ergebnis einer Indexversions-Aktualisierungsoperation dar."
type: docs
weight: 42
url: /de/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Stellt das Ergebnis einer Indexversions-Aktualisierungsoperation dar.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Updated](#Updated) | Index-Version aktualisiert. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Die Indexversion ist bereits aktuell. |
|
|  | [Unsupported](#Unsupported) | Die Indexversion wird nicht unterstützt oder das Verzeichnis enthält keine gültigen Indexdaten. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Index-Version aktualisiert.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Die Indexversion ist bereits aktuell.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Die Indexversion wird nicht unterstützt oder das Verzeichnis enthält keine gültigen Indexdaten.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
