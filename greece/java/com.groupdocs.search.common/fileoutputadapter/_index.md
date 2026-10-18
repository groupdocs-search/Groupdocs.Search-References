---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά έναν προσαρμογέα εξόδου που συλλέγει την έξοδο σε αρχείο."
type: docs
weight: 21
url: /el/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Αναπαριστά έναν προσαρμογέα εξόδου που συλλέγει την έξοδο σε αρχείο.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Δημιουργία προσαρμογέα εξόδου αρχείου
index.getDocumentText(documents[0], adapter); // Δημιουργία κειμένου εγγράφου στο αρχείο εξόδου
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της  FileOutputAdapter  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Λαμβάνει διαδρομή αρχείου εξόδου. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Αρχικοποιεί μια νέα παρουσία της  FileOutputAdapter  κλάσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Η μορφή εξόδου. |
|
|  | filePath | java.lang.String | Η διαδρομή αρχείου εξόδου. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Λαμβάνει διαδρομή αρχείου εξόδου.


**Returns:**
java.lang.String - Η διαδρομή αρχείου εξόδου.

