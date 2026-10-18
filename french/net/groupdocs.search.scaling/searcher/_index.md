---
title: "Moteur de recherche"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un service qui gère les requêtes de recherche vers les fragments du réseau de recherche."
type: docs
weight: 1570
url: /fr/net/groupdocs.search.scaling/searcher/
---
## Searcher class

Représente un service qui gère les requêtes de recherche vers les fragments du réseau de recherche.

```csharp
public sealed class Searcher
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetDocumentText](../../groupdocs.search.scaling/searcher/getdocumenttext)(NetworkDocumentInfo, OutputAdapter) | Génère le texte d'un document indexé et le transmet via un adaptateur de sortie. |
| [GetIndexedDocumentItems](../../groupdocs.search.scaling/searcher/getindexeddocumentitems)(NetworkDocumentInfo) | Obtient un tableau d'éléments imbriqués du document spécifié (pour les documents conteneurs tels que ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search.scaling/searcher/getindexeddocuments)(int) | Obtient un tableau de tous les documents indexés. |
| [Highlight](../../groupdocs.search.scaling/searcher/highlight)(NetworkFoundDocument, Highlighter, HighlightOptions) | Génère du texte formaté en HTML avec les termes trouvés mis en évidence. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst)(SearchImage, ImageSearchOptions) | Démarre une recherche d'image inversée dans l'index de recherche distribué. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst_1)(SearchQuery, SearchOptions) | Démarre une recherche avec une requête sous forme d'objet dans l'index de recherche distribué. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst_2)(string, SearchOptions) | Démarre une recherche avec une requête sous forme de texte dans l'index de recherche distribué. |
| [SearchNext](../../groupdocs.search.scaling/searcher/searchnext#searchnext)(NetworkImageSearchToken) | Poursuit une recherche d'image inversée dans l'index de recherche distribué. |
| [SearchNext](../../groupdocs.search.scaling/searcher/searchnext#searchnext_1)(NetworkSearchToken) | Poursuit une recherche dans l'index de recherche distribué. |

### Voir aussi

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
