---
title: "SearchResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un résultat de recherche correspondant à une requête de recherche."
type: docs
weight: 19
url: /fr/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

Représente un résultat de recherche correspondant à une requête de recherche.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Création d'un index
Index index = new Index(indexFolder);
// Indexation des documents du dossier spécifié
index.add(documentFolder);
// Définition des options de recherche
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Activation de la recherche floue
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Définition du nombre maximal de différences à 3
// Recherche de documents contenant le mot 'Einstein' ou la phrase 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// Affichage du résultat
System.out.println("Documents : " + result.getDocumentCount());
System.out.println("Occurrences totales : " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocument : " + document.getDocumentInfo().getFilePath());
System.out.println("\tOccurrences : " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tChamp : " + field.getFieldName());
System.out.println("\t\tOccurrences : " + document.getOccurrenceCount());
// Impression des termes trouvés
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// Impression des phrases trouvées
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = \"\";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | Obtient le nombre de documents trouvés. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtient le nombre total d'occurrences trouvées. |
|
|  | [getTruncated()](#getTruncated--) | Obtient une valeur indiquant que le résultat est tronqué. |
|
|  | [getWarnings()](#getWarnings--) | Obtient des avertissements décrivant le résultat. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | Obtient un jeton de recherche par bloc pour rechercher le bloc suivant. |
|
|  | [getStartTime()](#getStartTime--) | Obtient l'heure de début de la recherche. |
|
|  | [getEndTime()](#getEndTime--) | Obtient l'heure de fin de la recherche. |
|
|  | [getSearchDuration()](#getSearchDuration--) | Obtient la durée de la recherche en secondes. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | Obtient le document trouvé par indice. |
|
|  | [iterator()](#iterator--) | Renvoie un itérateur qui parcourt la collection des documents trouvés. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


Obtient une valeur indiquant que le résultat est tronqué.


**Returns:**
boolean - Une valeur indiquant que le résultat est tronqué.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


Obtient des avertissements décrivant le résultat.


**Returns:**
java.lang.String - Des avertissements décrivant le résultat.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


Obtient un jeton de recherche par bloc pour rechercher le bloc suivant.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


Obtient le document trouvé par indice.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | index | int | L'indice d'un document trouvé. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


Renvoie un itérateur qui parcourt la collection des documents trouvés.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - Un itérateur qui peut être utilisé pour parcourir la collection des documents trouvés.

