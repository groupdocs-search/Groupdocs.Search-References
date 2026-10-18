---
title: "Extractor"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει ένα εργαλείο για προκαταρκτική εξαγωγή δεδομένων από έγγραφα, προκειμένου να διαχωριστεί το στάδιο της επακόλουθης γρήγορης ευρετηρίασης."
type: docs
weight: 16
url: /el/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

Αντιπροσωπεύει ένα εργαλείο για προκαταρκτική εξαγωγή δεδομένων από έγγραφα, προκειμένου να διαχωριστεί το στάδιο της επακόλουθης γρήγορης ευρετηρίασης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Extractor()](#Extractor--) | Αρχικοποιεί ένα νέο αντικείμενο της  Extractor  κλάσης. |
|
## Πεδία

| Πεδίο | Περιγραφή |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | Συμβαίνει όταν προκύπτει σφάλμα κατά τη λειτουργία του εξαγωγέα. |
|
|  | [ImagePreparing](#ImagePreparing) | Συμβαίνει όταν μια εικόνα προετοιμάζεται για ευρετηρίαση. |
|
|  | [PasswordRequired](#PasswordRequired) | Συμβαίνει όταν ένα έγγραφο απαιτεί κωδικό πρόσβασης για άνοιγμα. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getSettings()](#getSettings--) | Λαμβάνει τις ρυθμίσεις του εξαγωγέα. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | Εξάγει δεδομένα από ένα έγγραφο. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


Αρχικοποιεί ένα νέο αντικείμενο της  Extractor  κλάσης.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


Συμβαίνει όταν προκύπτει σφάλμα κατά τη λειτουργία του εξαγωγέα.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


Συμβαίνει όταν μια εικόνα προετοιμάζεται για ευρετηρίαση.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


Συμβαίνει όταν ένα έγγραφο απαιτεί κωδικό πρόσβασης για άνοιγμα.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


Λαμβάνει τις ρυθμίσεις του εξαγωγέα.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


Εξάγει δεδομένα από ένα έγγραφο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | Το έγγραφο από το σύστημα αρχείων, τη ροή ή τη δομή. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | Οι επιλογές εξαγωγής. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μήνυμα | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| ροή | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
