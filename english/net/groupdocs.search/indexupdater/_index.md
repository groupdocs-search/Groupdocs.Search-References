---
title: IndexUpdater
second_title: GroupDocs.Search for .NET API Reference
description: Represents an index updater. This class performs reindexing documents in an index of an old version.
type: docs
weight: 610
url: /net/groupdocs.search/indexupdater/
---
## IndexUpdater class

Represents an index updater. This class performs reindexing documents in an index of an old version.

```csharp
public class IndexUpdater
```

## Constructors

| Name | Description |
| --- | --- |
| [IndexUpdater](indexupdater)() | Initializes a new instance of the [`IndexUpdater`](../indexupdater) class. |

## Methods

| Name | Description |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | Checks whether an index in the specified directory can be updated to the latest version. |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | Checks whether the specified directory contains an index of the latest version. |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | Performs reindexing documents in an index of an old version. The updated index will be placed in the *newIndexPath* directory. The index in the *indexPath* directory will not be changed. |

### Remarks

**Learn more**

* [Update index](https://docs.groupdocs.com/display/searchnet/Update+index)

### Examples

The example demonstrates a typical usage of the class.

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### See Also

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->