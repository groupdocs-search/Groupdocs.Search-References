---
title: "IndexStatus"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Specifica lo stato di un indice."
type: docs
weight: 240
url: /it/net/groupdocs.search.common/indexstatus/
---
## IndexStatus enumeration

Specifica lo stato di un indice.

```csharp
public enum IndexStatus
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Ready | `0` | L'indice è libero e pronto per le modifiche. |
| Failed | `1` | L'indice deve essere ricaricato a causa di un errore. |
| Indexing | `2` | L'indice esegue un'operazione di indicizzazione. |
| Updating | `3` | L'indice esegue un'operazione di aggiornamento. |
| Merging | `4` | L'indice esegue un'operazione di fusione. |
| Optimizing | `5` | L'indice esegue un'operazione di ottimizzazione. |
| Deleting | `6` | L'indice esegue un'operazione di eliminazione. |
| Renaming | `7` | L'indice esegue un'operazione di rinomina. |
| ChangingAttributes | `8` | L'indice modifica gli attributi. |
| CheckingSegments | `9` | L'indice verifica i segmenti. |
| SavingTheIndex | `10` | L'indice viene salvato in un'altra cartella. |

### Vedi anche

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
