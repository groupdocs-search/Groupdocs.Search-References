---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output come una struttura contenente ogni campo separatamente."
type: docs
weight: 33
url: /it/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Rappresenta un adattatore di output che raccoglie l'output come una struttura contenente ogni campo separatamente.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Inizializza una nuova istanza della classe StructureOutputAdapter. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getResult()](#getResult--) | Ottiene l'array risultante di campi. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Inizializza una nuova istanza della classe StructureOutputAdapter.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Il formato di output. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Ottiene l'array risultante di campi.


**Returns:**
com.groupdocs.search.common.DocumentField[] - L'array risultante di campi.

