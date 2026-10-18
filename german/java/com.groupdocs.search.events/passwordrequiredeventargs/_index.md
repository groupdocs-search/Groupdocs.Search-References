---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für das Ereignis dar, das auftritt, wenn ein durch ein Passwort geschütztes Dokument indexiert wird."
type: docs
weight: 20
url: /de/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Stellt Argumente für das Ereignis dar, das auftritt, wenn ein durch ein Passwort geschütztes Dokument indexiert wird.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Gibt den vollständigen Pfad des Dokuments zurück. |
|
|  | [getPassword()](#getPassword--) | Gibt das Passwort zum Öffnen des Dokuments zurück. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Setzt das Passwort zum Öffnen des Dokuments. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Gibt den vollständigen Pfad des Dokuments zurück.


**Returns:**
java.lang.String - Der vollständige Pfad des Dokuments.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gibt das Passwort zum Öffnen des Dokuments zurück.


**Returns:**
java.lang.String - Das Passwort zum Öffnen des Dokuments.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Setzt das Passwort zum Öffnen des Dokuments.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wert | java.lang.String | Das Passwort zum Öffnen des Dokuments. |
|

