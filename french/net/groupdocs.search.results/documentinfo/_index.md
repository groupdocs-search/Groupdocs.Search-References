---
title: "DocumentInfo"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un descripteur pour un document indexé."
type: docs
weight: 1230
url: /fr/net/groupdocs.search.results/documentinfo/
---
## DocumentInfo class

Représente un descripteur pour un document indexé.

```csharp
public class DocumentInfo
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DocumentSourceKind](../../groupdocs.search.results/documentinfo/documentsourcekind) { get; } | Obtient le type de source du document. |
| [FilePath](../../groupdocs.search.results/documentinfo/filepath) { get; } | Obtient le chemin du fichier indexé à partir d'un fichier ou la clé du document pour l'indexation à partir d'un flux ou d'une structure. |
| [FileType](../../groupdocs.search.results/documentinfo/filetype) { get; } | Obtient le type de fichier. |
| [FormatFamily](../../groupdocs.search.results/documentinfo/formatfamily) { get; } | Obtient la famille de format du document. |
| [IndexedWithError](../../groupdocs.search.results/documentinfo/indexedwitherror) { get; } | Obtient l'indicateur d'erreur d'indexation. |
| [InnerPath](../../groupdocs.search.results/documentinfo/innerpath) { get; } | Obtient le chemin interne de l'élément de document conteneur. |
| [InnerPathParts](../../groupdocs.search.results/documentinfo/innerpathparts) { get; } | Obtient les parties du chemin interne de l'élément de document conteneur. |
| [ModificationTime](../../groupdocs.search.results/documentinfo/modificationtime) { get; } | Obtient la date de modification. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [Deserialize](../../groupdocs.search.results/documentinfo/deserialize)(byte[]) | Désérialise une instance à partir d'un tableau d'octets. |
| [Serialize](../../groupdocs.search.results/documentinfo/serialize)() | Sérialise l'instance actuelle en un tableau d'octets. |
| override [ToString](../../groupdocs.search.results/documentinfo/tostring)() | Renvoie une chaîne qui représente le [`DocumentInfo`](../documentinfo) actuel. |

### Remarques

**Learn more**

* [Search results](https://docs.groupdocs.com/display/searchnet/Search+results)
* [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)

### Voir aussi

* namespace [GroupDocs.Search.Results](../../groupdocs.search.results)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
