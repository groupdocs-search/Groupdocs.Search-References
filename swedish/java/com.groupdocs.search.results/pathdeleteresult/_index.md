---
title: "PathDeleteResult"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar resultatet av operationen att ta bort en indexerad fil eller mapp från ett index."
type: docs
weight: 18
url: /sv/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Representerar resultatet av operationen att ta bort en indexerad fil eller mapp från ett index.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | Returnerar indikatorn för om raderingsoperationen lyckades. |
|
|  | [getError()](#getError--) | Returnerar en beskrivning av raderingsfelet. |
|
|  | [getPath()](#getPath--) | Returnerar sökvägen till filen eller mappen som ska raderas. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Returnerar indikatorn för om raderingsoperationen lyckades.


**Returns:**
boolean -  true  om raderingsoperationen lyckades; annars returneras  false .

### getError() {#getError--}
```
public final String getError()
```


Returnerar en beskrivning av raderingsfelet.


**Returns:**
java.lang.String - En beskrivning av raderingsfelet.

### getPath() {#getPath--}
```
public final String getPath()
```


Returnerar sökvägen till filen eller mappen som ska raderas.


**Returns:**
java.lang.String - Sökvägen till filen eller mappen som ska raderas.

