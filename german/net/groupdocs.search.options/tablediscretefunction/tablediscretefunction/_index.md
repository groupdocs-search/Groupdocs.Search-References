---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Initialisiert eine neue Instanz der Klasse TableDiscreteFunctiongroupdocs.search.options/tablediscretefunction."
type: docs
weight: 10
url: /de/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

Initialisiert eine neue Instanz der Klasse [`TableDiscreteFunction`](../../tablediscretefunction).

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| offsetOfInputs | Int32 | Der Versatz der Tabelleneindizes relativ zu den Eingabewerten. |
| tableOfOutputs | Int32[] | Die Tabelle der Ausgabewerte. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *tableOfOutputs* `null` ist. |
| ArgumentException | Wird ausgelöst, wenn die Anzahl der Tabellenelemente 0 ist. |

### Siehe auch

* class [TableDiscreteFunction](../../tablediscretefunction)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

Initialisiert eine neue Instanz der Klasse [`TableDiscreteFunction`](../../tablediscretefunction).

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| firstStepLevel | Int32 | Die Ebene des ersten Schritts der Schrittfunktion. |
| steps | Step[] | Die nächsten Schritte der Schrittfunktion. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Wird ausgelöst, wenn *steps* `null` ist. |
| ArgumentException | Wird ausgelöst, wenn die Grenzen der Schritte nicht streng monoton ansteigen. |

### Siehe auch

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
