---
title: IndexStatus
second_title: GroupDocs.Search efter .NET API Reference
description: Anger en indexstatus.
type: docs
weight: 230
url: /sv/net/groupdocs.search.common/indexstatus/
---
## IndexStatus enumeration

Anger en indexstatus.

```csharp
public enum IndexStatus
```

### Värderingar

| namn | Värde | Beskrivning |
| --- | --- | --- |
| Ready | `0` | Index är gratis och redo att ändras. |
| Failed | `1` | Index måste laddas om på grund av ett fel. |
| Indexing | `2` | Index utför en indexeringsoperation. |
| Updating | `3` | Index utför en uppdateringsåtgärd. |
| Merging | `4` | Index utför en sammanslagning. |
| Optimizing | `5` | Index utför en optimeringsoperation. |
| Deleting | `6` | Index utför en raderingsoperation. |
| Renaming | `7` | Index utför en byte av namn. |
| ChangingAttributes | `8` | Index ändrar attribut. |

### Se även

* namnutrymme [GroupDocs.Search.Common](../../groupdocs.search.common)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->