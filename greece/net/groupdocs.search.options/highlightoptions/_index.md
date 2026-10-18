---
title: "HighlightOptions"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Παρέχει επιλογές για την επισήμανση των ευρεθέντων όρων."
type: docs
weight: 910
url: /el/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Παρέχει επιλογές για την επισήμανση των ευρεθέντων όρων.

```csharp
public class HighlightOptions : TextOptions
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Αρχικοποιεί μια νέα παρουσία της κλάσης [`HighlightOptions`](../highlightoptions). |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Λαμβάνει ή ορίζει τα πρόσθετα πεδία εγγράφου που χρησιμοποιήθηκαν για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι `null`. Σημειώστε ότι αυτή η τιμή χρησιμοποιείται μόνο εάν το κείμενο του εγγράφου δεν αποθηκεύτηκε στο ευρετήριο. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα ανιχνεύεται η κωδικοποίηση αυτόματα ή όχι. Η προεπιλεγμένη τιμή είναι `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Λαμβάνει ή ορίζει το αντικείμενο ακύρωσης. Η προεπιλεγμένη τιμή είναι `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Λαμβάνει ή ορίζει τον προσαρμοσμένο εξαγωγέα κειμένου που χρησιμοποιήθηκε για την ευρετηρίαση. Η προεπιλεγμένη τιμή είναι `null`. Σημειώστε ότι αυτή η τιμή χρησιμοποιείται μόνο εάν το κείμενο του εγγράφου δεν αποθηκεύτηκε στο ευρετήριο. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Λαμβάνει ή ορίζει την κωδικοποίηση που χρησιμοποιείται για την εξαγωγή κειμένου από έγγραφα κειμένου. Η προεπιλεγμένη τιμή είναι `null`, που σημαίνει ότι χρησιμοποιείται η προεπιλεγμένη κωδικοποίηση UTF-8. Εάν το AutoDetectEncoding είναι `true`, τότε αυτή η τιμή χρησιμοποιείται ως προεπιλεγμένη κωδικοποίηση. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ετικέτα Head δημιουργείται στο παραγόμενο HTML. Η προεπιλεγμένη τιμή είναι `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Λαμβάνει ή ορίζει ένα χρώμα που χρησιμοποιείται για την επισήμανση εμφανίσεων. Η προεπιλεγμένη τιμή είναι #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Λαμβάνει τις επιλογές ευρετηρίασης εικόνας για αντίστροφη αναζήτηση εικόνας. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Λαμβάνει τις επιλογές για ευρετηρίαση πεδίων μεταδεδομένων. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Λαμβάνει τις επιλογές για επεξεργασία OCR και ευρετηρίαση του αναγνωρισμένου κειμένου. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Λαμβάνει ή ορίζει την ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης. Αυτή η ετικέτα χρησιμοποιείται μόνο όταν γίνεται επισήμανση σε απλό κείμενο. Η προεπιλεγμένη τιμή είναι μια κενή συμβολοσειρά. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Λαμβάνει ή ορίζει την ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης. Αυτή η ετικέτα χρησιμοποιείται μόνο όταν γίνεται επισήμανση σε απλό κείμενο. Η προεπιλεγμένη τιμή είναι μια κενή συμβολοσειρά. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Λαμβάνει ή ορίζει το μέγιστο αριθμό λέξεων σε ένα τμήμα κειμένου μετά την επισημασμένη λέξη. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Λαμβάνει ή ορίζει το μέγιστο αριθμό λέξεων σε ένα τμήμα κειμένου πριν την επισημασμένη λέξη. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Λαμβάνει ή ορίζει το μέγιστο αριθμό λέξεων σε ένα τμήμα κειμένου. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η διαδικασία πρέπει να χρησιμοποιεί το SeBackupPrivilege και το FILE_FLAG_BACKUP_SEMANTICS για πρόσβαση σε αρχεία και καταλόγους. Η προεπιλεγμένη τιμή είναι `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση εμφανίσεων. Η προεπιλεγμένη τιμή είναι `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν χρησιμοποιείται η ακατέργαστη λειτουργία για εξαγωγή κειμένου, εφόσον είναι δυνατόν. Η προεπιλεγμένη τιμή είναι `false`. Η ακατέργαστη λειτουργία μπορεί να αυξήσει σημαντικά την ταχύτητα ευρετηρίασης, αλλά η κανονική λειτουργία βελτιώνει τη μορφοποίηση του εξαγόμενου κειμένου. |

### Σχόλια

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Δείτε επίσης

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
