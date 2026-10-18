---
title: "IndexType"
second_title: "GroupDocs.Search για Java API Reference"
description: "Καθορίζει έναν τύπο ευρετηρίου."
type: docs
weight: 49
url: /el/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Καθορίζει έναν τύπο ευρετηρίου.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Κανονικός δείκτης με μεταδεδομένα εγγράφων και περιεχόμενο εγγράφων που υποστηρίζει όλες τις δυνατότητες αναζήτησης. |
|
|  | [MetadataIndex](#MetadataIndex) | Δείκτης που περιέχει μόνο τα μεταδεδομένα των εγγράφων, χωρίς περιεχόμενο. |
|
|  | [CompactIndex](#CompactIndex) | Τύπος δείκτη που καταλαμβάνει πολύ λιγότερο χώρο στο δίσκο αλλά δεν υποστηρίζει δυνατότητες αναζήτησης φράσεων και εύρους ημερομηνιών. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Κανονικός δείκτης με μεταδεδομένα εγγράφων και περιεχόμενο εγγράφων που υποστηρίζει όλες τις δυνατότητες αναζήτησης.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Δείκτης που περιέχει μόνο τα μεταδεδομένα των εγγράφων, χωρίς περιεχόμενο.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Τύπος δείκτη που καταλαμβάνει πολύ λιγότερο χώρο στο δίσκο αλλά δεν υποστηρίζει δυνατότητες αναζήτησης φράσεων και εύρους ημερομηνιών.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| όνομα | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
