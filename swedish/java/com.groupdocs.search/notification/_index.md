---
title: "Meddelande"
second_title: "GroupDocs.Search för Java API-referens"
description: "Basklassen för alla meddelanden till indexet."
type: docs
weight: 22
url: /sv/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

Bas-klassen för alla meddelanden till indexet. Denna klass innehåller också metoder för att skapa meddelandeobjekt.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Notification()](#Notification--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Skapar ett meddelandeobjekt för att byta namn på ett indexerat dokument som har bytts namn och inte behöver indexeras om. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Skapar ett meddelandeobjekt för att byta namn på ett indexerat dokument som har bytts namn och inte behöver indexeras om. Det omdöpta dokumentet kommer inte att indexeras om under nästa uppdateringsoperation, även om dess innehåll har ändrats.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | oldPath | java.lang.String | Den gamla sökvägen till det indexerade dokumentet. |
|
|  | newPath | java.lang.String | Den nya sökvägen till det indexerade dokumentet. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

