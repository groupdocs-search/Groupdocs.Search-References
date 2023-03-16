---
title: StringOutputAdapter
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο ως αString .
type: docs
weight: 310
url: /el/net/groupdocs.search.common/stringoutputadapter/
---
## StringOutputAdapter class

Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο ως αString .

```csharp
public class StringOutputAdapter : OutputAdapter
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [StringOutputAdapter](stringoutputadapter#constructor_1)(OutputFormat) | Αρχικοποιεί μια νέα παρουσία του[`StringOutputAdapter`](../stringoutputadapter) τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Λαμβάνει τη μορφή εξόδου. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [GetResult](../../groupdocs.search.common/stringoutputadapter/getresult)() | Παίρνει τη συμβολοσειρά που προκύπτει. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Προσαρμογείς εξόδου](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο

index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

DocumentInfo[] documents = index.GetIndexedDocuments(); // Λήψη πληροφοριών για έγγραφα με ευρετήριο

StringOutputAdapter adapter = new StringOutputAdapter(OutputFormat.Html); // Δημιουργία προσαρμογέα εξόδου συμβολοσειράς
index.GetDocumentText(documents[0], adapter); // Δημιουργία κειμένου εγγράφου στον προσαρμογέα
String result = adapter.GetResult(); // Λήψη αποτελέσματος
```

### Δείτε επίσης

* class [OutputAdapter](../outputadapter)
* χώρος ονομάτων [GroupDocs.Search.Common](../../groupdocs.search.common)
* συνέλευση [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->