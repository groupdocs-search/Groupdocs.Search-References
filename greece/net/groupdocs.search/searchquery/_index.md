---
title: "SearchQuery"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Αντιπροσωπεί ένα ερώτημα αναζήτησης σε μορφή αντικειμένου."
type: docs
weight: 1580
url: /el/net/groupdocs.search/searchquery/
---
## SearchQuery class

Αντιπροσωπεί ένα ερώτημα αναζήτησης σε μορφή αντικειμένου.

```csharp
public abstract class SearchQuery
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Λαμβάνει τον αριθμό των θυγατρικών ερωτημάτων. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Λαμβάνει το όνομα του πεδίου. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Λαμβάνει το πρώτο θυγατρικό ερώτημα. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Λαμβάνει ή ορίζει τις επιλογές αναζήτησης αυτού του ερωτήματος αναζήτησης. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Λαμβάνει το δεύτερο θυγατρικό ερώτημα. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery_1)(params SearchQuery[]) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρίσκει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα. |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery#createandquery)(SearchQuery, SearchQuery) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρίσκει μόνο έγγραφα που θα βρεθούν για κάθε αρχικό ερώτημα. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Δημιουργεί ένα ερώτημα εύρους ημερομηνίας. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Προσθέτει ένα πεδίο στο καθορισμένο ερώτημα. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Δημιουργεί ένα ανεστραμμένο ερώτημα που θα βρει τα υπόλοιπα έγγραφα σε ένα ευρετήριο σε αντίθεση με αυτά που θα βρεθούν για το αρχικό ερώτημα. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Δημιουργεί ένα ερώτημα αριθμητικού εύρους. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery_1)(params SearchQuery[]) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον σε ένα από τα αρχικά ερωτήματα. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery#createorquery)(SearchQuery, SearchQuery) | Δημιουργεί ένα συνδυασμένο ερώτημα που θα βρει όλα τα έγγραφα που θα βρεθούν τουλάχιστον σε ένα από τα αρχικά ερωτήματα. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Δημιουργεί ένα ερώτημα αναζήτησης φράσης. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Δημιουργεί ένα ερώτημα κανονικής έκφρασης. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Δημιουργεί ένα ερώτημα κανονικής έκφρασης. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Δημιουργεί ένα μπαλαντέρ για την αναζήτηση φράσης. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Δημιουργεί ένα μπαλαντέρ για την αναζήτηση φράσης. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Δημιουργεί ένα ερώτημα προτύπου λέξης. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Δημιουργεί ένα απλό ερώτημα λέξης. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Αποκτά ένα θυγατρικό ερώτημα με δείκτη. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον [`SearchQuery`](../searchquery) αντικείμενο. |

### Σχόλια

**Learn more**

* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)
* [Queries in text and object form](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Nesting search queries in object form](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Δημιουργία υποερωτήματος αναζήτησης εύρους ημερομηνίας
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Δημιουργία υποερωτήματος μπαλαντέρ με αριθμό παραλειπόμενων λέξεων από 0 έως 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Δημιουργία υποερωτήματος απλής λέξης
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Συνδυασμός υποερωτημάτων σε ένα ερώτημα
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Δημιουργία αντικειμένου επιλογών αναζήτησης με αυξημένη χωρητικότητα των ευρεθεισών εμφανίσεων
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Δείτε επίσης

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
