---
title: "SearchImage"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει μια εικόνα για αναζήτηση."
type: docs
weight: 29
url: /el/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

Αντιπροσωπεύει μια εικόνα για αναζήτηση.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | Δημιουργεί μια εικόνα από ένα αρχείο για αναζήτηση. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | Δημιουργεί μια εικόνα από ένα αρχείο για αναζήτηση. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | Δημιουργεί μια εικόνα από μια ροή για αναζήτηση. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | Δημιουργεί μια εικόνα από μια ροή για αναζήτηση. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


Δημιουργεί μια εικόνα από ένα αρχείο για αναζήτηση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή του αρχείου εικόνας. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


Δημιουργεί μια εικόνα από ένα αρχείο για αναζήτηση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Η διαδρομή του αρχείου εικόνας. |
|
|  | imageIndex | int | Ο δείκτης της εικόνας σε πολυσελίδες εικόνες. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


Δημιουργεί μια εικόνα από μια ροή για αναζήτηση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ροή | java.io.InputStream | Η ροή εικόνας. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


Δημιουργεί μια εικόνα από μια ροή για αναζήτηση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ροή | java.io.InputStream | Η ροή εικόνας. |
|
|  | imageIndex | int | Ο δείκτης της εικόνας σε πολυσελίδες εικόνες. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

