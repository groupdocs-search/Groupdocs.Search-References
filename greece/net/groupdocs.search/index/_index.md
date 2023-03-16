---
title: Index
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αντιπροσωπεύει την κύρια τάξη για την ευρετηρίαση εγγράφων και την αναζήτηση μέσω αυτών.
type: docs
weight: 680
url: /el/net/groupdocs.search/index/
---
## Index class

Αντιπροσωπεύει την κύρια τάξη για την ευρετηρίαση εγγράφων και την αναζήτηση μέσω αυτών.

```csharp
public class Index : IDisposable
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [Index](index#constructor)() | Αρχικοποιεί μια νέα παρουσία του[`Index`](../index) τάξη στη μνήμη. |
| [Index](index#constructor_1)(IndexSettings) | Αρχικοποιεί μια νέα παρουσία του[`Index`](../index) κλάση στη μνήμη με συγκεκριμένες ρυθμίσεις ευρετηρίου. |
| [Index](index#constructor_2)(string) | Αρχικοποιεί μια νέα παρουσία του[`Index`](../index) class. Δημιουργεί ένα νέο ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο. |
| [Index](index#constructor_3)(string, bool) | Αρχικοποιεί μια νέα παρουσία του[`Index`](../index) class. Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν*overwriteIfExists* είναι`ψευδής`; δημιουργεί ένα νέο ευρετήριο στο δίσκο διαφορετικά. |
| [Index](index#constructor_4)(string, IndexSettings) | Αρχικοποιεί μια νέα παρουσία του[`Index`](../index) class. Δημιουργεί ένα νέο ευρετήριο με συγκεκριμένες ρυθμίσεις ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Αρχικοποιεί μια νέα παρουσία του[`Index`](../index) class. Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν*overwriteIfExists* είναι`ψευδής` ; δημιουργεί ένα νέο ευρετήριο στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου διαφορετικά. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Παίρνει το αποθετήριο λεξικών. |
| [Events](../../groupdocs.search/index/events) { get; } | Αποκτά το κέντρο εκδηλώσεων για εγγραφή σε εκδηλώσεις. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Λαμβάνει τις βασικές πληροφορίες για το ευρετήριο. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Λαμβάνει τις ρυθμίσεις ευρετηρίου. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Λαμβάνει το αντικείμενο αποθήκης ευρετηρίου εάν το ευρετήριο περιέχεται σε αυτό. |

## Μέθοδοι

| Ονομα | Περιγραφή |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει έγγραφα από σύστημα αρχείων, ροή ή δομή. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει τα εξαγόμενα δεδομένα στο ευρετήριο. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Εφαρμόζει την καθορισμένη δέσμη αλλαγών χαρακτηριστικών σε έγγραφα με ευρετήριο χωρίς εκ νέου ευρετηρίαση κατά τη λειτουργία ενημέρωσης. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Διαγράφει αρχεία ή φακέλους με ευρετήριο από το ευρετήριο. Στη συνέχεια ενημερώνει το ευρετήριο χωρίς διαγραμμένες διαδρομές. Σημειώστε ότι ένα μεμονωμένο έγγραφο δεν μπορεί να διαγραφεί από το ευρετήριο εάν προστέθηκε στο ευρετήριο ως μέρος ενός φακέλου. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Διαγράφει έγγραφα που έχουν ευρετηριαστεί από ροές ή δομές. Στη συνέχεια ενημερώνει το ευρετήριο χωρίς διαγραμμένα έγγραφα. |
| [Dispose](../../groupdocs.search/index/dispose)() | Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Λαμβάνει όλα τα χαρακτηριστικά που σχετίζονται με το καθορισμένο έγγραφο με ευρετήριο. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Δημιουργεί κείμενο μορφοποιημένου HTML για έγγραφο με ευρετήριο και το μεταφέρει μέσω του προσαρμογέα εξόδου. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Δημιουργεί κείμενο μορφοποιημένου HTML για έγγραφο με ευρετήριο και το μεταφέρει μέσω του προσαρμογέα εξόδου. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Λαμβάνει μια σειρά από ένθετα στοιχεία του καθορισμένου εγγράφου (για έγγραφα κοντέινερ όπως ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Λαμβάνει μια σειρά από όλα τα ευρετηριασμένα έγγραφα. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Λαμβάνει μια σειρά από μονοπάτια με ευρετήριο - έγγραφα ή φακέλους. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Λαμβάνει τις αναφορές για τις λειτουργίες ευρετηρίασης. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Λαμβάνει τις αναφορές για τις λειτουργίες αναζήτησης. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Δημιουργεί κείμενο μορφοποιημένου HTML με επισημασμένους όρους που βρέθηκαν. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Δημιουργεί κείμενο μορφοποιημένου HTML με επισημασμένους όρους που βρέθηκαν. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Συγχωνεύει το καθορισμένο ευρετήριο στο τρέχον ευρετήριο. Σημειώστε ότι το άλλο ευρετήριο δεν θα αλλάξει. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Συγχωνεύει ευρετήρια από το καθορισμένο χώρο αποθήκευσης ευρετηρίου στο τρέχον ευρετήριο. Σημειώστε ότι τα ευρετήρια στο χώρο αποθήκευσης δεν θα αλλάξουν. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Μεταβιβάζει το καθορισμένο αντικείμενο ειδοποίησης στο ευρετήριο για την εκτέλεση της ειδοποίησης. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Ελαχιστοποιεί τον αριθμό των τμημάτων ευρετηρίου συγχωνεύοντάς τα το ένα με το άλλο. Αυτή η λειτουργία βελτιώνει την απόδοση αναζήτησης. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Ελαχιστοποιεί τον αριθμό των τμημάτων ευρετηρίου συγχωνεύοντάς τα το ένα με το άλλο. Αυτή η λειτουργία βελτιώνει την απόδοση αναζήτησης. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Αναζητήσεις στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Αναζητήσεις στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Εκτελεί αντίστροφη αναζήτηση εικόνας στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Αναζητήσεις στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Αναζητήσεις στο ευρετήριο. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Αναζήτηση. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Αναζήτηση. |
| [Update](../../groupdocs.search/index/update#update)() | Δημιουργεί εκ νέου ευρετήριο εγγράφων που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φακέλους ευρετηρίου. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Δημιουργεί εκ νέου ευρετήριο εγγράφων που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φακέλους ευρετηρίου. |

### Παρατηρήσεις

**Μάθε περισσότερα**

* [Δημιουργία ευρετηρίου](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Ευρετηρίαση](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Ερευνητικός](https://docs.groupdocs.com/display/searchnet/Searching)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

SearchResult result = index.Search(query); // Αναζήτηση στο ευρετήριο
```

### Δείτε επίσης

* χώρος ονομάτων [GroupDocs.Search](../../groupdocs.search)
* συνέλευση [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
