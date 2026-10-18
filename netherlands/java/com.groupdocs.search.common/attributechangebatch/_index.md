---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een container voor attribuutwijzigingen voor."
type: docs
weight: 10
url: /nl/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Stelt een container voor attribuutwijzigingen voor.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Initialiseert een nieuw exemplaar van de  AttributeChangeBatch  klasse. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Initialiseert een nieuw exemplaar van de  AttributeChangeBatch  klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Voegt de opgegeven attributen toe aan het opgegeven geïndexeerde document. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Voegt de opgegeven attributen toe aan de opgegeven geïndexeerde documenten. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Voegt de opgegeven attributen toe aan alle documenten in de index. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Verwijdert de opgegeven attributen van het opgegeven geïndexeerde document. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Verwijdert de opgegeven attributen van de opgegeven geïndexeerde documenten. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Verwijdert alle attributen van het opgegeven geïndexeerde document. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Verwijdert alle attributen van de opgegeven geïndexeerde documenten. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Verwijdert de opgegeven attributen van alle documenten in de index. |
|
|  | [clear()](#clear--) | Verwijdert alle attributen van alle documenten in de index. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Initialiseert een nieuw exemplaar van de  AttributeChangeBatch  klasse.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Initialiseert een nieuw exemplaar van de  AttributeChangeBatch  klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | gegevens | java.lang.Object | De geserialiseerde gegevens. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Voegt de opgegeven attributen toe aan het opgegeven geïndexeerde document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pad | java.lang.String | Het documentpad. |
|
|  | attributen | java.lang.String[] | De attributen om toe te voegen. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Voegt de opgegeven attributen toe aan de opgegeven geïndexeerde documenten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paths | java.lang.String[] | De paden van de documenten. |
|
|  | attributen | java.lang.String[] | De attributen om toe te voegen. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Voegt de opgegeven attributen toe aan alle documenten in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | attributen | java.lang.String[] | De attributen om toe te voegen. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Verwijdert de opgegeven attributen van het opgegeven geïndexeerde document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pad | java.lang.String | Het documentpad. |
|
|  | attributen | java.lang.String[] | De attributen om te verwijderen. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Verwijdert de opgegeven attributen van de opgegeven geïndexeerde documenten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paths | java.lang.String[] | De paden van de documenten. |
|
|  | attributen | java.lang.String[] | De attributen om te verwijderen. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Verwijdert alle attributen van het opgegeven geïndexeerde document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pad | java.lang.String | Het documentpad. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Verwijdert alle attributen van de opgegeven geïndexeerde documenten.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paths | java.lang.String[] | De paden van de documenten. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Verwijdert de opgegeven attributen van alle documenten in de index.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | attributen | java.lang.String[] | De attributen om te verwijderen. |
|

### clear() {#clear--}
```
public void clear()
```


Verwijdert alle attributen van alle documenten in de index.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
