---
title: "MergeOptions"
second_title: "GroupDocs.Search για Java API Reference"
description: "Παρέχει επιλογές για τη λειτουργία συγχώνευσης."
type: docs
weight: 28
url: /el/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Παρέχει επιλογές για τη λειτουργία συγχώνευσης.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  MergeOptions . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isAsync()](#isAsync--) | Λαμβάνει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Ορίζει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. |
|
|  | [getCancellation()](#getCancellation--) | Λαμβάνει το αντικείμενο ακύρωσης της λειτουργίας. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Ορίζει το αντικείμενο ακύρωσης της λειτουργίας. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης  MergeOptions .


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Λαμβάνει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  false .


**Returns:**
boolean - Η σημαία της ασύγχρονης εκτέλεσης της λειτουργίας.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Ορίζει τη σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  false .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | τιμή | boolean | Η σημαία της ασύγχρονης εκτέλεσης της λειτουργίας. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Λαμβάνει το αντικείμενο ακύρωσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Ορίζει το αντικείμενο ακύρωσης της λειτουργίας. Η προεπιλεγμένη τιμή είναι  null .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Το αντικείμενο ακύρωσης της λειτουργίας. |
|

