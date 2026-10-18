---
title: "HighlightOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για την επισήμανση των ευρεθέντων όρων."
type: docs
weight: 22
url: /el/java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Παρέχει επιλογές για την επισήμανση των ευρεθέντων όρων.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [HighlightOptions()](#HighlightOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης HighlightOptions. |
|
|  | [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Αρχικοποιεί μια νέα παρουσία της κλάσης TextOptions. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getTermsBefore()](#getTermsBefore--) | Λαμβάνει τον μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου πριν τη επισημασμένη λέξη. |
|
|  | [setTermsBefore(int value)](#setTermsBefore-int-) | Ορίζει τον μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου πριν τη επισημασμένη λέξη. |
|
|  | [getTermsAfter()](#getTermsAfter--) | Λαμβάνει τον μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου μετά τη επισημασμένη λέξη. |
|
|  | [setTermsAfter(int value)](#setTermsAfter-int-) | Ορίζει τον μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου μετά τη επισημασμένη λέξη. |
|
|  | [getTermsTotal()](#getTermsTotal--) | Λαμβάνει τον μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου. |
|
|  | [setTermsTotal(int value)](#setTermsTotal-int-) | Ορίζει τον μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου. |
|
|  | [getUseInlineStyles()](#getUseInlineStyles--) | Λαμβάνει μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση εμφανίσεων. |
|
|  | [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση εμφανίσεων. |
|
|  | [getHighlightColor()](#getHighlightColor--) | Λαμβάνει ένα χρώμα που χρησιμοποιείται για την επισήμανση εμφανίσεων. |
|
|  | [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Ορίζει ένα χρώμα που χρησιμοποιείται για την επισήμανση των εμφανίσεων. |
|
|  | [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Λαμβάνει την ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης. |
|
|  | [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Ορίζει την ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης. |
|
|  | [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Λαμβάνει την ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης. |
|
|  | [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Ορίζει την ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης. |
|
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης HighlightOptions.


### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης TextOptions.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | δεδομένα | java.lang.Object | Τα σειριοποιημένα δεδομένα. |
|

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Λαμβάνει το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου πριν από τη επισημασμένη λέξη. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι 7.


**Returns:**
int - Το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου πριν από τη επισημασμένη λέξη.

### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Ορίζει το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου πριν από τη επισημασμένη λέξη. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι 7.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου πριν από τη επισημασμένη λέξη. |
|

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Λαμβάνει το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου μετά τη επισημασμένη λέξη. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι 7.


**Returns:**
int - Το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου μετά τη επισημασμένη λέξη.

### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Ορίζει το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου μετά τη επισημασμένη λέξη. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι 7.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου μετά τη επισημασμένη λέξη. |
|

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Λαμβάνει το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι 21.


**Returns:**
int - Το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου.

### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Ορίζει το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου. Η τιμή πρέπει να βρίσκεται στο εύρος από 0 έως 10000. Η προεπιλεγμένη τιμή είναι 21.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | int | Το μέγιστο αριθμό λέξεων σε ένα απόσπασμα κειμένου. |
|

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση των εμφανίσεων. Η προεπιλεγμένη τιμή είναι true.


**Returns:**
boolean - Μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση των εμφανίσεων.

### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση των εμφανίσεων. Η προεπιλεγμένη τιμή είναι true.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Μια τιμή που υποδεικνύει εάν χρησιμοποιούνται ενσωματωμένα στυλ για την επισήμανση των εμφανίσεων. |
|

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Λαμβάνει ένα χρώμα που χρησιμοποιείται για την επισήμανση των εμφανίσεων. Η προεπιλεγμένη τιμή είναι #FFD800.


**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.

### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Ορίζει ένα χρώμα που χρησιμοποιείται για την επισήμανση των εμφανίσεων. Η προεπιλεγμένη τιμή είναι #FFD800.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [Color](../../com.groupdocs.search.options/color) | Ένα χρώμα που χρησιμοποιείται για την επισήμανση εμφανίσεων. |
|

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Λαμβάνει την ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης. Αυτή η ετικέτα χρησιμοποιείται μόνο όταν η επισήμανση γίνεται σε απλό κείμενο. Η προεπιλεγμένη τιμή είναι μια κενή συμβολοσειρά.


**Returns:**
java.lang.String - Η ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης.

### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Ορίζει την ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης. Αυτή η ετικέτα χρησιμοποιείται μόνο όταν η επισήμανση γίνεται σε απλό κείμενο. Η προεπιλεγμένη τιμή είναι μια κενή συμβολοσειρά.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Η ετικέτα έναρξης της επισήμανσης της ευρεθείσας λέξης. |
|

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Λαμβάνει την ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης. Αυτή η ετικέτα χρησιμοποιείται μόνο όταν η επισήμανση γίνεται σε απλό κείμενο. Η προεπιλεγμένη τιμή είναι μια κενή συμβολοσειρά.


**Returns:**
java.lang.String - Η ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης.

### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Ορίζει την ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης. Αυτή η ετικέτα χρησιμοποιείται μόνο όταν η επισήμανση γίνεται σε απλό κείμενο. Η προεπιλεγμένη τιμή είναι μια κενή συμβολοσειρά.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | java.lang.String | Η ετικέτα λήξης της επισήμανσης της ευρεθείσας λέξης. |
|

