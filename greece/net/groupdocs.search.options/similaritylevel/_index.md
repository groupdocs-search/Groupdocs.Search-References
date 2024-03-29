---
title: SimilarityLevel
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αντιπροσωπεύει έναν αλγόριθμο της ασαφούς αναζήτησης που καθορίζει το επίπεδο ομοιότητας. Ο αλγόριθμος επιπέδου ομοιότητας υπολογίζει τον μέγιστο αριθμό λαθών για μια λέξη ως αντιστρόφως ανάλογο με το μήκος της λέξης.
type: docs
weight: 1050
url: /el/net/groupdocs.search.options/similaritylevel/
---
## SimilarityLevel class

Αντιπροσωπεύει έναν αλγόριθμο της ασαφούς αναζήτησης που καθορίζει το επίπεδο ομοιότητας. Ο αλγόριθμος επιπέδου ομοιότητας υπολογίζει τον μέγιστο αριθμό λαθών για μια λέξη ως αντιστρόφως ανάλογο με το μήκος της λέξης.

```csharp
public class SimilarityLevel : FuzzyAlgorithm
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [SimilarityLevel](similaritylevel)(double) | Αρχικοποιεί μια νέα παρουσία του[`SimilarityLevel`](../similaritylevel) τάξη. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| override [GetMaxMistakeCount](../../groupdocs.search.options/similaritylevel/getmaxmistakecount)(int) | Λαμβάνει τον μέγιστο επιτρεπόμενο αριθμό σφαλμάτων για το καθορισμένο μήκος όρου. |
| override [GetSimilarityLevel](../../groupdocs.search.options/similaritylevel/getsimilaritylevel)(int) | Λαμβάνει την τιμή του επιπέδου ομοιότητας για το καθορισμένο μήκος όρου. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Ασαφής αναζήτηση](https://docs.groupdocs.com/display/searchnet/Fuzzy+search)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Ενεργοποίηση της ασαφούς αναζήτησης
options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8); // Δημιουργία του ασαφούς αλγορίθμου αναζήτησης
// Αυτή η συνάρτηση καθορίζει το 0 ως τον μέγιστο αριθμό λαθών για λέξεις από 1 έως 4 χαρακτήρες.
// Καθορίζει 1 ως μέγιστο αριθμό λαθών για λέξεις από 5 έως 9 χαρακτήρες.
// Καθορίζει 2 ως μέγιστο αριθμό λαθών για λέξεις από 10 έως 14 χαρακτήρες. Και ούτω καθεξής.

SearchResult result = index.Search(query, options); // Αναζήτηση στο ευρετήριο
```

### Δείτε επίσης

* class [FuzzyAlgorithm](../fuzzyalgorithm)
* χώρος ονομάτων [GroupDocs.Search.Options](../../groupdocs.search.options)
* συνέλευση [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
