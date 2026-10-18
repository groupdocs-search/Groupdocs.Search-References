---
title: "Configurator"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά το διαμορφωτή δικτύου αναζήτησης."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

Αναπαριστά το διαμορφωτή δικτύου αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [Configurator()](#Configurator--) | Αρχικοποιεί ένα νέο στιγμιότυπο της  Configurator  κλάσης. |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | Ξεκινά τη διαμόρφωση των ρυθμίσεων ευρετηρίου για κάθε shard στο δίκτυο αναζήτησης. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | Προσθέτει έναν κόμβο στη διαμόρφωση του δικτύου αναζήτησης. |
|
|  | [completeConfiguration()](#completeConfiguration--) | Ολοκληρώνει τη διαδικασία διαμόρφωσης και επιστρέφει ένα στιγμιότυπο της διαμόρφωσης του δικτύου αναζήτησης. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της  Configurator  κλάσης.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


Ξεκινά τη διαμόρφωση των ρυθμίσεων ευρετηρίου για κάθε shard στο δίκτυο αναζήτησης.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


Προσθέτει έναν κόμβο στη διαμόρφωση του δικτύου αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | nodeIndex | int | Ο δείκτης κόμβου. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


Ολοκληρώνει τη διαδικασία διαμόρφωσης και επιστρέφει ένα στιγμιότυπο της διαμόρφωσης του δικτύου αναζήτησης.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
