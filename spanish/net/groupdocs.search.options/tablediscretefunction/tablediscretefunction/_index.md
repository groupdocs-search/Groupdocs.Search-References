---
title: TableDiscreteFunction
second_title: GroupDocs.Buscar referencia de API de .NET
description: Inicializa una nueva instancia delTableDiscreteFunctiongroupdocs.search.options/tablediscretefunction clase.
type: docs
weight: 10
url: /es/net/groupdocs.search.options/tablediscretefunction/tablediscretefunction/
---
## TableDiscreteFunction(int, int[]) {#constructor_1}

Inicializa una nueva instancia del[`TableDiscreteFunction`](../../tablediscretefunction) clase.

```csharp
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| offsetOfInputs | Int32 | El desplazamiento de los índices de la tabla en relación con los valores de entrada. |
| tableOfOutputs | Int32[] | La tabla de valores de salida. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | arrojado cuando*tableOfOutputs* es`nulo`. |
| ArgumentException | Se lanza cuando el número de elementos de la tabla es 0. |

### Ver también

* class [TableDiscreteFunction](../../tablediscretefunction)
* espacio de nombres [GroupDocs.Search.Options](../../tablediscretefunction)
* asamblea [GroupDocs.Search](../../../)

---

## TableDiscreteFunction(int, params Step[]) {#constructor}

Inicializa una nueva instancia del[`TableDiscreteFunction`](../../tablediscretefunction) clase.

```csharp
public TableDiscreteFunction(int firstStepLevel, params Step[] steps)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| firstStepLevel | Int32 | El nivel del primer paso de la función de paso. |
| steps | Step[] | Los siguientes pasos de la función de paso. |

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | arrojado cuando*steps* es`nulo`. |
| ArgumentException | Se lanza cuando los límites de los pasos no son estrictamente crecientes. |

### Ver también

* class [Step](../../step)
* class [TableDiscreteFunction](../../tablediscretefunction)
* espacio de nombres [GroupDocs.Search.Options](../../tablediscretefunction)
* asamblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->