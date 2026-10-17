---
title: "FileLogger"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un journal qui enregistre les événements et les erreurs dans un fichier local."
type: docs
weight: 20
url: /fr/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

Représente un journal qui enregistre les événements et les erreurs dans un fichier local.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


L'exemple montre une utilisation typique de la classe.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // Spécification du chemin du fichier journal et d'une longueur maximale de 4 Mo
Index index = new Index(indexFolder, settings); // Création d'un index dans le dossier spécifié
index.add(documentsFolder); // Indexation des documents depuis le dossier spécifié
SearchResult result = index.search(query); // Recherche dans l'index
 
```
 
````


## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | Initialise une nouvelle instance de la classe FileLogger. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | Enregistre une erreur survenue dans l'index. |
|
|  | [trace(String message)](#trace-java.lang.String-) | Enregistre un événement survenu dans l'index. |
|
|  | [getFilePath()](#getFilePath--) | Obtient le chemin du fichier journal. |
|
|  | [getMaxSize()](#getMaxSize--) | Obtient la taille maximale du fichier journal en mégaoctets. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


Initialise une nouvelle instance de la classe FileLogger.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | filePath | java.lang.String | Le chemin du fichier journal. |
|
|  | maxSize | double | La taille maximale du fichier journal en mégaoctets. La valeur doit être comprise entre 0,1 et 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


Enregistre une erreur survenue dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | message | java.lang.String | Le message d'erreur. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


Enregistre un événement survenu dans l'index.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | message | java.lang.String | Le message d'événement. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Obtient le chemin du fichier journal.


**Returns:**
java.lang.String - Le chemin du fichier journal.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


Obtient la taille maximale du fichier journal en mégaoctets.


**Returns:**
double - La taille maximale du fichier journal en mégaoctets.

