---
title: IndexStatus
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Specifica uno stato di indice.
type: docs
weight: 230
url: /it/net/groupdocs.search.common/indexstatus/
---
## IndexStatus enumeration

Specifica uno stato di indice.

```csharp
public enum IndexStatus
```

### I valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Ready | `0` | Index è gratuito e pronto a cambiare. |
| Failed | `1` | L'indice deve essere ricaricato a causa di un errore. |
| Indexing | `2` | Index esegue un'operazione di indicizzazione. |
| Updating | `3` | L'indice esegue un'operazione di aggiornamento. |
| Merging | `4` | L'indice esegue un'operazione di unione. |
| Optimizing | `5` | Index esegue un'operazione di ottimizzazione. |
| Deleting | `6` | L'indice esegue un'operazione di eliminazione. |
| Renaming | `7` | Index esegue un'operazione di ridenominazione. |
| ChangingAttributes | `8` | L'indice modifica gli attributi. |

### Guarda anche

* spazio dei nomi [GroupDocs.Search.Common](../../groupdocs.search.common)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->