---
title: IndexUpdater
second_title: GroupDocs.Search for Java API Reference
description: Represents an index updater.
type: docs
weight: 21
url: /java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Represents an index updater. This class performs reindexing documents in an index of an old version.

**Learn more**

 *  [Update index][]

The example demonstrates a typical usage of the class.

```
String sourceIndexFolder = "c:\\MyOldIndex\\";
 String targetIndexFolder = "c:\\MyNewIndex\\";
 IndexUpdater updater = new IndexUpdater();
 if (updater.canUpdateVersion(sourceIndexFolder))
 {
     int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
 }
```


[Update index]: https://docs.groupdocs.com/display/searchjava/Update+index
## Constructors

| Constructor | Description |
| --- | --- |
| [IndexUpdater()](#IndexUpdater--) | Initializes a new instance of the  IndexUpdater  class. |
## Methods

| Method | Description |
| --- | --- |
| [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Checks whether the specified directory contains an index of the latest version. |
| [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Checks whether an index in the specified directory can be updated to the latest version. |
| [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Performs reindexing documents in an index of an old version. |
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Initializes a new instance of the  IndexUpdater  class.

### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Checks whether the specified directory contains an index of the latest version.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexPath | java.lang.String | The index directory path. |

**Returns:**
boolean -  true  if the specified directory contains an index of the latest version; otherwise  false .
### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Checks whether an index in the specified directory can be updated to the latest version.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexPath | java.lang.String | The index directory path. |

**Returns:**
boolean -  true  if an index in the specified directory can be updated to the latest version; otherwise  false .
### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Performs reindexing documents in an index of an old version. The updated index will be placed in the  newIndexPath  directory. The index in the  indexPath  directory will not be changed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexPath | java.lang.String | The index directory path. |
| newIndexPath | java.lang.String | The directory for the updated index. |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.
