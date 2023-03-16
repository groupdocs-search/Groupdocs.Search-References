---
title: FileLogger
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αντιπροσωπεύει έναν καταγραφέα που καταγράφει συμβάντα και σφάλματα σε ένα τοπικό αρχείο.
type: docs
weight: 140
url: /el/net/groupdocs.search.common/filelogger/
---
## FileLogger class

Αντιπροσωπεύει έναν καταγραφέα που καταγράφει συμβάντα και σφάλματα σε ένα τοπικό αρχείο.

```csharp
public class FileLogger : ILogger
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [FileLogger](filelogger)(string, double) | Αρχικοποιεί μια νέα παρουσία του[`FileLogger`](../filelogger) τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [FilePath](../../groupdocs.search.common/filelogger/filepath) { get; } | Λαμβάνει τη διαδρομή του αρχείου καταγραφής. |
| [MaxSize](../../groupdocs.search.common/filelogger/maxsize) { get; } | Λαμβάνει το μέγιστο μέγεθος αρχείου καταγραφής σε megabyte. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Error](../../groupdocs.search.common/filelogger/error)(string) | Καταγράφει ένα σφάλμα που παρουσιάστηκε στο ευρετήριο. |
| [Trace](../../groupdocs.search.common/filelogger/trace)(string) | Καταγράφει ένα συμβάν που συνέβη στο ευρετήριο. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Ξύλευση](https://docs.groupdocs.com/display/searchnet/Logging)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";
string logPath = @"c:\Log.txt";

IndexSettings settings = new IndexSettings();
settings.Logger = new FileLogger(logPath, 4.0); // Καθορισμός της διαδρομής προς το αρχείο καταγραφής και μέγιστου μήκους 4 MB

Index index = new Index(indexFolder, settings); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο

index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

SearchResult result = index.Search(query); // Αναζήτηση στο ευρετήριο
```

### Δείτε επίσης

* interface [ILogger](../ilogger)
* χώρος ονομάτων [GroupDocs.Search.Common](../../groupdocs.search.common)
* συνέλευση [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->