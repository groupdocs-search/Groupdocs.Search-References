---
title: "TableDiscreteFunction"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Initialise une nouvelle instance de la classe TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction."
type: docs
weight: 10
url: /fr/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

Initialise une nouvelle instance de la classe [`TableDiscreteFunction`](../../tablediscretefunction).

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| offsetOfInputs | Int32 | Le décalage des indices du tableau par rapport aux valeurs d'entrée. |
| tableOfOutputs | Int32[] | Le tableau des valeurs de sortie. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancé lorsque *tableOfOutputs* est `null`. |
| ArgumentException | Lancé lorsque le nombre d'éléments du tableau est 0. |

### Voir aussi

* class [TableDiscreteFunction](../../tablediscretefunction)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

Initialise une nouvelle instance de la classe [`TableDiscreteFunction`](../../tablediscretefunction).

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| firstStepLevel | Int32 | Le niveau de la première étape de la fonction d'étape. |
| steps | Step[] | Les étapes suivantes de la fonction d'étape. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Lancé lorsque *steps* est `null`. |
| ArgumentException | Lancée lorsque les limites des étapes ne sont pas strictement croissantes. |

### Voir aussi

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
