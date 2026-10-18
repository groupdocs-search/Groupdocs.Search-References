---
title: "Configuration"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά μια διαμόρφωση δικτύου αναζήτησης."
type: docs
weight: 10
url: /el/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

Αναπαριστά μια διαμόρφωση δικτύου αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | Αποθηκεύει αυτή τη διαμόρφωση σε ένα αρχείο. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | Αποθηκεύει αυτή τη διαμόρφωση σε μια ροή. |
|
|  | [load(String filePath)](#load-java.lang.String-) | Φορτώνει μια διαμόρφωση δικτύου αναζήτησης από ένα αρχείο. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | Φορτώνει μια διαμόρφωση δικτύου αναζήτησης από μια ροή. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


Αποθηκεύει αυτή τη διαμόρφωση σε ένα αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Το αρχείο για αποθήκευση. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


Αποθηκεύει αυτή τη διαμόρφωση σε μια ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ροή | java.io.OutputStream | Η ροή για αποθήκευση. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


Φορτώνει μια διαμόρφωση δικτύου αναζήτησης από ένα αρχείο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filePath | java.lang.String | Το αρχείο για φόρτωση. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


Φορτώνει μια διαμόρφωση δικτύου αναζήτησης από μια ροή.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ροή | java.io.InputStream | Η ροή από την οποία θα φορτωθεί. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

