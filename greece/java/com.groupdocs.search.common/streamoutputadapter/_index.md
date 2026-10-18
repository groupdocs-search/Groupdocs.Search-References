---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο σε ένα java.io.OutputStream."
type: docs
weight: 31
url: /el/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο σε ένα  java.io.OutputStream .


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // Δημιουργία ροής εξόδου
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Δημιουργία προσαρμογέα εξόδου ροής
index.getDocumentText(documents[0], adapter); // Δημιουργία κειμένου εγγράφου στη ροή
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  StreamOutputAdapter  . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getStream()](#getStream--) | Λαμβάνει μια ροή εξόδου. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  StreamOutputAdapter  .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Η μορφή εξόδου. |
|
|  | ροή | java.io.OutputStream | Η ροή εξόδου. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Λαμβάνει μια ροή εξόδου.


**Returns:**
java.io.OutputStream - Η ροή εξόδου.

