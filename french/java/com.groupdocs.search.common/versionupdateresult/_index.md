---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le résultat d'une opération de mise à jour de version d'index."
type: docs
weight: 42
url: /fr/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Représente le résultat d'une opération de mise à jour de version d'index.

## Fields

| Field | Description |
| --- | --- |
|  | [Updated](#Updated) | Version de l'index mise à jour. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | La version de l'index est déjà à jour. |
|
|  | [Unsupported](#Unsupported) | La version de l'index n'est pas prise en charge ou le répertoire ne contient pas de données d'index valides. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Version de l'index mise à jour.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


La version de l'index est déjà à jour.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


La version de l'index n'est pas prise en charge ou le répertoire ne contient pas de données d'index valides.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
