---
title: "TextStorageSettings"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά τις ρυθμίσεις αποθήκευσης κειμένου."
type: docs
weight: 42
url: /el/java/com.groupdocs.search.options/textstoragesettings/
---
**Inheritance:**
java.lang.Object
```
public class TextStorageSettings
```

Αναπαριστά τις ρυθμίσεις αποθήκευσης κειμένου.


**Learn more**

* [Storing text of indexed documents](../https://docs.groupdocs.com/display/searchjava/Storing+text+of+indexed+documents)
* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [TextStorageSettings(Compression compression)](#TextStorageSettings-com.groupdocs.search.options.Compression-) | Αρχικοποιεί μια νέα παρουσία της κλάσης  TextStorageSettings  . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getCompression()](#getCompression--) | Λαμβάνει τη συμπίεση της αποθήκευσης κειμένου. |
|
|  | [setCompression(Compression value)](#setCompression-com.groupdocs.search.options.Compression-) | Ορίζει τη συμπίεση της αποθήκευσης κειμένου. |
|
### TextStorageSettings(Compression compression) {#TextStorageSettings-com.groupdocs.search.options.Compression-}
```
public TextStorageSettings(Compression compression)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  TextStorageSettings  .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | compression | [Compression](../../com.groupdocs.search.options/compression) | Η συμπίεση της αποθήκευσης κειμένου. |
|

### getCompression() {#getCompression--}
```
public final Compression getCompression()
```


Λαμβάνει τη συμπίεση της αποθήκευσης κειμένου. Η προεπιλεγμένη τιμή είναι Compression.Normal.


**Returns:**
[Compression](../../com.groupdocs.search.options/compression) - The compression of text storage.

### setCompression(Compression value) {#setCompression-com.groupdocs.search.options.Compression-}
```
public final void setCompression(Compression value)
```


Ορίζει τη συμπίεση της αποθήκευσης κειμένου. Η προεπιλεγμένη τιμή είναι Compression.Normal.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | value | [Compression](../../com.groupdocs.search.options/compression) | Η συμπίεση της αποθήκευσης κειμένου. |
|

