---
title: "Melding"
second_title: "GroupDocs.Search for Java API-referentie"
description: "De basisklasse voor alle meldingen aan de index."
type: docs
weight: 22
url: /nl/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

De basisklasse voor alle meldingen naar de index. Deze klasse bevat ook methoden voor het maken van meldingsobjecten.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Notification()](#Notification--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | Maakt een meldingsobject om een geïndexeerd document te hernoemen dat al is hernoemd en niet opnieuw geïndexeerd hoeft te worden. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


Maakt een meldingsobject om een geïndexeerd document te hernoemen dat al is hernoemd en niet opnieuw geïndexeerd hoeft te worden. Het hernoemde document wordt niet opnieuw geïndexeerd tijdens de volgende updatebewerking, zelfs als de inhoud is gewijzigd.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | oldPath | java.lang.String | Het oude pad naar het geïndexeerde document. |
|
|  | newPath | java.lang.String | Het nieuwe pad naar het geïndexeerde document. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

