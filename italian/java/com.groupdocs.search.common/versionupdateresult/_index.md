---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il risultato di un'operazione di aggiornamento della versione dell'indice."
type: docs
weight: 42
url: /it/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Rappresenta il risultato di un'operazione di aggiornamento della versione dell'indice.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Updated](#Updated) | Versione dell'indice aggiornata. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | La versione dell'indice è già aggiornata. |
|
|  | [Unsupported](#Unsupported) | La versione dell'indice non è supportata o la directory non contiene dati di indice validi. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Versione dell'indice aggiornata.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


La versione dell'indice è già aggiornata.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


La versione dell'indice non è supportata o la directory non contiene dati di indice validi.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
