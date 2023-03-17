---
title: SearchQuery
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αντιπροσωπεύει ένα ερώτημα αναζήτησης σε μορφή αντικειμένου.
type: docs
weight: 1240
url: /el/net/groupdocs.search/searchquery/
---
## SearchQuery class

Αντιπροσωπεύει ένα ερώτημα αναζήτησης σε μορφή αντικειμένου.

```csharp
public abstract class SearchQuery
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Λαμβάνει τον αριθμό των θυγατρικών ερωτημάτων. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Λαμβάνει το όνομα του πεδίου. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Λαμβάνει το πρώτο θυγατρικό ερώτημα. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Λαμβάνει ή ορίζει τις επιλογές αναζήτησης αυτού του ερωτήματος αναζήτησης. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Λαμβάνει το δεύτερο θυγατρικό ερώτημα. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Δημιουργεί ένα ερώτημα εύρους ημερομηνιών. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Προσθέτει ένα πεδίο στο καθορισμένο ερώτημα. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Δημιουργεί ένα ανεστραμμένο ερώτημα που θα βρει τα υπόλοιπα έγγραφα σε ένα ευρετήριο έναντι αυτών που θα βρεθούν για το αρχικό ερώτημα. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Δημιουργεί ένα ερώτημα αριθμητικής περιοχής. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον για ένα από τα αρχικά ερωτήματα. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Δημιουργεί ένα ερώτημα αναζήτησης φράσης. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Δημιουργεί ένα ερώτημα τυπικής έκφρασης. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Δημιουργεί ένα ερώτημα τυπικής έκφρασης. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Δημιουργεί έναν μπαλαντέρ για την αναζήτηση φράσης. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Δημιουργεί έναν μπαλαντέρ για την αναζήτηση φράσης. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Δημιουργεί ένα ερώτημα μοτίβου λέξης. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Δημιουργεί ένα απλό ερώτημα λέξης. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Λαμβάνει ένα θυγατρικό ερώτημα από ένα ευρετήριο. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Επιστρέφει αString που αντιπροσωπεύει το ρεύμα[`SearchQuery`](../searchquery) παράδειγμα. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Ερευνητικός](https://docs.groupdocs.com/display/searchnet/Searching)
* [Ερωτήματα σε μορφή κειμένου και αντικειμένου](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Ένθεση ερωτημάτων αναζήτησης σε μορφή αντικειμένου](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

// Δημιουργία υποερωτήματος αναζήτησης εύρους ημερομηνιών
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Δημιουργία υποερωτήματος μπαλαντέρ με αριθμό χαμένων λέξεων από 0 έως 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Δημιουργία υποερωτήματος απλής λέξης
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Ρύθμιση επιλογών αναζήτησης μόνο για το δευτερεύον ερώτημα 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Συνδυασμός υποερωτημάτων σε ένα ερώτημα
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Δημιουργία αντικειμένου επιλογών αναζήτησης με αυξημένη χωρητικότητα εντοπισμένων εμφανίσεων
SearchOptions options = new SearchOptions(); // Συνολικές επιλογές αναζήτησης
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Αναζήτηση
```

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Search](../../groupdocs.search)
* συνέλευση [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
