---
title: "IndexingReport"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente des informations détaillées sur une opération d'indexation."
type: docs
weight: 25
url: /fr/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

Représente des informations détaillées sur une opération d'indexation.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents
index.add(documentsFolder1);
index.add(documentsFolder2);
// Obtention des rapports d'indexation
IndexingReport[] reports = index.getIndexingReports();
// Impression des rapports dans la console
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | Obtient le nombre total de documents dans l'index. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | Obtient le nombre total de termes dans l'index. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | Obtient la longueur totale des documents indexés en Mo. |
|
|  | [getSegmentCount()](#getSegmentCount--) | Obtient le nombre de segments d'index. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | Obtient la taille totale de l'index en octets. |
|
|  | [getStartTime()](#getStartTime--) | Obtient l'heure de début de l'indexation. |
|
|  | [getEndTime()](#getEndTime--) | Obtient l'heure de fin de l'indexation. |
|
|  | [getIndexingTime()](#getIndexingTime--) | Obtient la durée de l'indexation en secondes. |
|
|  | [getErrors()](#getErrors--) | Obtient la liste des erreurs. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Obtient la liste des documents indexés. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | Obtient la liste des documents mis à jour. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | Obtient la liste des documents supprimés de l'index. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


Obtient le nombre total de documents dans l'index.


**Returns:**
int - Le nombre total de documents dans l'index.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


Obtient le nombre total de termes dans l'index.


**Returns:**
int - Le nombre total de termes dans l'index.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


Obtient la longueur totale des documents indexés en Mo.


**Returns:**
double - La longueur totale des documents indexés en Mo.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


Obtient le nombre de segments d'index.


**Returns:**
int - Le nombre de segments d'index.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


Obtient la taille totale de l'index en octets.


**Returns:**
long - La taille totale de l'index en octets.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Obtient l'heure de début de l'indexation.


**Returns:**
java.util.Date - L'heure de début de l'indexation.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Obtient l'heure de fin de l'indexation.


**Returns:**
java.util.Date - L'heure de fin de l'indexation.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


Obtient la durée de l'indexation en secondes.


**Returns:**
double - La durée de l'indexation en secondes.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


Obtient la liste des erreurs.


**Returns:**
java.lang.String[] - La liste des erreurs.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


Obtient la liste des documents indexés.


**Returns:**
java.lang.String[] - La liste des documents indexés.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


Obtient la liste des documents mis à jour.


**Returns:**
java.lang.String[] - La liste des documents mis à jour.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


Obtient la liste des documents supprimés de l'index.


**Returns:**
java.lang.String[] - La liste des documents supprimés de l'index.

