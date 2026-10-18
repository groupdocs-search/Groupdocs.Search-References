---
title: "PathDeleteResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt das Ergebnis der Operation zum Löschen einer indizierten Datei oder eines Ordners aus einem Index dar."
type: docs
weight: 18
url: /de/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Stellt das Ergebnis der Operation zum Löschen einer indizierten Datei oder eines Ordners aus einem Index dar.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Gibt den Erfolgsindikator der Löschoperation zurück. |
|
|  | [getError()](#getError--) | Gibt eine Beschreibung des Löschfehlers zurück. |
|
|  | [getPath()](#getPath--) | Gibt den Pfad zur zu löschenden Datei oder zum Ordner zurück. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Gibt den Erfolgsindikator der Löschoperation zurück.


**Returns:**
boolean -  true  wenn die Löschoperation erfolgreich war; andernfalls wird  false  zurückgegeben.

### getError() {#getError--}
```
public final String getError()
```


Gibt eine Beschreibung des Löschfehlers zurück.


**Returns:**
java.lang.String - Eine Beschreibung des Löschfehlers.

### getPath() {#getPath--}
```
public final String getPath()
```


Gibt den Pfad zur zu löschenden Datei oder zum Ordner zurück.


**Returns:**
java.lang.String - Der Pfad zur zu löschenden Datei oder zum Ordner.

