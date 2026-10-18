---
title: "DeleteResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar resultatet av operationen för att ta bort indexerade filer eller mappar från ett index."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Representerar resultatet av operationen för att ta bort indexerade filer eller mappar från ett index.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Returnerar resultaten av att ta bort varje sökväg. |
|
|  | [getTotalCount()](#getTotalCount--) | Returnerar det totala antalet sökvägar att ta bort. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Returnerar antalet framgångsrikt borttagna sökvägar. |
|
|  | [getFailedCount()](#getFailedCount--) | Returnerar antalet sökvägar som inte togs bort på grund av fel. |
|
|  | [getErrors()](#getErrors--) | Returnerar beskrivningar av borttagningsfel. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Returnerar resultaten av att ta bort varje sökväg.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Resultaten av att ta bort varje sökväg.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Returnerar det totala antalet sökvägar att ta bort.


**Returns:**
int - Det totala antalet sökvägar att ta bort.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Returnerar antalet framgångsrikt borttagna sökvägar.


**Returns:**
int - Antalet framgångsrikt raderade sökvägar.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Returnerar antalet sökvägar som inte togs bort på grund av fel.


**Returns:**
int - Antalet sökvägar som inte raderades på grund av fel.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Returnerar beskrivningar av borttagningsfel.


**Returns:**
java.lang.String[] - Beskrivningar av raderingsfel.

