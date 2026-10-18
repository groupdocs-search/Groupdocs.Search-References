---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο ως μια δομή που περιέχει κάθε πεδίο ξεχωριστά."
type: docs
weight: 33
url: /el/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

Αντιπροσωπεύει έναν προσαρμογέα εξόδου που συλλέγει την έξοδο ως μια δομή που περιέχει κάθε πεδίο ξεχωριστά.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Αρχικοποιεί μια νέα παρουσία της κλάσης StructureOutputAdapter. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getResult()](#getResult--) | Λαμβάνει τον τελικό πίνακα πεδίων. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης StructureOutputAdapter.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Η μορφή εξόδου. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


Λαμβάνει τον τελικό πίνακα πεδίων.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Ο τελικός πίνακας πεδίων.

