---
title: "Αναζήτηση"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Αναζητά στο ευρετήριο."
type: docs
weight: 260
url: /el/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Αναζητά στο ευρετήριο.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| ερώτημα | String | Το ερώτημα αναζήτησης. |

### Τιμή Επιστροφής

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε απλή αναζήτηση.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση με κανονικές εκφράσεις.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε φασέτα αναζήτηση.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Αναζητά στο ευρετήριο.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| ερώτημα | String | Το ερώτημα αναζήτησης. |
| επιλογές | SearchOptions | Οι επιλογές αναζήτησης. |

### Τιμή Επιστροφής

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε ασαφή αναζήτηση.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Τα διπλά εισαγωγικά στην αρχή και στο τέλος ενημερώνουν το ευρετήριο ότι είναι ερώτημα φράσης.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση συνωνύμων.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Enabling the synonym search

string query = "cry";
SearchResult result = index.Search(query, options); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Αναζητά στο ευρετήριο.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| ερώτημα | SearchQuery | Το ερώτημα αναζήτησης. |

### Τιμή Επιστροφής

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Δημιουργία υποερωτήματος 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Δημιουργία υποερωτήματος 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Δημιουργία υποερωτήματος 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Συνδυασμός υποερωτημάτων σε ένα ερώτημα
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Αναζητά στο ευρετήριο.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| ερώτημα | SearchQuery | Το ερώτημα αναζήτησης. |
| επιλογές | SearchOptions | Οι επιλογές αναζήτησης. |

### Τιμή Επιστροφής

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παρακάτω παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση χρησιμοποιώντας ερώτημα σε μορφή αντικειμένου.

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

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Εκτελεί αντίστροφη αναζήτηση εικόνας στο ευρετήριο.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| εικόνα | SearchImage | Η εικόνα για αναζήτηση. |
| επιλογές | ImageSearchOptions | Οι επιλογές αναζήτησης εικόνας. |

### Τιμή Επιστροφής

Το αποτέλεσμα μιας αντίστροφης αναζήτησης εικόνας.

### Δείτε επίσης

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
