---
title: "EventHub"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει γεγονότα ευρετηρίου για εγγραφή."
type: docs
weight: 12
url: /el/java/com.groupdocs.search.events/eventhub/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public abstract class EventHub extends EventHubBase
```

Παρέχει γεγονότα ευρετηρίου για εγγραφή.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Αναζήτηση στο ευρετήριο
SearchResult result = index.search(query);
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [EventHub()](#EventHub--) |  |
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [OperationFinished](#OperationFinished) | Συμβαίνει όταν ολοκληρωθεί μια λειτουργία ευρετηρίου. |
|
|  | [ErrorOccurred](#ErrorOccurred) | Συμβαίνει όταν προκύψει σφάλμα κατά τη διάρκεια μιας λειτουργίας ευρετηρίου. |
|
|  | [OperationProgressChanged](#OperationProgressChanged) | Συμβαίνει όταν αλλάζει η πρόοδος της διαδικασίας ευρετηρίου ή ενημέρωσης. |
|
|  | [OptimizationProgressChanged](#OptimizationProgressChanged) | Συμβαίνει όταν αλλάζει η πρόοδος της διαδικασίας βελτιστοποίησης. |
|
|  | [PasswordRequired](#PasswordRequired) | Συμβαίνει όταν ένα έγγραφο απαιτεί κωδικό πρόσβασης για άνοιγμα. |
|
|  | [FileIndexing](#FileIndexing) | Συμβαίνει όταν ένα έγγραφο πρόκειται να ευρετηριαστεί. |
|
|  | [ImagePreparing](#ImagePreparing) | Συμβαίνει όταν μια εικόνα προετοιμάζεται για ευρετηρίαση. |
|
|  | [StatusChanged](#StatusChanged) | Συμβαίνει όταν η κατάσταση του ευρετηρίου αλλάζει. |
|
|  | [SearchPhaseCompleted](#SearchPhaseCompleted) | Συμβαίνει όταν η φάση αναζήτησης ολοκληρωθεί. |
|
### EventHub() {#EventHub--}
```
public EventHub()
```


### OperationFinished {#OperationFinished}
```
public final Event<EventHandler<OperationFinishedEventArgs>> OperationFinished
```


Συμβαίνει όταν ολοκληρωθεί μια λειτουργία ευρετηρίου.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().OperationFinished.add(new EventHandler() {
public void invoke(Object sender, OperationFinishedEventArgs args) {
System.out.println("Operation finished: " + args.getOperationType());
System.out.println("Μήνυμα: " + args.getMessage());
System.out.println("Φάκελος ευρετηρίου: " + args.getIndexFolder());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Ώρα: " + df.format(args.getTime()));
}
});
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
 
```
 
````



### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Συμβαίνει όταν προκύψει σφάλμα κατά τη διάρκεια μιας λειτουργίας ευρετηρίου.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().ErrorOccurred.add(new EventHandler() {
public void invoke(Object sender, IndexErrorEventArgs args) {
System.out.println(args.getMessage());
}
});
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Αναζήτηση στο ευρετήριο
SearchResult result = index.search(query);
 
```
 
````



### OperationProgressChanged {#OperationProgressChanged}
```
public final Event<EventHandler<OperationProgressEventArgs>> OperationProgressChanged
```


Συμβαίνει όταν αλλάζει η πρόοδος της διαδικασίας ευρετηρίου ή ενημέρωσης.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().OperationProgressChanged.add(new EventHandler() {
public void invoke(Object sender, OperationProgressEventArgs args) {
System.out.println("Τελευταία επεξεργασία: " + args.getLastDocumentPath());
System.out.println("Αποτέλεσμα: " + args.getLastDocumentStatus());
System.out.println("Επεξεργασμένα έγγραφα: " + args.getTotalDocuments());
System.out.println("Ποσοστό προόδου: " + args.getProgressPercentage());
}
});
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
 
```
 
````



### OptimizationProgressChanged {#OptimizationProgressChanged}
```
public final Event<EventHandler<OptimizationProgressEventArgs>> OptimizationProgressChanged
```


Συμβαίνει όταν αλλάζει η πρόοδος της διαδικασίας βελτιστοποίησης.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Συμβαίνει όταν ένα έγγραφο απαιτεί κωδικό πρόσβασης για άνοιγμα.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().PasswordRequired.add(new EventHandler() {
public void invoke(Object sender, PasswordRequiredEventArgs args) {
if (args.getDocumentFullPath().endsWith("ProtectedDocument.pdf")) {
args.setPassword("123456");
}
}
});
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
 
```
 
````



### FileIndexing {#FileIndexing}
```
public final Event<EventHandler<FileIndexingEventArgs>> FileIndexing
```


Συμβαίνει όταν ένα έγγραφο πρόκειται να ευρετηριαστεί.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().FileIndexing.add(new EventHandler() {
public void invoke(Object sender, FileIndexingEventArgs args) {
if (args.getDocumentFullPath().endsWith("Protected.pdf")) {
args.setAdditionalFields(new DocumentField[] {
new DocumentField("Tags", "Protected")
});
}
if (!args.getDocumentFullPath().toLowerCase().contains("σημαντικό")) {
args.setSkipIndexing(true);
}
}
});
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
 
```
 
````



### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Συμβαίνει όταν μια εικόνα προετοιμάζεται για ευρετηρίαση.


### StatusChanged {#StatusChanged}
```
public final Event<EventHandler<BaseIndexEventArgs>> StatusChanged
```


Συμβαίνει όταν η κατάσταση του ευρετηρίου αλλάζει.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().StatusChanged.add(new EventHandler() {
public void invoke(Object sender, BaseIndexEventArgs args) {
if (args.getStatus() != IndexStatus.InProgress) {
// Μια ειδοποίηση της ολοκλήρωσης της λειτουργίας θα πρέπει να είναι εδώ
}
}
});
// Ορισμός της σημαίας για ασύγχρονη ευρετηρίαση
IndexingOptions options = new IndexingOptions();
options.setAsync(true);
// Ασύγχρονη ευρετηρίαση εγγράφων από το καθορισμένο φάκελο
// Η μέθοδος τερματίζει πριν ολοκληρωθεί η λειτουργία
index.add(documentsFolder, options);
 
```
 
````



### SearchPhaseCompleted {#SearchPhaseCompleted}
```
public final Event<EventHandler<SearchPhaseEventArgs>> SearchPhaseCompleted
```


Συμβαίνει όταν η φάση αναζήτησης ολοκληρωθεί.

Το παράδειγμα δείχνει πώς να χρησιμοποιήσετε το συμβάν.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Γίνεται εγγραφή στο συμβάν
index.getEvents().SearchPhaseCompleted.add(new EventHandler() {
public void invoke(Object sender, SearchPhaseEventArgs args) {
System.out.println("Search phase: " + args.getSearchPhase());
System.out.println("Words: " + args.getWords().length);
}
});
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true);
options.setUseWordFormsSearch(true);
options.getFuzzySearch().setEnabled(true);
options.setUseHomophoneSearch(true);
SearchResult result = index.search("Einstein", options);
 
```
 
````



