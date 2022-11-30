---
title: TableDiscreteFunction
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Inizializza una nuova istanza diTableDiscreteFunctiongroupdocs.search.options/tablediscretefunction classe.
type: docs
weight: 10
url: /it/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

Inizializza una nuova istanza di[`TableDiscreteFunction`](../../tablediscretefunction) classe.

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| offsetOfInputs | Int32 | L'offset della tabella indicizza rispetto ai valori di input. |
| tableOfOutputs | Int32[] | La tabella dei valori di output. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Lanciato quando*tableOfOutputs* è`nullo`. |
| ArgumentException | Generato quando il numero di elementi della tabella è 0. |

### Guarda anche

* class [TableDiscreteFunction](../../tablediscretefunction)
* spazio dei nomi [GroupDocs.Search.Options](../../tablediscretefunction)
* assemblea [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

Inizializza una nuova istanza di[`TableDiscreteFunction`](../../tablediscretefunction) classe.

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstStepLevel | Int32 | Il livello del primo passo della funzione passo. |
| steps | Step[] | I passi successivi della funzione passo. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentNullException | Lanciato quando*steps* è`nullo`. |
| ArgumentException | Lanciato quando i limiti dei passaggi non sono strettamente crescenti. |

### Guarda anche

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* spazio dei nomi [GroupDocs.Search.Options](../../tablediscretefunction)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->