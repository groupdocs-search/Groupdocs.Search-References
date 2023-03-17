---
title: Search
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αναζητήσεις στο ευρετήριο.
type: docs
weight: 220
url: /el/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Αναζητήσεις στο ευρετήριο.

```csharp
public SearchResult Search(string query)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| query | String | Το ερώτημα αναζήτησης. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να κάνετε απλή αναζήτηση.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

SearchResult result = index.Search(query); // Αναζήτηση
```

Το ακόλουθο παράδειγμα δείχνει πώς να πραγματοποιήσετε αναζήτηση Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

string query = "^[0-9]{3,}"; // Το σύμβολο caret στην αρχή του ερωτήματος αναζήτησης λέει στο ευρετήριο ότι είναι ερώτημα Regex
SearchResult result = index.Search(query); // Αναζήτηση
```

Το ακόλουθο παράδειγμα δείχνει πώς να εκτελείτε πολύπλευρη αναζήτηση.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

string query = "content:Newton"; // Η λέξη πριν από την άνω και κάτω τελεία στο ερώτημα σημαίνει το όνομα του πεδίου του εγγράφου για αναζήτηση
SearchResult result = index.Search(query); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Αναζητήσεις στο ευρετήριο.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| query | String | Το ερώτημα αναζήτησης. |
| options | SearchOptions | Οι επιλογές αναζήτησης. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εκτελείτε ασαφή αναζήτηση.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Ενεργοποίηση της ασαφούς αναζήτησης
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Ρύθμιση του αριθμού των πιθανών διαφορών για κάθε λέξη

// Τα διπλά εισαγωγικά στην αρχή και στο τέλος λένε στο ευρετήριο ότι είναι ερώτημα αναζήτησης φράσης
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Αναζήτηση
```

Το ακόλουθο παράδειγμα δείχνει πώς να πραγματοποιήσετε αναζήτηση συνωνύμων.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Ενεργοποίηση της αναζήτησης συνωνύμων

string query = "cry";
SearchResult result = index.Search(query, options); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Αναζητήσεις στο ευρετήριο.

```csharp
public SearchResult Search(SearchQuery query)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| query | SearchQuery | Το ερώτημα αναζήτησης. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εκτελείτε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

// Δημιουργία υποερωτήματος 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Ρύθμιση επιλογών αναζήτησης μόνο για το δευτερεύον ερώτημα 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Ενεργοποίηση της ασαφούς αναζήτησης
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Ρύθμιση μέγιστου αριθμού διαφορών

// Δημιουργία υποερωτήματος 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Δημιουργία υποερωτήματος 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Συνδυασμός υποερωτημάτων σε ένα ερώτημα
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Αναζητήσεις στο ευρετήριο.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| query | SearchQuery | Το ερώτημα αναζήτησης. |
| options | SearchOptions | Οι επιλογές αναζήτησης. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει πώς να εκτελείτε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

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

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Εκτελεί αντίστροφη αναζήτηση εικόνας στο ευρετήριο.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| image | SearchImage | Η εικόνα για αναζήτηση. |
| options | ImageSearchOptions | Οι επιλογές αναζήτησης εικόνων. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα μιας αντίστροφης αναζήτησης εικόνων.

### Δείτε επίσης

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
