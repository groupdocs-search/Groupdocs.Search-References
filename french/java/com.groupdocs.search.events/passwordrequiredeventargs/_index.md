---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments de l'événement qui se produit lorsqu'un document protégé par un mot de passe est indexé."
type: docs
weight: 20
url: /fr/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Représente les arguments de l'événement qui se produit lorsqu'un document protégé par un mot de passe est indexé.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Obtient le chemin complet du document. |
|
|  | [getPassword()](#getPassword--) | Obtient le mot de passe pour ouvrir le document. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Définit le mot de passe pour ouvrir le document. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Obtient le chemin complet du document.


**Returns:**
java.lang.String - Le chemin complet du document.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Obtient le mot de passe pour ouvrir le document.


**Returns:**
java.lang.String - Le mot de passe pour ouvrir le document.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Définit le mot de passe pour ouvrir le document.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | valeur | java.lang.String | Le mot de passe pour ouvrir le document. |
|

