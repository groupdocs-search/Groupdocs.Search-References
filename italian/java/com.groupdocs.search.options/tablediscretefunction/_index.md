---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta l'algoritmo di ricerca fuzzy che contiene corrispondenze tra le lunghezze delle parole e il numero di errori consentiti."
type: docs
weight: 40
url: /it/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

Rappresenta l'algoritmo di ricerca fuzzy che contiene corrispondenze tra le lunghezze delle parole e il numero di errori consentiti. Questo algoritmo può essere specificato tramite una tabella di valori di output o mediante una funzione a gradini.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


L'esempio dimostra un utilizzo tipico della classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Creazione di un indice nella cartella specificata
index.add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Abilitazione della ricerca fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // Creazione dell'algoritmo di ricerca fuzzy
// Questa funzione specifica 1 come numero massimo di errori per parole da 1 a 4 caratteri.
// Specifica 2 come numero massimo di errori per parole da 5 a 7 caratteri.
// Specifica 3 come numero massimo di errori per parole da 8 caratteri in su.
SearchResult result = index.search(query, options); // Cerca nell'indice
 
```
 
````


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | Inizializza una nuova istanza della  TableDiscreteFunction  classe. |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | Inizializza una nuova istanza della  TableDiscreteFunction  classe. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | Ottiene un livello di similarità per la lunghezza del termine specificata. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


Inizializza una nuova istanza della  TableDiscreteFunction  classe.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | offsetOfInputs | int | L'offset degli indici della tabella relativo ai valori di input. |
|
|  | tableOfOutputs | int[] | La tabella dei valori di output. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


Inizializza una nuova istanza della  TableDiscreteFunction  classe.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | firstStepLevel | int | Il livello del primo passo della funzione a gradini. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | I prossimi passi della funzione a gradini. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


Ottiene un livello di similarità per la lunghezza del termine specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termLength | int | La lunghezza del termine. |
|

**Returns:**
double - Un livello di similarità.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


Ottiene il numero massimo consentito di errori per la lunghezza del termine specificata.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | termLength | int | La lunghezza del termine. |
|

**Returns:**
int - Un numero massimo consentito di errori.

