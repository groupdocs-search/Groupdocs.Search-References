---
title: "Αναζήτηση"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Αναζητά σε όλους τους δείκτες του αποθετηρίου."
type: docs
weight: 70
url: /el/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Αναζητά σε όλους τους δείκτες του αποθετηρίου.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| ερώτημα | String | Το ερώτημα αναζήτησης. |

### Τιμή Επιστροφής

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchResult result = repository.Search(query); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Αναζητά σε όλους τους δείκτες του αποθετηρίου.

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

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Setting flag of case sensitive search

SearchResult result = repository.Search(query, options); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Αναζητά σε όλους τους δείκτες του αποθετηρίου.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| ερώτημα | SearchQuery | Το ερώτημα αναζήτησης. |

### Τιμή Επιστροφής

Το αποτέλεσμα αναζήτησης.

### Παραδείγματα

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Αναζητά σε όλους τους δείκτες του αποθετηρίου.

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

Το παράδειγμα δείχνει πώς να εκτελέσετε αναζήτηση στο αποθετήριο ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Setting flag of case sensitive search

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creating search query in object form

SearchResult result = repository.Search(query, options); // Searching
```

### Δείτε επίσης

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
