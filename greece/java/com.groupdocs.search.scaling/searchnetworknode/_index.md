---
title: "SearchNetworkNode"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει έναν κόμβο δικτύου αναζήτησης που μπορεί να περιέχει υπηρεσίες όπως extractor indexer searcher shard."
type: docs
weight: 11
url: /el/java/com.groupdocs.search.scaling/searchnetworknode/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class SearchNetworkNode implements Closeable
```

Αντιπροσωπεύει έναν κόμβο δικτύου αναζήτησης που μπορεί να περιέχει υπηρεσίες όπως εξαγωγέας, ευρετηριαστής, αναζητητής, τμήμα.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SearchNetworkNode . |
|
|  | [SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)](#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SearchNetworkNode . |
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [start()](#start--) | Ξεκινά τη λειτουργία του κόμβου δικτύου αναζήτησης. |
|
|  | [configureAllNodes()](#configureAllNodes--) | Διαμορφώνει όλους τους κόμβους στο δίκτυο αναζήτησης. |
|
|  | [configureNode(int nodeIndex)](#configureNode-int-) | Διαμορφώνει τον καθορισμένο κόμβο στο δίκτυο αναζήτησης. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | Λαμβάνει τη συλλογή προσαρμοσμένων εξαγωγέων. |
|
|  | [setOcrConnector(IOcrConnector ocrConnector)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Ορίζει έναν σύνδεσμο OCR που χρησιμοποιείται για επεξεργασία OCR. |
|
|  | [setWordFormsProvider(IWordFormsProvider wordFormsProvider)](#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-) | Ορίζει έναν πάροχο μορφών λέξεων. |
|
|  | [close()](#close--) | Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το SearchNetworkNode. |
|
|  | [getNodeIndex()](#getNodeIndex--) | Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης. |
|
|  | [getEvents()](#getEvents--) | Λαμβάνει το κέντρο γεγονότων για την εγγραφή σε γεγονότα. |
|
|  | [getIndexer()](#getIndexer--) | Λαμβάνει τον ευρετηριαστή. |
|
|  | [getSearcher()](#getSearcher--) | Λαμβάνει τον αναζητητή. |
|
|  | [getShardIndices()](#getShardIndices--) | Λαμβάνει έναν πίνακα με όλους τους δείκτες των shards στο δίκτυο αναζήτησης. |
|
|  | [getNodeIndex(int serviceIndex)](#getNodeIndex-int-) | Λαμβάνει τον δείκτη του κόμβου όπου βρίσκεται η υπηρεσία. |
|
| [getCore()](#getCore--) |  |
### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SearchNetworkNode .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | nodeIndex | int | Ο δείκτης κόμβου. |
|
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Οι ρυθμίσεις δικτύου. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SearchNetworkNode .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | nodeIndex | int | Ο δείκτης κόμβου. |
|
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Οι ρυθμίσεις δικτύου. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Ο καταγραφέας. |
|

### SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration) {#SearchNetworkNode-int-java.lang.String-com.groupdocs.search.scaling.configuring.INetworkSettings-com.groupdocs.search.common.ILogger-com.groupdocs.search.scaling.configuring.Configuration-}
```
public SearchNetworkNode(int nodeIndex, String storagePath, INetworkSettings networkSettings, ILogger logger, Configuration configuration)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης  SearchNetworkNode .


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | nodeIndex | int | Ο δείκτης κόμβου. |
|
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης. |
|
|  | networkSettings | [INetworkSettings](../../com.groupdocs.search.scaling.configuring/inetworksettings) | Οι ρυθμίσεις δικτύου. |
|
|  | logger | [ILogger](../../com.groupdocs.search.common/ilogger) | Ο καταγραφέας. |
|
|  | configuration | [Configuration](../../com.groupdocs.search.scaling.configuring/configuration) | Η διαμόρφωση. |
|

### start() {#start--}
```
public void start()
```


Ξεκινά τη λειτουργία του κόμβου δικτύου αναζήτησης.


### configureAllNodes() {#configureAllNodes--}
```
public void configureAllNodes()
```


Διαμορφώνει όλους τους κόμβους στο δίκτυο αναζήτησης.


### configureNode(int nodeIndex) {#configureNode-int-}
```
public void configureNode(int nodeIndex)
```


Διαμορφώνει τον καθορισμένο κόμβο στο δίκτυο αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | nodeIndex | int | Ο δείκτης κόμβου. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public CustomExtractorCollection getCustomExtractors()
```


Λαμβάνει τη συλλογή προσαρμοσμένων εξαγωγέων. Το πλήρες παράδειγμα υλοποίησης ενός προσαρμοσμένου εξαγωγέα παρουσιάζεται στην τεκμηρίωση για τη διεπαφή GroupDocs.Search.Common.IFieldExtractor.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### setOcrConnector(IOcrConnector ocrConnector) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public void setOcrConnector(IOcrConnector ocrConnector)
```


Ορίζει έναν σύνδεσμο OCR που χρησιμοποιείται για επεξεργασία OCR.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Ο σύνδεσμος OCR. |
|

### setWordFormsProvider(IWordFormsProvider wordFormsProvider) {#setWordFormsProvider-com.groupdocs.search.dictionaries.IWordFormsProvider-}
```
public void setWordFormsProvider(IWordFormsProvider wordFormsProvider)
```


Ορίζει έναν πάροχο μορφών λέξεων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | wordFormsProvider | [IWordFormsProvider](../../com.groupdocs.search.dictionaries/iwordformsprovider) | Ο πάροχος μορφών λέξεων. |
|

### close() {#close--}
```
public void close()
```


Απελευθερώνει όλους τους πόρους που χρησιμοποιούνται από το SearchNetworkNode.


### getNodeIndex() {#getNodeIndex--}
```
public int getNodeIndex()
```


Λαμβάνει τον δείκτη του κόμβου δικτύου αναζήτησης.


**Returns:**
int - Ο δείκτης του κόμβου δικτύου αναζήτησης.

### getEvents() {#getEvents--}
```
public NodeEventHub getEvents()
```


Λαμβάνει το κέντρο γεγονότων για την εγγραφή σε γεγονότα.


**Returns:**
[NodeEventHub](../../com.groupdocs.search.scaling.events/nodeeventhub) - The event hub for subscribing to events.

### getIndexer() {#getIndexer--}
```
public Indexer getIndexer()
```


Λαμβάνει τον ευρετηριαστή.


**Returns:**
[Indexer](../../com.groupdocs.search.scaling/indexer) - The indexer.

### getSearcher() {#getSearcher--}
```
public Searcher getSearcher()
```


Λαμβάνει τον αναζητητή.


**Returns:**
[Searcher](../../com.groupdocs.search.scaling/searcher) - The searcher.

### getShardIndices() {#getShardIndices--}
```
public int[] getShardIndices()
```


Λαμβάνει έναν πίνακα με όλους τους δείκτες των shards στο δίκτυο αναζήτησης.


**Returns:**
int[] - Ένας πίνακας με όλους τους δείκτες των shards στο δίκτυο αναζήτησης.

### getNodeIndex(int serviceIndex) {#getNodeIndex-int-}
```
public int getNodeIndex(int serviceIndex)
```


Λαμβάνει τον δείκτη του κόμβου όπου βρίσκεται η υπηρεσία.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | serviceIndex | int | Ο δείκτης της υπηρεσίας. |
|

**Returns:**
int - Ο δείκτης του κόμβου όπου βρίσκεται η υπηρεσία. Εάν ο δείκτης της υπηρεσίας είναι εσφαλμένος, επιστρέφεται -1.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
