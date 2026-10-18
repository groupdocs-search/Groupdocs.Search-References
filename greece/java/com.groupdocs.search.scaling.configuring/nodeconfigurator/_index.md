---
title: "NodeConfigurator"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά το διαμορφωτή κόμβου δικτύου αναζήτησης."
type: docs
weight: 13
url: /el/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

Αναπαριστά το διαμορφωτή κόμβου δικτύου αναζήτησης.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | Ορίζει το σημείο λήψης TCP. |
|
|  | [addLogSink()](#addLogSink--) | Προσθέτει ένα log sink στον κόμβο δικτύου αναζήτησης. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | Προσθέτει μια υπηρεσία αναζήτησης στον κόμβο δικτύου αναζήτησης. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | Προσθέτει μια υπηρεσία ευρετηρίου στον κόμβο του δικτύου αναζήτησης. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | Προσθέτει μια υπηρεσία εξαγωγέα στον κόμβο του δικτύου αναζήτησης. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | Προσθέτει μια υπηρεσία shard στον κόμβο του δικτύου αναζήτησης. |
|
|  | [completeNode()](#completeNode--) | Ολοκληρώνει τη διαμόρφωση του κόμβου του δικτύου αναζήτησης. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


Ορίζει το σημείο λήψης TCP.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | Το όνομα κεντρικού υπολογιστή ή η διεύθυνση. |
|
|  | port | int | Ο αριθμός θύρας. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


Προσθέτει ένα log sink στον κόμβο δικτύου αναζήτησης.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


Προσθέτει μια υπηρεσία αναζήτησης στον κόμβο δικτύου αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης της υπηρεσίας προσθήκης. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


Προσθέτει μια υπηρεσία ευρετηρίου στον κόμβο του δικτύου αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης της υπηρεσίας προσθήκης. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


Προσθέτει μια υπηρεσία εξαγωγέα στον κόμβο του δικτύου αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης της υπηρεσίας προσθήκης. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


Προσθέτει μια υπηρεσία shard στον κόμβο του δικτύου αναζήτησης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | storagePath | java.lang.String | Η διαδρομή αποθήκευσης της υπηρεσίας προσθήκης. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


Ολοκληρώνει τη διαμόρφωση του κόμβου του δικτύου αναζήτησης.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

