---
title: Search
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αναζήτηση σε όλα τα ευρετήρια του αποθετηρίου.
type: docs
weight: 70
url: /el/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Αναζήτηση σε όλα τα ευρετήρια του αποθετηρίου.

```csharp
public SearchResult Search(string query)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| query | String | Το ερώτημα αναζήτησης. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παράδειγμα δείχνει πώς να κάνετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Δημιουργία ευρετηρίου
index.Add(documentsFolder); // Ευρετηρίαση εγγράφων

SearchResult result = repository.Search(query); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* χώρος ονομάτων [GroupDocs.Search](../../indexrepository)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Αναζήτηση σε όλα τα ευρετήρια του αποθετηρίου.

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

Το παράδειγμα δείχνει πώς να κάνετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Δημιουργία ευρετηρίου
index.Add(documentsFolder); // Ευρετηρίαση εγγράφων

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Ρύθμιση σημαίας αναζήτησης με διάκριση πεζών-κεφαλαίων

SearchResult result = repository.Search(query, options); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* χώρος ονομάτων [GroupDocs.Search](../../indexrepository)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Αναζήτηση σε όλα τα ευρετήρια του αποθετηρίου.

```csharp
public SearchResult Search(SearchQuery query)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| query | SearchQuery | Το ερώτημα αναζήτησης. |

### Επιστρεφόμενη Αξία

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παράδειγμα δείχνει πώς να κάνετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Δημιουργία ευρετηρίου
index.Add(documentsFolder); // Ευρετηρίαση εγγράφων

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Δημιουργία ερωτήματος αναζήτησης σε μορφή αντικειμένου

SearchResult result = repository.Search(query); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* χώρος ονομάτων [GroupDocs.Search](../../indexrepository)
* συνέλευση [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Αναζήτηση σε όλα τα ευρετήρια του αποθετηρίου.

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

Το παράδειγμα δείχνει πώς να κάνετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Δημιουργία ευρετηρίου
index.Add(documentsFolder); // Ευρετηρίαση εγγράφων

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Ρύθμιση σημαίας αναζήτησης με διάκριση πεζών-κεφαλαίων

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Δημιουργία ερωτήματος αναζήτησης σε μορφή αντικειμένου

SearchResult result = repository.Search(query, options); // Αναζήτηση
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* χώρος ονομάτων [GroupDocs.Search](../../indexrepository)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
