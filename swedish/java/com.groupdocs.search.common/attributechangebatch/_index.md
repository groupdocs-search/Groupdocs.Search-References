---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en behållare för attributändringar."
type: docs
weight: 10
url: /sv/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Representerar en behållare för attributändringar.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Initierar en ny instans av klassen  AttributeChangeBatch  . |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Initierar en ny instans av klassen  AttributeChangeBatch  . |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Lägger till de angivna attributen i det angivna indexerade dokumentet. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Lägger till de angivna attributen i de angivna indexerade dokumenten. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Lägger till de angivna attributen till alla dokument i indexet. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Tar bort de angivna attributen från det angivna indexerade dokumentet. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Tar bort de angivna attributen från de angivna indexerade dokumenten. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Tar bort alla attribut från det angivna indexerade dokumentet. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Tar bort alla attribut från de angivna indexerade dokumenten. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Tar bort de angivna attributen från alla dokument i indexet. |
|
|  | [clear()](#clear--) | Tar bort alla attribut från alla dokument i indexet. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Initierar en ny instans av klassen  AttributeChangeBatch  .


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Initierar en ny instans av klassen  AttributeChangeBatch  .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | data | java.lang.Object | Den serialiserade datan. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Lägger till de angivna attributen i det angivna indexerade dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökväg | java.lang.String | Dokumentets sökväg. |
|
|  | attribut | java.lang.String[] | Attributen att lägga till. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Lägger till de angivna attributen i de angivna indexerade dokumenten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökvägar | java.lang.String[] | Dokumentens sökvägar. |
|
|  | attribut | java.lang.String[] | Attributen att lägga till. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Lägger till de angivna attributen till alla dokument i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | attribut | java.lang.String[] | Attributen att lägga till. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Tar bort de angivna attributen från det angivna indexerade dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökväg | java.lang.String | Dokumentets sökväg. |
|
|  | attribut | java.lang.String[] | Attributen att ta bort. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Tar bort de angivna attributen från de angivna indexerade dokumenten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökvägar | java.lang.String[] | Dokumentens sökvägar. |
|
|  | attribut | java.lang.String[] | Attributen att ta bort. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Tar bort alla attribut från det angivna indexerade dokumentet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökväg | java.lang.String | Dokumentets sökväg. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Tar bort alla attribut från de angivna indexerade dokumenten.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | sökvägar | java.lang.String[] | Dokumentens sökvägar. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Tar bort de angivna attributen från alla dokument i indexet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | attribut | java.lang.String[] | Attributen att ta bort. |
|

### clear() {#clear--}
```
public void clear()
```


Tar bort alla attribut från alla dokument i indexet.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
