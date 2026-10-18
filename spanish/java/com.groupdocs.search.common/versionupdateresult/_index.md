---
title: "VersionUpdateResult"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el resultado de una operación de actualización de versión de índice."
type: docs
weight: 42
url: /es/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Representa el resultado de una operación de actualización de versión de índice.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Updated](#Updated) | Versión del índice actualizada. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | La versión del índice ya está actualizada. |
|
|  | [Unsupported](#Unsupported) | La versión del índice no es compatible o el directorio no contiene datos de índice válidos. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Versión del índice actualizada.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


La versión del índice ya está actualizada.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


La versión del índice no es compatible o el directorio no contiene datos de índice válidos.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
