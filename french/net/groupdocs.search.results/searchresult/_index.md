---
title: "SearchResult"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un résultat de recherche correspondant à une requête de recherche."
type: docs
weight: 1310
url: /fr/net/groupdocs.search.results/searchresult/
---
## SearchResult class

Représente un résultat de recherche correspondant à une requête de recherche.

```csharp
public class SearchResult : IEnumerable<FoundDocument>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DocumentCount](../../groupdocs.search.results/searchresult/documentcount) { get; } | Obtient le nombre de documents trouvés. |
| [EndTime](../../groupdocs.search.results/searchresult/endtime) { get; } | Obtient l'heure de fin de la recherche. |
| [NextChunkSearchToken](../../groupdocs.search.results/searchresult/nextchunksearchtoken) { get; } | Obtient un jeton de recherche de fragment pour rechercher le fragment suivant. |
| [OccurrenceCount](../../groupdocs.search.results/searchresult/occurrencecount) { get; } | Obtient le nombre total d'occurrences trouvées. |
| [SearchDuration](../../groupdocs.search.results/searchresult/searchduration) { get; } | Obtient la durée de la recherche. |
| [StartTime](../../groupdocs.search.results/searchresult/starttime) { get; } | Obtient l'heure de début de la recherche. |
| [Truncated](../../groupdocs.search.results/searchresult/truncated) { get; } | Obtient une valeur indiquant que le résultat est tronqué. |
| [Warnings](../../groupdocs.search.results/searchresult/warnings) { get; } | Obtient un avertissement décrivant le résultat. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../groupdocs.search.results/searchresult/getenumerator)() | Renvoie un énumérateur qui parcourt la collection des documents trouvés. |
| [GetFoundDocument](../../groupdocs.search.results/searchresult/getfounddocument)(int) | Obtient le document trouvé par indice. |

### Remarques

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Search results](https://docs.groupdocs.com/display/searchnet/Search+results)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// Création d'un index
Index index = new Index(indexFolder);

// Indexation des documents depuis le dossier spécifié
index.Add(documentFolder);

// Définition des options de recherche
SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting the maximum number of differences to 3

// Rechercher des documents contenant le mot 'Einstein' ou la phrase 'Theory of Relativity'
SearchResult result = index.Search("Einstein OR \"Theory of Relativity\"", options);

// Impression du résultat
Console.WriteLine("Documents: " + result.DocumentCount);
Console.WriteLine("Total occurrences: " + result.OccurrenceCount);
for (int i = 0; i < result.DocumentCount; i++)
{
    FoundDocument document = result.GetFoundDocument(i);
    Console.WriteLine("\tDocument: " + document.DocumentInfo.FilePath);
    Console.WriteLine("\tOccurrences: " + document.OccurrenceCount);
    for (int j = 0; j < document.FoundFields.Length; j++)
    {
        FoundDocumentField field = document.FoundFields[j];
        Console.WriteLine("\t\tField: " + field.FieldName);
        Console.WriteLine("\t\tOccurrences: " + document.OccurrenceCount);
        // Impression des termes trouvés
        if (field.Terms != null)
        {
            for (int k = 0; k < field.Terms.Length; k++)
            {
                Console.WriteLine("\t\t\t" + field.Terms[k].PadRight(20) + field.TermsOccurrences[k]);
            }
        }
        // Impression des phrases trouvées
        if (field.TermSequences != null)
        {
            for (int k = 0; k < field.TermSequences.Length; k++)
            {
                string sequence = string.Join(" ", field.TermSequences[k]);
                Console.WriteLine("\t\t\t" + sequence.PadRight(30) + field.TermSequencesOccurrences[k]);
            }
        }
    }
}
```

### Voir aussi

* class [FoundDocument](../founddocument)
* namespace [GroupDocs.Search.Results](../../groupdocs.search.results)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
