---
title: SearchQuery
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Représente une requête de recherche sous forme dobjet.
type: docs
weight: 1240
url: /fr/net/groupdocs.search/searchquery/
---
## SearchQuery class

Représente une requête de recherche sous forme d'objet.

```csharp
public abstract class SearchQuery
```

## Propriétés

| Nom | La description |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Obtient le nombre de requêtes enfants. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Obtient le nom du champ. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Obtient la première requête enfant. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Obtient ou définit les options de recherche de cette requête de recherche. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Obtient la deuxième requête enfant. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête d'origine. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Crée une requête de plage de dates. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Ajoute un champ à la requête spécifiée. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Crée une requête inversée qui trouvera les autres documents dans un index par rapport à ceux qui seront trouvés pour la requête d'origine. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Crée une requête de plage numérique. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour une des requêtes d'origine. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Crée une requête de recherche d'expression. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Crée une requête d'expression régulière. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Crée une requête d'expression régulière. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Crée un caractère générique pour la recherche d'expression. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Crée un caractère générique pour la recherche d'expression. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Crée une requête de modèle de mot. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Crée une requête de mot simple. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Obtient une requête enfant par un index. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Renvoie unString qui représente le courant[`SearchQuery`](../searchquery) instance. |

### Remarques

**Apprendre encore plus**

* [Recherche](https://docs.groupdocs.com/display/searchnet/Searching)
* [Requêtes sous forme de texte et d'objet](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Imbrication des requêtes de recherche sous forme d'objet](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

// Création d'une sous-requête de recherche par plage de dates
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Création d'une sous-requête de caractère générique avec un nombre de mots manqués de 0 à 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Création d'une sous-requête de mot simple
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Définition des options de recherche uniquement pour la sous-requête 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinaison de sous-requêtes en une seule requête
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Création d'un objet d'options de recherche avec une capacité accrue d'occurrences trouvées
SearchOptions options = new SearchOptions(); // Options de recherche globales
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Recherche
```

### Voir également

* espace de noms [GroupDocs.Search](../../groupdocs.search)
* Assemblée [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
