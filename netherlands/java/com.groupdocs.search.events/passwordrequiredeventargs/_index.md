---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor het evenement voor wanneer een met een wachtwoord beschermd document wordt geïndexeerd."
type: docs
weight: 20
url: /nl/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Stelt de argumenten voor het evenement voor wanneer een met een wachtwoord beschermd document wordt geïndexeerd.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Haalt het volledige pad van het document op. |
|
|  | [getPassword()](#getPassword--) | Haalt het wachtwoord op voor het openen van het document. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Stelt het wachtwoord in voor het openen van het document. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Haalt het volledige pad van het document op.


**Returns:**
java.lang.String - Het volledige pad van het document.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Haalt het wachtwoord op voor het openen van het document.


**Returns:**
java.lang.String - Het wachtwoord voor het openen van het document.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Stelt het wachtwoord in voor het openen van het document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | waarde | java.lang.String | Het wachtwoord om het document te openen. |
|

