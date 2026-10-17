---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement d'une erreur d'index."
type: docs
weight: 16
url: /fr/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement d'une erreur d'index.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getMessage()](#getMessage--) | Obtient le message d'erreur. |
|
|  | [isCritical()](#isCritical--) | Obtient un indicateur indiquant que l'erreur survenue est critique et que l'index doit être redémarré. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Obtient le message d'erreur.


**Returns:**
java.lang.String - Le message d'erreur.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Obtient un indicateur indiquant que l'erreur survenue est critique et que l'index doit être redémarré.


**Returns:**
boolean - L'indicateur indiquant que l'erreur survenue est critique et que l'index doit être redémarré.

