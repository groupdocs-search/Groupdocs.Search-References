---
title: "SearchReport"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει λεπτομερείς πληροφορίες σχετικά με μια λειτουργία αναζήτησης."
type: docs
weight: 30
url: /el/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Αντιπροσωπεύει λεπτομερείς πληροφορίες σχετικά με μια λειτουργία αναζήτησης.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Καταχώριση εγγράφων από τον καθορισμένο φάκελο
index.add(documentsFolder);
// Αναζήτηση στο ευρετήριο
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Λήψη αναφορών αναζήτησης
SearchReport[] reports = index.getSearchReports();
// Εκτύπωση αναφορών στην κονσόλα
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Ώρα: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Λαμβάνει την ώρα έναρξης της αναζήτησης. |
|
|  | [getEndTime()](#getEndTime--) | Λαμβάνει την ώρα λήξης της αναζήτησης. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Λαμβάνει τη διάρκεια της αναζήτησης σε δευτερόλεπτα. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Λαμβάνει τον αριθμό των εγγράφων που βρέθηκαν. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Λαμβάνει τον συνολικό αριθμό των εμφανίσεων που βρέθηκαν. |
|
|  | [getTextQuery()](#getTextQuery--) | Λαμβάνει το ερώτημα αναζήτησης σε μορφή κειμένου. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Λαμβάνει το ερώτημα αναζήτησης σε μορφή αντικειμένου. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Λαμβάνει τις επιλογές αναζήτησης. |
|
|  | [toString()](#toString--) | Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον SearchReport. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Λαμβάνει την ώρα έναρξης της αναζήτησης.


**Returns:**
java.util.Date - Η ώρα έναρξης της αναζήτησης.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Λαμβάνει την ώρα λήξης της αναζήτησης.


**Returns:**
java.util.Date - Η ώρα λήξης της αναζήτησης.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Λαμβάνει τη διάρκεια της αναζήτησης σε δευτερόλεπτα.


**Returns:**
double - Η διάρκεια της αναζήτησης σε δευτερόλεπτα.

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Λαμβάνει τον αριθμό των εγγράφων που βρέθηκαν.


**Returns:**
int - Ο αριθμός των εγγράφων που βρέθηκαν.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Λαμβάνει τον συνολικό αριθμό των εμφανίσεων που βρέθηκαν.


**Returns:**
int - Ο συνολικός αριθμός των εμφανίσεων που βρέθηκαν.

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Λαμβάνει το ερώτημα αναζήτησης σε μορφή κειμένου.


**Returns:**
java.lang.String - Η ερώτηση αναζήτησης σε μορφή κειμένου.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Λαμβάνει το ερώτημα αναζήτησης σε μορφή αντικειμένου.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Λαμβάνει τις επιλογές αναζήτησης.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει ένα String που αντιπροσωπεύει το τρέχον SearchReport.


**Returns:**
java.lang.String - Μια συμβολοσειρά που αντιπροσωπεύει το τρέχον SearchReport.

