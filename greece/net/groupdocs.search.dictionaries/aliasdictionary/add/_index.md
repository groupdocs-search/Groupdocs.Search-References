---
title: Add
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Προσθέτει το καθορισμένο ζεύγος ψευδωνύμων και το σχετικό κείμενο σε αυτήν την εμφάνιση τουAliasDictionarygroupdocs.search.dictionaries/aliasdictionary .
type: docs
weight: 20
url: /el/net/groupdocs.search.dictionaries/aliasdictionary/add/
---
## AliasDictionary.Add method

Προσθέτει το καθορισμένο ζεύγος ψευδωνύμων και το σχετικό κείμενο σε αυτήν την εμφάνιση του[`AliasDictionary`](../../aliasdictionary) .

```csharp
public void Add(string alias, string text)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| alias | String | Το ψευδώνυμο για προσθήκη στο λεξικό. |
| text | String | Το κείμενο που θα συσχετιστεί με το ψευδώνυμο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | Ρίχτηκε όταν*alias* ή*text* είναι`μηδενικό`. |
| ArgumentException | Το ψευδώνυμο περιέχει χαρακτήρα που δεν είναι από τα εύρη ab και 0-9. |

### Δείτε επίσης

* class [AliasDictionary](../../aliasdictionary)
* χώρος ονομάτων [GroupDocs.Search.Dictionaries](../../aliasdictionary)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->