---
title: "DeleteResult"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt het resultaat van de bewerking om geïndexeerde bestanden of mappen uit een index te verwijderen voor."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Stelt het resultaat van de bewerking om geïndexeerde bestanden of mappen uit een index te verwijderen voor.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Retourneert de resultaten van het verwijderen van elk pad. |
|
|  | [getTotalCount()](#getTotalCount--) | Retourneert het totale aantal paden om te verwijderen. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Retourneert het aantal succesvol verwijderde paden. |
|
|  | [getFailedCount()](#getFailedCount--) | Retourneert het aantal paden dat niet is verwijderd vanwege fouten. |
|
|  | [getErrors()](#getErrors--) | Retourneert beschrijvingen van verwijderingsfouten. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Retourneert de resultaten van het verwijderen van elk pad.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - De resultaten van het verwijderen van elk pad.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Retourneert het totale aantal paden om te verwijderen.


**Returns:**
int - Het totale aantal paden om te verwijderen.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Retourneert het aantal succesvol verwijderde paden.


**Returns:**
int - Het aantal succesvol verwijderde paden.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Retourneert het aantal paden dat niet is verwijderd vanwege fouten.


**Returns:**
int - Het aantal paden dat niet is verwijderd vanwege fouten.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Retourneert beschrijvingen van verwijderingsfouten.


**Returns:**
java.lang.String[] - Beschrijvingen van verwijderingsfouten.

