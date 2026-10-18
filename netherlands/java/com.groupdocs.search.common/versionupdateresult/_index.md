---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt het resultaat van een indexversie‑update‑operatie voor."
type: docs
weight: 42
url: /nl/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Stelt het resultaat van een indexversie‑update‑operatie voor.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Updated](#Updated) | Indexversie bijgewerkt. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | Indexversie is al up-to-date. |
|
|  | [Unsupported](#Unsupported) | Indexversie wordt niet ondersteund of de map bevat geen geldige indexgegevens. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Indexversie bijgewerkt.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Indexversie is al up-to-date.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Indexversie wordt niet ondersteund of de map bevat geen geldige indexgegevens.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
