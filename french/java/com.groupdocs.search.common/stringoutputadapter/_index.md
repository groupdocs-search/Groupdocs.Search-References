---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un adaptateur de sortie qui collecte la sortie sous forme d'un System.String."
type: docs
weight: 32
url: /fr/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

Représente un adaptateur de sortie qui collecte la sortie sous forme d'un System.String.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
DocumentInfo[] documents = index.getIndexedDocuments(); // Obtention des informations sur les documents indexés
StringOutputAdapter adapter = new StringOutputAdapter(); // Création d'un adaptateur de sortie de chaîne
index.getDocumentText(documents[0], adapter); // Génération du texte du document dans l'adaptateur
String result = adapter.getResult(); // Obtention d'un résultat
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | Initialise une nouvelle instance de la classe  StringOutputAdapter . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getResult()](#getResult--) | Obtient la chaîne résultante. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


Initialise une nouvelle instance de la classe  StringOutputAdapter .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Le format de sortie. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


Obtient la chaîne résultante.


**Returns:**
java.lang.String - La chaîne résultante.

