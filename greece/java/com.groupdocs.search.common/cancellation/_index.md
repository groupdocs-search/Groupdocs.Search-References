---
title: "Ακύρωση"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά ένα αντικείμενο για αίτηση ακύρωσης μιας λειτουργίας."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Αναπαριστά ένα αντικείμενο για αίτηση ακύρωσης μιας λειτουργίας.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Αρχικοποιεί μια νέα παρουσία της |
Ακύρωση
κλάσης.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Λαμβάνει μια τιμή που υποδεικνύει ότι έχει ζητηθεί η ακύρωση. |
|
|  | [cancel()](#cancel--) | Κάνει αίτηση για ακύρωση. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Κάνει αίτηση για ακύρωση μετά τη λήξη του καθορισμένου αριθμού χιλιοστών του δευτερολέπτου. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Αρχικοποιεί μια νέα παρουσία της
Ακύρωση
κλάσης.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Λαμβάνει μια τιμή που υποδεικνύει ότι έχει ζητηθεί η ακύρωση.


**Returns:**
boolean - Μια τιμή που υποδεικνύει ότι έχει ζητηθεί η ακύρωση.

### cancel() {#cancel--}
```
public final void cancel()
```


Κάνει αίτηση για ακύρωση.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Κάνει αίτηση για ακύρωση μετά τη λήξη του καθορισμένου αριθμού χιλιοστών του δευτερολέπτου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | χιλιοστά του δευτερολέπτου | int | Ο αριθμός των χιλιοστών του δευτερολέπτου μετά τον οποίο μια λειτουργία θα ακυρωθεί. |
|

