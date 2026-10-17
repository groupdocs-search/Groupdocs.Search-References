---
title: "SearchReport"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente une information détaillée sur une opération de recherche."
type: docs
weight: 30
url: /fr/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

Représente une information détaillée sur une opération de recherche.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentsFolder);
// Recherche dans l'index
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// Obtention des rapports de recherche
SearchReport[] reports = index.getSearchReports();
// Impression des rapports dans la console
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | Obtient l'heure de début de la recherche. |
|
|  | [getEndTime()](#getEndTime--) | Obtient l'heure de fin de la recherche. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Obtient la durée de la recherche en secondes. |
|
|  | [getDocumentCount()](#getDocumentCount--) | Obtient le nombre de documents trouvés. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtient le nombre total d'occurrences trouvées. |
|
|  | [getTextQuery()](#getTextQuery--) | Obtient la requête de recherche sous forme de texte. |
|
|  | [getObjectQuery()](#getObjectQuery--) | Obtient la requête de recherche sous forme d'objet. |
|
|  | [getSearchOptions()](#getSearchOptions--) | Obtient les options de recherche. |
|
|  | [toString()](#toString--) | Renvoie une chaîne qui représente le SearchReport actuel. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


Obtient l'heure de début de la recherche.


**Returns:**
java.util.Date - L'heure de début de la recherche.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


Obtient l'heure de fin de la recherche.


**Returns:**
java.util.Date - L'heure de fin de la recherche.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


Obtient la durée de la recherche en secondes.


**Returns:**
double - La durée de la recherche en secondes.

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


Obtient le nombre de documents trouvés.


**Returns:**
int - Le nombre de documents trouvés.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtient le nombre total d'occurrences trouvées.


**Returns:**
int - Le nombre total d'occurrences trouvées.

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


Obtient la requête de recherche sous forme de texte.


**Returns:**
java.lang.String - La requête de recherche sous forme de texte.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


Obtient la requête de recherche sous forme d'objet.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


Obtient les options de recherche.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


Renvoie une chaîne qui représente le SearchReport actuel.


**Returns:**
java.lang.String - Une chaîne qui représente le SearchReport actuel.

