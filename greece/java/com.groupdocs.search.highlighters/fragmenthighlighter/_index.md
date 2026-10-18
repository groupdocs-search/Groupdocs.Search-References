---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν επισημαστικό αποτελεσμάτων αναζήτησης που επισημαίνει τα αποτελέσματα αναζήτησης σε αποσπάσματα κειμένου."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

Αντιπροσωπεύει έναν επισημαστικό αποτελεσμάτων αναζήτησης που επισημαίνει τα αποτελέσματα αναζήτησης σε αποσπάσματα κειμένου.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ενός δείκτη
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Αναζήτηση για τη λέξη 'Einstein'
SearchResult result = index.search("Einstein");
// Ανάθεση επιλογών επισήμανσης
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// Επισήμανση των ευρεθέντων λέξεων στο κείμενο ενός εγγράφου
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// Λήψη του αποτελέσματος
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// Εκτύπωση του HTML markup στην κονσόλα
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  FragmentHighlighter  . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getResult()](#getResult--) | Λαμβάνει έναν πίνακα των fragment containers που προκύπτουν. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  FragmentHighlighter  .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Η μορφή εξόδου. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


Λαμβάνει έναν πίνακα των fragment containers που προκύπτουν.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - Ένας πίνακας των fragment containers που προκύπτουν.

