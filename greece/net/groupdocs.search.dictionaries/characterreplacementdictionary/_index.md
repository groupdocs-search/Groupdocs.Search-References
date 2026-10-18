---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Αντιπροσωπεύει ένα λεξικό αντικατάστασης χαρακτήρων που χρησιμοποιείται κατά τη διαδικασία ευρετηρίασης. Η αντικατάσταση χαρακτήρων μπορεί, για παράδειγμα, να χρησιμοποιηθεί για την αφαίρεση τόνων από τονισμένους χαρακτήρες ή για τη δημιουργία ευρετηρίου χωρίς διάκριση πεζών-κεφαλαίων."
type: docs
weight: 390
url: /el/net/groupdocs.search.dictionaries/characterreplacementdictionary/
---
## CharacterReplacementDictionary class

Αντιπροσωπεύει ένα λεξικό αντικατάστασης χαρακτήρων που χρησιμοποιείται κατά τη διαδικασία ευρετηρίασης. Η αντικατάσταση χαρακτήρων μπορεί, για παράδειγμα, να χρησιμοποιηθεί για την αφαίρεση τόνων από τονισμένους χαρακτήρες ή για τη δημιουργία ευρετηρίου χωρίς διάκριση πεζών-κεφαλαίων.

```csharp
public class CharacterReplacementDictionary : DictionaryBase, IEnumerable<int>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../groupdocs.search.dictionaries/characterreplacementdictionary/count) { get; } | Λαμβάνει τον αριθμό των σημείων κώδικα Unicode που περιέχονται σε αυτό το [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [DictionaryType](../../groupdocs.search.dictionaries/characterreplacementdictionary/dictionarytype) { get; } | Λαμβάνει τον τύπο του λεξικού. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange)(CharacterReplacementPair[]) | Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτή την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_1)(IEnumerable&lt;CharacterReplacementPair&gt;) | Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτή την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_2)(IEnumerable&lt;KeyValuePair&lt;char, char&gt;&gt;) | Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων χαρακτήρων σε αυτή την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [AddRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/addrange#addrange_3)(IEnumerable&lt;KeyValuePair&lt;int, int&gt;&gt;) | Προσθέτει τη συγκεκριμένη συλλογή αντικαταστάσεων σημείων κώδικα Unicode σε αυτή την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| override [Clear](../../groupdocs.search.dictionaries/characterreplacementdictionary/clear)() | Αφαιρεί όλες τις αντικαταστάσεις χαρακτήρων από ένα αντικείμενο [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [Contains](../../groupdocs.search.dictionaries/characterreplacementdictionary/contains)(int) | Καθορίζει εάν ένα αντικείμενο [`CharacterReplacementDictionary`](../characterreplacementdictionary) περιέχει αντικατάσταση για το συγκεκριμένο σημείο κώδικα Unicode. |
| [ExportDictionary](../../groupdocs.search.dictionaries/dictionarybase/exportdictionary)(string) | Εξάγει το λεξικό σε ένα αρχείο με το καθορισμένο όνομα. |
| [GetEnumerator](../../groupdocs.search.dictionaries/characterreplacementdictionary/getenumerator)() | Επιστρέφει έναν επαναλήπτη που διασχίζει τη συλλογή. |
| [GetReplacement](../../groupdocs.search.dictionaries/characterreplacementdictionary/getreplacement)(int) | Λαμβάνει μια αντικατάσταση για το καθορισμένο σημείο κώδικα Unicode. |
| [ImportDictionary](../../groupdocs.search.dictionaries/dictionarybase/importdictionary)(string) | Εισάγει ένα λεξικό από το καθορισμένο αρχείο. |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange)(char[]) | Αφαιρεί τη καθορισμένη συλλογή αντικαταστάσεων χαρακτήρων από αυτήν την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_2)(IEnumerable&lt;char&gt;) | Αφαιρεί τη καθορισμένη συλλογή αντικαταστάσεων χαρακτήρων από αυτήν την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_3)(IEnumerable&lt;int&gt;) | Αφαιρεί τη καθορισμένη συλλογή αντικαταστάσεων σημείων κώδικα Unicode από αυτήν την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |
| [RemoveRange](../../groupdocs.search.dictionaries/characterreplacementdictionary/removerange#removerange_1)(int[]) | Αφαιρεί τη καθορισμένη συλλογή αντικαταστάσεων σημείων κώδικα Unicode από αυτήν την παρουσία του [`CharacterReplacementDictionary`](../characterreplacementdictionary). |

### Σχόλια

**Learn more**

* [Character replacement during Indexing](https://docs.groupdocs.com/display/searchnet/Character+replacement+during+Indexing)
* [Managing character replacements](https://docs.groupdocs.com/display/searchnet/Character+replacements)

### Δείτε επίσης

* class [DictionaryBase](../dictionarybase)
* namespace [GroupDocs.Search.Dictionaries](../../groupdocs.search.dictionaries)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
