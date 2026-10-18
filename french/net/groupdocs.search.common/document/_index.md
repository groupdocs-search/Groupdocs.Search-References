---
title: "Document"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente la classe de base pour les documents ajoutés à un index à partir d'un flux ou d'une structure du système de fichiers. Contient des méthodes statiques pour créer des documents à partir de différents types de sources."
type: docs
weight: 50
url: /fr/net/groupdocs.search.common/document/
---
## Document class

Représente la classe de base pour les documents ajoutés à un index depuis le système de fichiers, un flux ou une structure. Contient des méthodes statiques pour créer des documents à partir de différents types de sources.

```csharp
public abstract class Document
```

## Propriétés

| Nom | Description |
| --- | --- |
| virtual [AdditionalFields](../../groupdocs.search.common/document/additionalfields) { get; set; } | Obtient ou définit les champs supplémentaires du document. |
| virtual [Attributes](../../groupdocs.search.common/document/attributes) { get; set; } | Obtient ou définit les attributs du document. |
| abstract [DocumentKey](../../groupdocs.search.common/document/documentkey) { get; } | Obtient la clé du document utilisée pour identifier le document au sein d'un index. |
| abstract [DocumentSourceKind](../../groupdocs.search.common/document/documentsourcekind) { get; } | Obtient le type de source du document. |
| abstract [Extension](../../groupdocs.search.common/document/extension) { get; } | Obtient l'extension utilisée pour ce type de document. |
| abstract [IsLazy](../../groupdocs.search.common/document/islazy) { get; } | Obtient une valeur indiquant si le document est chargé à la demande ou non. |
| abstract [ModificationDate](../../groupdocs.search.common/document/modificationdate) { get; } | Obtient la date de dernière modification du document. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateFromFile](../../groupdocs.search.common/document/createfromfile)(string) | Crée un document à partir d'un fichier. |
| static [CreateFromStream](../../groupdocs.search.common/document/createfromstream)(string, DateTime, string, Stream) | Crée un document à partir d'un flux. |
| static [CreateFromStructure](../../groupdocs.search.common/document/createfromstructure)(string, DateTime, DocumentField[]) | Crée un document à partir d'une structure qui est un tableau de champs texte. |
| static [CreateLazy](../../groupdocs.search.common/document/createlazy)(DocumentSourceKind, string, IDocumentLoader) | Crée un document chargé paresseusement. |
| override [ToString](../../groupdocs.search.common/document/tostring)() | Renvoie une String qui représente le [`Document`](../document) actuel. |

### Remarques

**Learn more**

* [Indexing from different sources](https://docs.groupdocs.com/search/net/indexing-from-different-sources/)

### Voir aussi

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
