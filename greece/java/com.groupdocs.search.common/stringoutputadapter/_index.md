---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο ως System.String."
type: docs
weight: 32
url: /el/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο ως ένα  System.String .


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.add(documentsFolder); // Καταχώρηση εγγράφων από τον καθορισμένο φάκελο
DocumentInfo[] documents = index.getIndexedDocuments(); // Λήψη πληροφοριών για τα ευρετηριασμένα έγγραφα
StringOutputAdapter adapter = new StringOutputAdapter(); // Δημιουργία προσαρμογέα εξόδου συμβολοσειράς
index.getDocumentText(documents[0], adapter); // Δημιουργία κειμένου εγγράφου στον προσαρμογέα
String result = adapter.getResult(); // Λήψη αποτελέσματος
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Αρχικοποιεί μια νέα παρουσία της  StringOutputAdapter  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getResult()](#getResult--) | Λαμβάνει τη δημιουργημένη συμβολοσειρά. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Αρχικοποιεί μια νέα παρουσία της  StringOutputAdapter  κλάσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Η μορφή εξόδου. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Λαμβάνει τη δημιουργημένη συμβολοσειρά.


**Returns:**
java.lang.String - Η δημιουργημένη συμβολοσειρά.

