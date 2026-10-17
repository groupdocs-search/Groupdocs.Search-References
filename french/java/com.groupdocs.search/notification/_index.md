---
title: "Notification"
second_title: "GroupDocs.Search pour Java Référence API"
description: "La classe de base pour toutes les notifications à l'index."
type: docs
weight: 22
url: /fr/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

La classe de base pour toutes les notifications vers l'index. Cette classe contient également des méthodes pour créer des objets de notification.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Notification()](#Notification--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Crée un objet de notification pour renommer un document indexé qui a été renommé et qui n'a pas besoin d'être réindexé. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Crée un objet de notification pour renommer un document indexé qui a été renommé et qui n'a pas besoin d'être réindexé. Le document renommé ne sera pas réindexé lors de la prochaine opération de mise à jour, même si son contenu a été modifié.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | oldPath | java.lang.String | L'ancien chemin vers le document indexé. |
|
|  | newPath | java.lang.String | Le nouveau chemin vers le document indexé. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

