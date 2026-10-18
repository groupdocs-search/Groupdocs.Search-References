---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för händelsen som inträffar när ett lösenordsskyddat dokument indexeras."
type: docs
weight: 20
url: /sv/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Representerar argument för händelsen som inträffar när ett lösenordsskyddat dokument indexeras.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | Hämtar dokumentets fullständiga sökväg. |
|
|  | [getPassword()](#getPassword--) | Hämtar lösenordet för att öppna dokumentet. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in lösenordet för att öppna dokumentet. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Hämtar dokumentets fullständiga sökväg.


**Returns:**
java.lang.String - Dokumentets fullständiga sökväg.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


Hämtar lösenordet för att öppna dokumentet.


**Returns:**
java.lang.String - Lösenordet för att öppna dokumentet.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Ställer in lösenordet för att öppna dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | värde | java.lang.String | Lösenordet för att öppna dokumentet. |
|

