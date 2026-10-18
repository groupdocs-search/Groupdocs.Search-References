---
title: "IndexStatus"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Spécifie l'état d'un index."
type: docs
weight: 240
url: /fr/net/groupdocs.search.common/indexstatus/
---
## IndexStatus enumeration

Spécifie l'état d'un index.

```csharp
public enum IndexStatus
```

### Values

| Nom | Value | Description |
| --- | --- | --- |
| Ready | `0` | L'index est libre et prêt pour les modifications. |
| Failed | `1` | L'index doit être rechargé en raison d'une erreur. |
| Indexing | `2` | L'index effectue une opération d'indexation. |
| Updating | `3` | L'index effectue une opération de mise à jour. |
| Merging | `4` | L'index effectue une opération de fusion. |
| Optimizing | `5` | L'index effectue une opération d'optimisation. |
| Deleting | `6` | L'index effectue une opération de suppression. |
| Renaming | `7` | L'index effectue une opération de renommage. |
| ChangingAttributes | `8` | L'index modifie les attributs. |
| CheckingSegments | `9` | L'index vérifie les segments. |
| SavingTheIndex | `10` | L'index est enregistré dans un autre dossier. |

### Voir aussi

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
