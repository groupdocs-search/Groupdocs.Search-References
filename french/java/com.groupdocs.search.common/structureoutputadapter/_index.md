---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un adaptateur de sortie qui collecte la sortie sous forme d'une structure contenant chaque champ séparément."
type: docs
weight: 33
url: /fr/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Représente un adaptateur de sortie qui collecte la sortie sous forme d'une structure contenant chaque champ séparément.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initialise une nouvelle instance de la classe StructureOutputAdapter. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getResult()](#getResult--) | Obtient le tableau résultant de champs. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Initialise une nouvelle instance de la classe StructureOutputAdapter.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Le format de sortie. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Obtient le tableau résultant de champs.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Le tableau résultant de champs.

