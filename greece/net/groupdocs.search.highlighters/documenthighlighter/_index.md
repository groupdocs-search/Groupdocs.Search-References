---
title: DocumentHighlighter
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αντιπροσωπεύει ένα εργαλείο επισήμανσης αποτελεσμάτων αναζήτησης που επισημαίνει τα αποτελέσματα αναζήτησης σε ένα ολόκληρο κείμενο εγγράφου.
type: docs
weight: 630
url: /el/net/groupdocs.search.highlighters/documenthighlighter/
---
## DocumentHighlighter class

Αντιπροσωπεύει ένα εργαλείο επισήμανσης αποτελεσμάτων αναζήτησης που επισημαίνει τα αποτελέσματα αναζήτησης σε ένα ολόκληρο κείμενο εγγράφου.

```csharp
public class DocumentHighlighter : Highlighter
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [DocumentHighlighter](documenthighlighter)(OutputAdapter) | Αρχικοποιεί μια νέα παρουσία του[`DocumentHighlighter`](../documenthighlighter) τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [OutputAdapter](../../groupdocs.search.highlighters/documenthighlighter/outputadapter) { get; } | Παίρνει τον προσαρμογέα εξόδου που περνά στον κατασκευαστή. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Λαμβάνει τη μορφή εξόδου. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Επισήμανση αποτελεσμάτων αναζήτησης](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Δημιουργία ευρετηρίου
Index index = new Index(indexFolder);

// Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο
index.Add(documentsFolder);

// Αναζήτηση για τη φάση «Θεωρία της Σχετικότητας»
SearchResult result = index.Search("\"Theory of Relativity\"");

// Επισήμανση λέξεων που βρέθηκαν στο κείμενο ενός εγγράφου
FoundDocument document = result.GetFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.Highlight(document, highlighter);
```

### Δείτε επίσης

* class [Highlighter](../highlighter)
* χώρος ονομάτων [GroupDocs.Search.Highlighters](../../groupdocs.search.highlighters)
* συνέλευση [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
