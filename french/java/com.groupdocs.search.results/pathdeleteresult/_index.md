---
title: "PathDeleteResult"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le résultat de l'opération de suppression d'un fichier ou dossier indexé d'un index."
type: docs
weight: 18
url: /fr/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Représente le résultat de l'opération de suppression d'un fichier ou dossier indexé d'un index.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Renvoie l'indicateur de succès de l'opération de suppression. |
|
|  | [getError()](#getError--) | Renvoie une description de l'erreur de suppression. |
|
|  | [getPath()](#getPath--) | Renvoie le chemin du fichier ou du dossier à supprimer. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Renvoie l'indicateur de succès de l'opération de suppression.


**Returns:**
boolean -  true  si l'opération de suppression a réussi ; sinon, renvoie  false .

### getError() {#getError--}
```
public final String getError()
```


Renvoie une description de l'erreur de suppression.


**Returns:**
java.lang.String - Une description de l'erreur de suppression.

### getPath() {#getPath--}
```
public final String getPath()
```


Renvoie le chemin du fichier ou du dossier à supprimer.


**Returns:**
java.lang.String - Le chemin du fichier ou du dossier à supprimer.

