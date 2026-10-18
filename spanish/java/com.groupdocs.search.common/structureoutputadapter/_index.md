---
title: "StructureOutputAdapter"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un adaptador de salida que recopila la salida como una estructura que contiene cada campo por separado."
type: docs
weight: 33
url: /es/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Representa un adaptador de salida que recopila la salida como una estructura que contiene cada campo por separado.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Inicializa una nueva instancia de la clase StructureOutputAdapter. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getResult()](#getResult--) | Obtiene la matriz resultante de campos. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Inicializa una nueva instancia de la clase StructureOutputAdapter.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | El formato de salida. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Obtiene la matriz resultante de campos.


**Returns:**
com.groupdocs.search.common.DocumentField[] - La matriz resultante de campos.

