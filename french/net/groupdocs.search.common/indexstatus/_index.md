---
title: IndexStatus
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Spécifie un état dindex.
type: docs
weight: 230
url: /fr/net/groupdocs.search.common/indexstatus/
---
## IndexStatus enumeration

Spécifie un état d'index.

```csharp
public enum IndexStatus
```

### Valeurs

| Nom | Évaluer | La description |
| --- | --- | --- |
| Ready | `0` | L'index est gratuit et prêt à être modifié. |
| Failed | `1` | L'index doit être rechargé en raison d'une erreur. |
| Indexing | `2` | Index effectue une opération d'indexation. |
| Updating | `3` | Index effectue une opération de mise à jour. |
| Merging | `4` | Index effectue une opération de fusion. |
| Optimizing | `5` | Index effectue une opération d'optimisation. |
| Deleting | `6` | Index effectue une opération de suppression. |
| Renaming | `7` | Index effectue une opération de changement de nom. |
| ChangingAttributes | `8` | L'index modifie les attributs. |

### Voir également

* espace de noms [GroupDocs.Search.Common](../../groupdocs.search.common)
* Assemblée [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->