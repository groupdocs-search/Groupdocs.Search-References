---
title: "PathDeleteResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt het resultaat van de bewerking om een geïndexeerd bestand of map uit een index te verwijderen voor."
type: docs
weight: 18
url: /nl/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Stelt het resultaat van de bewerking om een geïndexeerd bestand of map uit een index te verwijderen voor.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Geeft de succesindicator van de verwijderingsbewerking terug. |
|
|  | [getError()](#getError--) | Geeft een beschrijving van de verwijderingsfout terug. |
|
|  | [getPath()](#getPath--) | Geeft het pad naar het bestand of de map dat moet worden verwijderd terug. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Geeft de succesindicator van de verwijderingsbewerking terug.


**Returns:**
boolean - true als de verwijderingsbewerking succesvol was; anders wordt false geretourneerd.

### getError() {#getError--}
```
public final String getError()
```


Geeft een beschrijving van de verwijderingsfout terug.


**Returns:**
java.lang.String - Een beschrijving van de verwijderingsfout.

### getPath() {#getPath--}
```
public final String getPath()
```


Geeft het pad naar het bestand of de map dat moet worden verwijderd terug.


**Returns:**
java.lang.String - Het pad naar het bestand of de map die moet worden verwijderd.

