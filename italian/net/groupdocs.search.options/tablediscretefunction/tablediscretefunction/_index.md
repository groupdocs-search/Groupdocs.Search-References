---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Inizializza una nuova istanza della classe TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction."
type: docs
weight: 10
url: /it/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

Inizializza una nuova istanza della classe [`TableDiscreteFunction`](../../tablediscretefunction).

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| offsetOfInputs | Int32 | L'offset degli indici della tabella relativo ai valori di input. |
| tableOfOutputs | Int32[] | La tabella dei valori di output. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generato quando *tableOfOutputs* è `null`. |
| ArgumentException | Generato quando il numero di elementi della tabella è 0. |

### Vedi anche

* class [TableDiscreteFunction](../../tablediscretefunction)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

Inizializza una nuova istanza della classe [`TableDiscreteFunction`](../../tablediscretefunction).

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| firstStepLevel | Int32 | Il livello del primo passo della funzione a gradini. |
| steps | Step[] | I prossimi passi della funzione a gradini. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Generato quando *steps* è `null`. |
| ArgumentException | Generato quando i limiti dei passaggi non sono strettamente crescenti. |

### Vedi anche

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
