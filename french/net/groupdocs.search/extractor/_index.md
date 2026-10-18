---
title: "Extracteur"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un outil d'extraction préliminaire de données à partir de documents afin de séparer l'étape d'indexation rapide ultérieure."
type: docs
weight: 660
url: /fr/net/groupdocs.search/extractor/
---
## Extractor class

Représente un outil d'extraction préliminaire de données à partir de documents afin de séparer l'étape d'indexation rapide ultérieure.

```csharp
public class Extractor
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [Extractor](extractor)() | Initialise une nouvelle instance de la classe [`Extractor`](../extractor). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Settings](../../groupdocs.search/extractor/settings) { get; } | Obtient les paramètres de l'extracteur. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Extract](../../groupdocs.search/extractor/extract)(Document, ExtractionOptions) | Extrait des données d'un document. |

## Événements

| Nom | Description |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search/extractor/erroroccurred) | Se produit lorsqu'une erreur survient pendant une opération d'extracteur. |
| event [ImagePreparing](../../groupdocs.search/extractor/imagepreparing) | Se produit lorsqu'une image va être préparée pour l'indexation. |
| event [PasswordRequired](../../groupdocs.search/extractor/passwordrequired) | Se produit lorsqu'un document nécessite un mot de passe pour être ouvert. |

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
