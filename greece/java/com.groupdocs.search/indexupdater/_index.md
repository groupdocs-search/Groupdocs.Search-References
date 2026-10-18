---
title: "IndexUpdater"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν ενημερωτή ευρετηρίου."
type: docs
weight: 20
url: /el/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Αντιπροσωπεύει έναν ενημερωτή ευρετηρίου. Αυτή η κλάση εκτελεί επανευρετηρίαση εγγράφων σε ένα ευρετήριο παλαιάς έκδοσης.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Το παράδειγμα δείχνει μια τυπική χρήση της κλάσης.

````
 ```

String sourceIndexFolder = "c:\\MyOldIndex\\";
String targetIndexFolder = "c:\\MyNewIndex\\";
IndexUpdater updater = new IndexUpdater();
if (updater.canUpdateVersion(sourceIndexFolder)) {
int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
}
 
```
 
````


## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Αρχικοποιεί μια νέα παρουσία της κλάσης  IndexUpdater  . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Ελέγχει εάν ο καθορισμένος φάκελος περιέχει ένα ευρετήριο της τελευταίας έκδοσης. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Ελέγχει εάν ένα ευρετήριο στον καθορισμένο φάκελο μπορεί να ενημερωθεί στην τελευταία έκδοση. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Εκτελεί επανευρετηρίαση εγγράφων σε ένα ευρετήριο παλαιάς έκδοσης. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης  IndexUpdater  .


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Ελέγχει εάν ο καθορισμένος φάκελος περιέχει ένα ευρετήριο της τελευταίας έκδοσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexPath | java.lang.String | Η διαδρομή του φακέλου ευρετηρίου. |
|

**Returns:**
boolean -  true  εάν ο καθορισμένος φάκελος περιέχει ένα ευρετήριο της τελευταίας έκδοσης· διαφορετικά  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Ελέγχει εάν ένα ευρετήριο στον καθορισμένο φάκελο μπορεί να ενημερωθεί στην τελευταία έκδοση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexPath | java.lang.String | Η διαδρομή του φακέλου ευρετηρίου. |
|

**Returns:**
boolean -  true  εάν ένα ευρετήριο στον καθορισμένο φάκελο μπορεί να ενημερωθεί στην τελευταία έκδοση· διαφορετικά  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Εκτελεί επανευρετηρίαση εγγράφων σε ένα ευρετήριο παλαιάς έκδοσης. Το ενημερωμένο ευρετήριο θα τοποθετηθεί στον φάκελο  newIndexPath . Ο φάκελος  indexPath  δεν θα αλλάξει.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | indexPath | java.lang.String | Η διαδρομή του φακέλου ευρετηρίου. |
|
|  | newIndexPath | java.lang.String | Ο φάκελος για το ενημερωμένο ευρετήριο. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

