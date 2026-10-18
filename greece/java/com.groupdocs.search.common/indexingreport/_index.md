---
title: "IndexingReport"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά λεπτομερείς πληροφορίες για μια λειτουργία ευρετηρίασης."
type: docs
weight: 25
url: /el/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Αναπαριστά λεπτομερείς πληροφορίες για μια λειτουργία ευρετηρίασης.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
Index index = new Index(indexFolder);
// Ευρετηρίαση εγγράφων
index.add(documentsFolder1);
index.add(documentsFolder2);
// Λήψη αναφορών ευρετηρίου
IndexingReport[] reports = index.getIndexingReports();
// Εκτύπωση αναφορών στην κονσόλα
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Ώρα: " + df.format(report.getStartTime()));
System.out.println("Διάρκεια: " + report.getIndexingTime());
System.out.println("Συνολικά έγγραφα: " + report.getTotalDocumentsInIndex());
System.out.println("Συνολικοί όροι: " + report.getTotalTermCount());
System.out.println("Μέγεθος ευρετηριασμένων εγγράφων (MB): " + report.getIndexedDocumentsSize());
System.out.println("Μέγεθος ευρετηρίου (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Λαμβάνει τον συνολικό αριθμό εγγράφων στο ευρετήριο. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Λαμβάνει τον συνολικό αριθμό όρων στο ευρετήριο. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Λαμβάνει το συνολικό μήκος των ευρετηριασμένων εγγράφων σε MB. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Λαμβάνει τον αριθμό των τμημάτων του ευρετηρίου. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Λαμβάνει το συνολικό μέγεθος του ευρετηρίου σε byte. |
|
|  | [getStartTime()](#getStartTime--) | Λαμβάνει την ώρα έναρξης της ευρετηρίασης. |
|
|  | [getEndTime()](#getEndTime--) | Λαμβάνει την ώρα λήξης της ευρετηρίασης. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Λαμβάνει τη διάρκεια της ευρετηρίασης σε δευτερόλεπτα. |
|
|  | [getErrors()](#getErrors--) | Λαμβάνει τη λίστα σφαλμάτων. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Λαμβάνει τη λίστα των ευρετηριασμένων εγγράφων. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Λαμβάνει τη λίστα των ενημερωμένων εγγράφων. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Λαμβάνει τη λίστα των εγγράφων που αφαιρέθηκαν από το ευρετήριο. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Λαμβάνει τον συνολικό αριθμό εγγράφων στο ευρετήριο.


**Returns:**
int - Συνολικός αριθμός εγγράφων στο ευρετήριο.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Λαμβάνει τον συνολικό αριθμό όρων στο ευρετήριο.


**Returns:**
int - Συνολικός αριθμός όρων στο ευρετήριο.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Λαμβάνει το συνολικό μήκος των ευρετηριασμένων εγγράφων σε MB.


**Returns:**
double - Συνολικό μήκος των ευρετηριασμένων εγγράφων σε MB.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Λαμβάνει τον αριθμό των τμημάτων του ευρετηρίου.


**Returns:**
int - Ο αριθμός των τμημάτων του ευρετηρίου.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Λαμβάνει το συνολικό μέγεθος του ευρετηρίου σε byte.


**Returns:**
long - Συνολικό μέγεθος ευρετηρίου σε bytes.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Λαμβάνει την ώρα έναρξης της ευρετηρίασης.


**Returns:**
java.util.Date - Η ώρα έναρξης της ευρετηρίασης.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Λαμβάνει την ώρα λήξης της ευρετηρίασης.


**Returns:**
java.util.Date - Η ώρα λήξης της ευρετηρίασης.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Λαμβάνει τη διάρκεια της ευρετηρίασης σε δευτερόλεπτα.


**Returns:**
double - Διάρκεια ευρετηρίασης σε δευτερόλεπτα.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Λαμβάνει τη λίστα σφαλμάτων.


**Returns:**
java.lang.String[] - Η λίστα των σφαλμάτων.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Λαμβάνει τη λίστα των ευρετηριασμένων εγγράφων.


**Returns:**
java.lang.String[] - Η λίστα των ευρετηριασμένων εγγράφων.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Λαμβάνει τη λίστα των ενημερωμένων εγγράφων.


**Returns:**
java.lang.String[] - Η λίστα των ενημερωμένων εγγράφων.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Λαμβάνει τη λίστα των εγγράφων που αφαιρέθηκαν από το ευρετήριο.


**Returns:**
java.lang.String[] - Η λίστα των εγγράφων που αφαιρέθηκαν από το ευρετήριο.

