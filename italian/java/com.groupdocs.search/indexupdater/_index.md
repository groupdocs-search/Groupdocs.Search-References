---
title: "IndexUpdater"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un aggiornatore di indice."
type: docs
weight: 20
url: /it/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Rappresenta un aggiornatore di indice. Questa classe esegue la reindicizzazione dei documenti in un indice di una versione precedente.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


L'esempio dimostra un utilizzo tipico della classe.

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


## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Inizializza una nuova istanza della  IndexUpdater  classe. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Verifica se la directory specificata contiene un indice dell'ultima versione. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Verifica se un indice nella directory specificata può essere aggiornato all'ultima versione. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Esegue la reindicizzazione dei documenti in un indice di una versione precedente. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Inizializza una nuova istanza della  IndexUpdater  classe.


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Verifica se la directory specificata contiene un indice dell'ultima versione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexPath | java.lang.String | Il percorso della directory dell'indice. |
|

**Returns:**
boolean -  true  se la directory specificata contiene un indice dell'ultima versione; altrimenti  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Verifica se un indice nella directory specificata può essere aggiornato all'ultima versione.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexPath | java.lang.String | Il percorso della directory dell'indice. |
|

**Returns:**
boolean -  true  se un indice nella directory specificata può essere aggiornato all'ultima versione; altrimenti  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Esegue la reindicizzazione dei documenti in un indice di una versione precedente. L'indice aggiornato sarà collocato nella directory  newIndexPath . L'indice nella directory  indexPath  non verrà modificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | indexPath | java.lang.String | Il percorso della directory dell'indice. |
|
|  | newIndexPath | java.lang.String | La directory per l'indice aggiornato. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

