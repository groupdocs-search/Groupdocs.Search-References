---
title: "Benachrichtigung"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Die Basisklasse für alle Benachrichtigungen an den Index."
type: docs
weight: 22
url: /de/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

Die Basisklasse für alle Benachrichtigungen zum Index. Diese Klasse enthält außerdem Methoden zum Erstellen von Benachrichtigungsobjekten.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Notification()](#Notification--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Erstellt ein Benachrichtigungsobjekt, um ein indiziertes Dokument umzubenennen, das bereits umbenannt wurde und nicht erneut indiziert werden muss. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Erstellt ein Benachrichtigungsobjekt, um ein indiziertes Dokument umzubenennen, das bereits umbenannt wurde und nicht erneut indiziert werden muss. Das umbenannte Dokument wird während des nächsten Update‑Vorgangs nicht erneut indiziert, selbst wenn sein Inhalt geändert wurde.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | oldPath | java.lang.String | Der alte Pfad zum indizierten Dokument. |
|
|  | newPath | java.lang.String | Der neue Pfad zum indizierten Dokument. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

