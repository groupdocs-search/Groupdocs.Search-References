---
title: "FragmentHighlighter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans des fragments de texte."
type: docs
weight: 680
url: /fr/net/groupdocs.search.highlighters/fragmenthighlighter/
---
## FragmentHighlighter class

Représente un surligneur de résultats de recherche qui met en évidence les résultats de recherche dans des fragments de texte.

```csharp
public class FragmentHighlighter : Highlighter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FragmentHighlighter](fragmenthighlighter)(OutputFormat) | Initialise une nouvelle instance de la classe [`FragmentHighlighter`](../fragmenthighlighter). |

## Propriétés

| Nom | Description |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Obtient le format de sortie. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetResult](../../groupdocs.search.highlighters/fragmenthighlighter/getresult)() | Obtient un tableau de conteneurs de fragments résultants. |

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

// Rechercher le mot 'Einstein'
SearchResult result = index.Search("Einstein");

// Affectation des options de mise en évidence
HighlightOptions options = new HighlightOptions();
options.TermsBefore = 5;
options.TermsAfter = 5;
options.TermsTotal = 15;

// Mise en évidence des mots trouvés dans le texte d'un document
FoundDocument document = result.GetFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.Highlight(document, highlighter, options);

// Obtention du résultat
FragmentContainer[] fragmentContainers = highlighter.GetResult();
for (int i = 0; i < fragmentContainers.Length; i++)
{
    FragmentContainer container = fragmentContainers[i];
    string[] fragments = container.GetFragments();
    if (fragments.Length > 0)
    {
        Console.WriteLine(container.FieldName);
        Console.WriteLine();
        for (int j = 0; j < fragments.Length; j++)
        {
            // Impression du balisage HTML dans la console
            Console.WriteLine(fragments[j]);
            Console.WriteLine();
        }
    }
}
```

### Voir aussi

* class [Highlighter](../highlighter)
* namespace [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
