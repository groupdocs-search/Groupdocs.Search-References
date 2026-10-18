---
title: "DocumentHighlighter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans le texte complet d'un document."
type: docs
weight: 670
url: /fr/net/groupdocs.search.highlighters/documenthighlighter/
---
## DocumentHighlighter class

Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans le texte complet d'un document.

```csharp
public class DocumentHighlighter : Highlighter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [DocumentHighlighter](documenthighlighter)(OutputAdapter) | Initialise une nouvelle instance de la classe [`DocumentHighlighter`](../documenthighlighter). |

## Propriétés

| Nom | Description |
| --- | --- |
| [OutputAdapter](../../groupdocs.search.highlighters/documenthighlighter/outputadapter) { get; } | Obtient l'adaptateur de sortie passé au constructeur. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Obtient le format de sortie. |

### Remarques

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);

// Rechercher la phase 'Theory of Relativity'
SearchResult result = index.Search("\"Theory of Relativity\"");

// Mise en évidence des mots trouvés dans le texte d'un document
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Voir aussi

* class [Highlighter](../highlighter)
* namespace [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
