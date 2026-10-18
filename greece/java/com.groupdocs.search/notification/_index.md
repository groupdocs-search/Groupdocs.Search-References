---
title: "Ειδοποίηση"
second_title: "GroupDocs.Search για Java API Reference"
description: "Η βασική κλάση για όλες τις ειδοποιήσεις προς το ευρετήριο."
type: docs
weight: 22
url: /el/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

Η βασική κλάση για όλες τις ειδοποιήσεις προς το ευρετήριο. Αυτή η κλάση περιέχει επίσης μεθόδους για τη δημιουργία αντικειμένων ειδοποίησης.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Notification()](#Notification--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Δημιουργεί ένα αντικείμενο ειδοποίησης για τη μετονομασία ενός ευρετηριασμένου εγγράφου που έχει μετονομαστεί και δεν χρειάζεται να επαναευρετηριστεί. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Δημιουργεί ένα αντικείμενο ειδοποίησης για τη μετονομασία ενός ευρετηριασμένου εγγράφου που έχει μετονομαστεί και δεν χρειάζεται να επαναευρετηριστεί. Το μετονομασμένο έγγραφο δεν θα επαναευρετηριστεί κατά την επόμενη λειτουργία ενημέρωσης, ακόμη και αν τα περιεχόμενά του έχουν αλλάξει.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | oldPath | java.lang.String | Η παλιά διαδρομή προς το ευρετηριασμένο έγγραφο. |
|
|  | newPath | java.lang.String | Η νέα διαδρομή προς το ευρετηριασμένο έγγραφο. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

