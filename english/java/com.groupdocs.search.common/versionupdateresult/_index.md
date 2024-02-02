---
title: VersionUpdateResult
second_title: GroupDocs.Search for Java API Reference
description: Represents the result of an index version update operation.
type: docs
weight: 42
url: /java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

Represents the result of an index version update operation.
## Fields

| Field | Description |
| --- | --- |
| [Updated](#Updated) | Index version updated. |
| [AlreadyUpToDate](#AlreadyUpToDate) | Index version is already up-to-date. |
| [Unsupported](#Unsupported) | Index version is not supported or directory does not contain valid index data. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


Index version updated.

### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


Index version is already up-to-date.

### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


Index version is not supported or directory does not contain valid index data.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
