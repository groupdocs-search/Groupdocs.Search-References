---
title: "FileIndexingEventArgs"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente les arguments de l'événement de démarrage de l'indexation d'un document."
type: docs
weight: 540
url: /fr/net/groupdocs.search.events/fileindexingeventargs/
---
## FileIndexingEventArgs class

Représente les arguments de l'événement de démarrage de l'indexation d'un document.

```csharp
public class FileIndexingEventArgs : BaseIndexEventArgs
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.events/fileindexingeventargs/additionalfields) { get; set; } | Obtient ou définit les champs supplémentaires du document. |
| [Attributes](../../groupdocs.search.events/fileindexingeventargs/attributes) { get; set; } | Obtient ou définit les attributs du document. |
| [CustomExtractor](../../groupdocs.search.events/fileindexingeventargs/customextractor) { get; set; } | Obtient ou définit l'extracteur de texte personnalisé. |
| [Document](../../groupdocs.search.events/fileindexingeventargs/document) { get; } | Obtient le document. |
| [DocumentFullPath](../../groupdocs.search.events/fileindexingeventargs/documentfullpath) { get; } | Obtient le chemin complet du document. |
| [DocumentKey](../../groupdocs.search.events/fileindexingeventargs/documentkey) { get; } | Obtient la clé du document. |
| [Encoding](../../groupdocs.search.events/fileindexingeventargs/encoding) { get; set; } | Obtient ou définit l'encodage du document. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Obtient le dossier d'index. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Obtient l'ID de l'index. |
| [SkipIndexing](../../groupdocs.search.events/fileindexingeventargs/skipindexing) { get; set; } | Obtient ou définit une valeur indiquant que l'indexation du document doit être ignorée. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Obtient le statut de l'index. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Obtient le moment d'un événement. |
| [WordSplitter](../../groupdocs.search.events/fileindexingeventargs/wordsplitter) { get; set; } | Obtient ou définit le séparateur de mots personnalisé utilisé pour diviser le texte en mots. |

### Remarques

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Voir aussi

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
