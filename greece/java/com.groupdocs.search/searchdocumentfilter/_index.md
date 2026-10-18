---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Περιέχει μεθόδους για τη δημιουργία φίλτρων αναζήτησης εγγράφων."
type: docs
weight: 24
url: /el/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Περιέχει μεθόδους για τη δημιουργία φίλτρων αναζήτησης εγγράφων.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν βρίσκονται στη συγκεκριμένη λίστα πιθανών επεκτάσεων. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Δημιουργεί ένα φίλτρο που έχει αντίστροφη λογική σε σχέση με το καθορισμένο εσωτερικό φίλτρο. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Δημιουργεί μια λογική σύζευξη των καθορισμένων φίλτρων. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Δημιουργεί μια λογική διάζευξη των καθορισμένων φίλτρων. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν έχουν καμία τιμή από τη συγκεκριμένη λίστα επιτρεπόμενων χαρακτηριστικών. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. Η κανονική έκφραση εφαρμόζεται στην πλήρη διαδρομή ενός εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | java.lang.String | Το μοτίβο της κανονικής έκφρασης. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. Η κανονική έκφραση εφαρμόζεται στην πλήρη διαδρομή ενός εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | java.lang.String | Το μοτίβο της κανονικής έκφρασης. |
|
|  | options | int | Οι επιλογές της κανονικής έκφρασης. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν βρίσκονται στη συγκεκριμένη λίστα πιθανών επεκτάσεων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Η λίστα των πιθανών επεκτάσεων. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Δημιουργεί ένα φίλτρο που έχει αντίστροφη λογική σε σχέση με το καθορισμένο εσωτερικό φίλτρο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Το εσωτερικό φίλτρο εγγράφου αναζήτησης. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Δημιουργεί μια λογική σύζευξη των καθορισμένων φίλτρων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Τα φίλτρα εγγράφου αναζήτησης. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Δημιουργεί μια λογική διάζευξη των καθορισμένων φίλτρων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Τα φίλτρα εγγράφου αναζήτησης. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν έχουν καμία τιμή από τη συγκεκριμένη λίστα επιτρεπόμενων χαρακτηριστικών.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ιδιότητες | java.lang.String[] | Η λίστα των επιτρεπτών ιδιοτήτων. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

