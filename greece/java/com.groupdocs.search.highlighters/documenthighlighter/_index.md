---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν επισημαστικό αποτελεσμάτων αναζήτησης που επισημαίνει τα αποτελέσματα αναζήτησης σε ολόκληρο το κείμενο του εγγράφου."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

Αντιπροσωπεύει έναν επισημαστικό αποτελεσμάτων αναζήτησης που επισημαίνει τα αποτελέσματα αναζήτησης σε ολόκληρο το κείμενο του εγγράφου.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Αναζήτηση για τη φράση 'Theory of Relativity'
SearchResult result = index.search("\"Theory of Relativity\"");
// Επισήμανση των ευρεθέντων λέξεων στο κείμενο ενός εγγράφου
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | Αρχικοποιεί μια νέα παρουσία της κλάσης DocumentHighlighter. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | Λαμβάνει τον προσαρμογέα εξόδου που περάστηκε στον κατασκευαστή. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης DocumentHighlighter.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Ο προσαρμογέας εξόδου που μεταφέρει το αποτέλεσμα της επισήμανσης. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


Λαμβάνει τον προσαρμογέα εξόδου που περάστηκε στον κατασκευαστή.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

