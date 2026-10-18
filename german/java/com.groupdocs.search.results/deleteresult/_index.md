---
title: "DeleteResult"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt das Ergebnis der Operation zum Löschen indizierter Dateien oder Ordner aus einem Index dar."
type: docs
weight: 10
url: /de/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Stellt das Ergebnis der Operation zum Löschen indizierter Dateien oder Ordner aus einem Index dar.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Gibt die Ergebnisse des Löschens jedes Pfads zurück. |
|
|  | [getTotalCount()](#getTotalCount--) | Gibt die Gesamtzahl der zu löschenden Pfade zurück. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Gibt die Anzahl der erfolgreich gelöschten Pfade zurück. |
|
|  | [getFailedCount()](#getFailedCount--) | Gibt die Anzahl der aufgrund von Fehlern nicht gelöschten Pfade zurück. |
|
|  | [getErrors()](#getErrors--) | Gibt Beschreibungen der Löschfehler zurück. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Gibt die Ergebnisse des Löschens jedes Pfads zurück.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Die Ergebnisse des Löschens jedes Pfads.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Gibt die Gesamtzahl der zu löschenden Pfade zurück.


**Returns:**
int - Die Gesamtzahl der zu löschenden Pfade.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Gibt die Anzahl der erfolgreich gelöschten Pfade zurück.


**Returns:**
int - Die Anzahl der erfolgreich gelöschten Pfade.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Gibt die Anzahl der aufgrund von Fehlern nicht gelöschten Pfade zurück.


**Returns:**
int - Die Anzahl der Pfade, die aufgrund von Fehlern nicht gelöscht wurden.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Gibt Beschreibungen der Löschfehler zurück.


**Returns:**
java.lang.String[] - Beschreibungen der Löschfehler.

