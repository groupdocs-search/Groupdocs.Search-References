---
title: "Notifica"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "La classe base per tutte le notifiche all'indice."
type: docs
weight: 22
url: /it/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

La classe base per tutte le notifiche all'indice. Questa classe contiene anche metodi per creare oggetti di notifica.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Notification()](#Notification--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Crea un oggetto di notifica per rinominare un documento indicizzato che è stato rinominato e non necessita di essere reindicizzato. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Crea un oggetto di notifica per rinominare un documento indicizzato che è stato rinominato e non necessita di essere reindicizzato. Il documento rinominato non verrà reindicizzato durante la prossima operazione di aggiornamento, anche se il suo contenuto è stato modificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | oldPath | java.lang.String | Il percorso vecchio del documento indicizzato. |
|
|  | newPath | java.lang.String | Il nuovo percorso del documento indicizzato. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

