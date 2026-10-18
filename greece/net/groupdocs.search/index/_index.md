---
title: "Index"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Αντιπροσωπεί την κύρια κλάση για την ευρετηρίαση εγγράφων και την αναζήτηση σε αυτά."
type: docs
weight: 700
url: /el/net/groupdocs.search/index/
---
## Index class

Αντιπροσωπεί την κύρια κλάση για την ευρετηρίαση εγγράφων και την αναζήτηση σε αυτά.

```csharp
public class Index : IDisposable
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [Index](index#constructor)() | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../index) στη μνήμη. |
| [Index](index#constructor_1)(IndexSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../index) στη μνήμη με συγκεκριμένες ρυθμίσεις ευρετηρίου. |
| [Index](index#constructor_2)(string) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../index). Δημιουργεί ένα νέο ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο. |
| [Index](index#constructor_3)(string, bool) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../index). Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν η *overwriteIfExists* είναι `false`; δημιουργεί ένα νέο ευρετήριο στο δίσκο διαφορετικά. |
| [Index](index#constructor_4)(string, IndexSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../index). Δημιουργεί ένα νέο ευρετήριο με συγκεκριμένες ρυθμίσεις ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../index). Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν *overwriteIfExists* είναι `false`; δημιουργεί ένα νέο ευρετήριο στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου διαφορετικά. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Λαμβάνει το αποθετήριο λεξικού. |
| [Events](../../groupdocs.search/index/events) { get; } | Λαμβάνει το κέντρο γεγονότων για εγγραφή σε γεγονότα. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Λαμβάνει τις βασικές πληροφορίες για το ευρετήριο. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Λαμβάνει τις ρυθμίσεις του ευρετηρίου. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Λαμβάνει το αντικείμενο αποθετηρίου ευρετηρίου εάν το ευρετήριο περιέχεται σε αυτό. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Φορτώνει ολόκληρο το ευρετήριο στη μνήμη. Οποιεσδήποτε αλλαγές στο ευρετήριο δεν αποθηκεύονται αυτόματα στο αρχικό φάκελο. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Φορτώνει ολόκληρο το ευρετήριο στη μνήμη. Οποιεσδήποτε αλλαγές στο ευρετήριο δεν αποθηκεύονται αυτόματα στο αρχικό φάκελο. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Εκτελεί λειτουργία ευρετηρίου. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Εκτελεί λειτουργία ευρετηρίου. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Εκτελεί λειτουργία ευρετηρίου. Προσθέτει έγγραφα από σύστημα αρχείων, ροή ή δομή. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Εκτελεί λειτουργία ευρετηρίου. Προσθέτει τα εξαγόμενα δεδομένα στο ευρετήριο. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Εκτελεί λειτουργία ευρετηρίου. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Εκτελεί λειτουργία ευρετηρίου. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Εφαρμόζει το καθορισμένο πακέτο αλλαγών χαρακτηριστικών στα ευρετηριασμένα έγγραφα χωρίς επανευρετηρίαση κατά τη λειτουργία ενημέρωσης. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Ελέγχει το ευρετήριο για κατεστραμμένα αρχεία τμημάτων στο δίσκο. Η μέθοδος διορθώνει τη λειτουργικότητα του ευρετηρίου παρουσία κατεστραμμένων τμημάτων, εάν *fixIndexFunctionality* είναι true· δεν διορθώνει - διαφορετικά. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Διαγράφει τα ευρετηριασμένα αρχεία ή φακέλους από το ευρετήριο. Στη συνέχεια ενημερώνει το ευρετήριο χωρίς τις διαγραμμένες διαδρομές. Σημειώστε ότι ένα μεμονωμένο έγγραφο δεν μπορεί να διαγραφεί από το ευρετήριο εάν προστέθηκε στο ευρετήριο ως μέρος φακέλου. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Διαγράφει έγγραφα που ευρετηριάστηκαν από ροές ή δομές. Στη συνέχεια ενημερώνει το ευρετήριο χωρίς τα διαγραμμένα έγγραφα. |
| [Dispose](../../groupdocs.search/index/dispose)() | Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Λαμβάνει όλα τα χαρακτηριστικά που σχετίζονται με το καθορισμένο ευρετηριασμένο έγγραφο. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Δημιουργεί το κείμενο ενός ευρετηριασμένου εγγράφου και το περνά μέσω ενός προσαρμογέα εξόδου. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Δημιουργεί κείμενο μορφοποιημένο σε HTML για το ευρετηριασμένο έγγραφο και το μεταφέρει μέσω του προσαρμογέα εξόδου. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Λαμβάνει ένα ευρετηριασμένο έγγραφο με κλειδί εγγράφου. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Λαμβάνει έναν πίνακα με ένθετα στοιχεία του καθορισμένου εγγράφου (για έγγραφα κοντέινερ όπως ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Λαμβάνει έναν πίνακα με όλα τα ευρετηριασμένα έγγραφα. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Λαμβάνει έναν πίνακα με ευρετηριασμένες διαδρομές - έγγραφα ή φακέλους. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Λαμβάνει τις αναφορές για τις λειτουργίες ευρετηρίου. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Λαμβάνει τις αναφορές για τις λειτουργίες αναζήτησης. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Δημιουργεί κείμενο μορφοποιημένο σε HTML με επισημασμένους εντοπισμένους όρους. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Συγχωνεύει το καθορισμένο ευρετήριο στο τρέχον ευρετήριο. Σημειώστε ότι το άλλο ευρετήριο δεν θα αλλάξει. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Συγχωνεύει ευρετήρια από το καθορισμένο αποθετήριο ευρετηρίων στο τρέχον ευρετήριο. Σημειώστε ότι τα ευρετήρια στο αποθετήριο δεν θα αλλάξουν. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Περνά το καθορισμένο αντικείμενο ειδοποίησης στο ευρετήριο για να εκτελέσει την ειδοποίηση. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους. Αυτή η λειτουργία βελτιώνει την απόδοση της αναζήτησης. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Μειώνει τον αριθμό των τμημάτων του ευρετηρίου συγχωνεύοντάς τα μεταξύ τους. Αυτή η λειτουργία βελτιώνει την απόδοση της αναζήτησης. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Αποθηκεύει το ευρετήριο στη μνήμη στο δίσκο. Επίσης αποθηκεύει το κανονικό ευρετήριο σε άλλο φάκελο. Δεν αλλάζει τις ρυθμίσεις αυτού του ευρετηρίου. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Αναζητά στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Αναζητά στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Εκτελεί αντίστροφη αναζήτηση εικόνας στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Αναζητά στο ευρετήριο. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Αναζητά στο ευρετήριο. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Συνεχίζει την αναζήτηση τμημάτων που ξεκίνησε με τη μέθοδο Search. |
| [Update](../../groupdocs.search/index/update#update)() | Επαναευρετηρίζει έγγραφα που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φάκελους που έχουν ευρετηριαστεί. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Επαναευρετηρίζει έγγραφα που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φάκελους που έχουν ευρετηριαστεί. |

### Σχόλια

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Παραδείγματα

Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Δείτε επίσης

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
