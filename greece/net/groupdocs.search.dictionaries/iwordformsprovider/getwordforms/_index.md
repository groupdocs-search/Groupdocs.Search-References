---
title: GetWordForms
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Λαμβάνει τις μορφές λέξης για την καθορισμένη λέξη. Ο πίνακας που προκύπτει δεν περιέχει την αρχική λέξη.
type: docs
weight: 10
url: /el/net/groupdocs.search.dictionaries/iwordformsprovider/getwordforms/
---
## IWordFormsProvider.GetWordForms method

Λαμβάνει τις μορφές λέξης για την καθορισμένη λέξη. Ο πίνακας που προκύπτει δεν περιέχει την αρχική λέξη.

```csharp
public string[] GetWordForms(string word)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| word | String | Η λέξη που προτείνει τη λέξη σχηματίζει. |

### Επιστρεφόμενη Αξία

Η λέξη σχηματίζεται για την καθορισμένη λέξη ή τον κενό πίνακα εάν[`IWordFormsProvider`](../../iwordformsprovider) δεν παρέχει μορφές λέξης για την καθορισμένη λέξη.

### Δείτε επίσης

* interface [IWordFormsProvider](../../iwordformsprovider)
* χώρος ονομάτων [GroupDocs.Search.Dictionaries](../../iwordformsprovider)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->