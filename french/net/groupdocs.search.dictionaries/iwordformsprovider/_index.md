---
title: "IWordFormsProvider"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Définit l'interface d'un fournisseur de formes de mots."
type: docs
weight: 470
url: /fr/net/groupdocs.search.dictionaries/iwordformsprovider/
---
## IWordFormsProvider interface

Définit l'interface d'un fournisseur de formes de mots.

```csharp
public interface IWordFormsProvider
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetWordForms](../../groupdocs.search.dictionaries/iwordformsprovider/getwordforms)(string) | Obtient les formes du mot pour le mot spécifié. Le tableau résultant ne contient pas le mot original. |

### Remarques

**Learn more**

* [Search for different word forms](https://docs.groupdocs.com/display/searchnet/Search+for+different+word+forms)
* [Word forms provider](https://docs.groupdocs.com/display/searchnet/Word+forms+provider)

### Exemples

L'exemple suivant montre comment implémenter un fournisseur de formes de mots personnalisé.

```csharp
public class SimpleWordFormsProvider : IWordFormsProvider
{
    public string[] GetWordForms(string word)
    {
        List<string> result = new List<string>();

        // Supposons que le mot d'entrée soit au pluriel, alors nous ajoutons le singulier.
        if (word.Length > 2 &&
            word.EndsWith("es", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 2));
        }
        if (word.Length > 1 &&
            word.EndsWith("s", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1));
        }

        // Ensuite, supposons que le mot d'entrée soit au singulier, nous ajoutons le pluriel.
        if (word.Length > 1 &&
            word.EndsWith("y", StringComparison.InvariantCultureIgnoreCase))
        {
            result.Add(word.Substring(0, word.Length - 1) + "is");
        }
        result.Add(word + "s");
        result.Add(word + "es");
        // Toutes les règles sont implémentées dans la classe EnglishWordFormsProvider.

        return result.ToArray();
    }
}
```

L'exemple suivant montre comment définir un fournisseur de formes de mots personnalisé à utiliser.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
  
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
  
// Indexation des documents depuis le dossier spécifié
index.Add(documentsFolder);
 
// Définition de l'instance du fournisseur de formes de mots personnalisé
index.Dictionaries.WordFormsProvider = new SimpleWordFormsProvider();
 
// Création d'une instance d'options de recherche
SearchOptions options = new SearchOptions();
options.UseWordFormsSearch = true; // Enabling search for word forms
  
// Recherche dans l'index
SearchResult result = index.Search("relative", options);
  
// Les mots suivants peuvent être trouvés :
// relatif
// parents
```

### Voir aussi

* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
