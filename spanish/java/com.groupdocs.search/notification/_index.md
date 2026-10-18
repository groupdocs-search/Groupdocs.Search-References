---
title: "Notificación"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "La clase base para todas las notificaciones al índice."
type: docs
weight: 22
url: /es/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

La clase base para todas las notificaciones al índice. Esta clase también contiene métodos para crear objetos de notificación.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [Notification()](#Notification--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Crea un objeto de notificación para renombrar un documento indexado que ha sido renombrado y no necesita ser reindexado. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Crea un objeto de notificación para renombrar un documento indexado que ha sido renombrado y no necesita ser reindexado. El documento renombrado no será reindexado durante la próxima operación de actualización, incluso si su contenido ha sido modificado.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | oldPath | java.lang.String | La ruta antigua al documento indexado. |
|
|  | newPath | java.lang.String | La ruta nueva al documento indexado. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

