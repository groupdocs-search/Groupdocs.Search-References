---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un adaptateur de sortie qui collecte la sortie dans un fichier."
type: docs
weight: 21
url: /fr/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

Représente un adaptateur de sortie qui collecte la sortie dans un fichier.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // Création d'un adaptateur de sortie de fichier
index.getDocumentText(documents[0], adapter); // Génération du texte du document dans le fichier de sortie
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | Initialise une nouvelle instance de la classe  FileOutputAdapter  . |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | Obtient un chemin de fichier de sortie. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


Initialise une nouvelle instance de la classe  FileOutputAdapter  .


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | Le format de sortie. |
|
|  | filePath | java.lang.String | Le chemin du fichier de sortie. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Obtient un chemin de fichier de sortie.


**Returns:**
java.lang.String - Le chemin du fichier de sortie.

