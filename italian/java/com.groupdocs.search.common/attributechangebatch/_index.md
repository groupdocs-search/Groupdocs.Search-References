---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un contenitore per le modifiche agli attributi."
type: docs
weight: 10
url: /it/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

Rappresenta un contenitore per le modifiche agli attributi.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | Inizializza una nuova istanza della classe  AttributeChangeBatch  . |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | Inizializza una nuova istanza della classe  AttributeChangeBatch  . |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | Aggiunge gli attributi specificati al documento indicizzato specificato. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | Aggiunge gli attributi specificati ai documenti indicizzati specificati. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | Aggiunge gli attributi specificati a tutti i documenti nell'indice. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | Rimuove gli attributi specificati dal documento indicizzato specificato. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | Rimuove gli attributi specificati dai documenti indicizzati specificati. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | Rimuove tutti gli attributi dal documento indicizzato specificato. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | Rimuove tutti gli attributi dai documenti indicizzati specificati. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | Rimuove gli attributi specificati da tutti i documenti nell'indice. |
|
|  | [clear()](#clear--) | Rimuove tutti gli attributi da tutti i documenti nell'indice. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


Inizializza una nuova istanza della classe  AttributeChangeBatch  .


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


Inizializza una nuova istanza della classe  AttributeChangeBatch  .


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | dati | java.lang.Object | I dati serializzati. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


Aggiunge gli attributi specificati al documento indicizzato specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | percorso | java.lang.String | Il percorso del documento. |
|
|  | attributi | java.lang.String[] | Gli attributi da aggiungere. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


Aggiunge gli attributi specificati ai documenti indicizzati specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | paths | java.lang.String[] | I percorsi dei documenti. |
|
|  | attributi | java.lang.String[] | Gli attributi da aggiungere. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


Aggiunge gli attributi specificati a tutti i documenti nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | attributi | java.lang.String[] | Gli attributi da aggiungere. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


Rimuove gli attributi specificati dal documento indicizzato specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | percorso | java.lang.String | Il percorso del documento. |
|
|  | attributi | java.lang.String[] | Gli attributi da rimuovere. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


Rimuove gli attributi specificati dai documenti indicizzati specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | paths | java.lang.String[] | I percorsi dei documenti. |
|
|  | attributi | java.lang.String[] | Gli attributi da rimuovere. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


Rimuove tutti gli attributi dal documento indicizzato specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | percorso | java.lang.String | Il percorso del documento. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


Rimuove tutti gli attributi dai documenti indicizzati specificati.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | paths | java.lang.String[] | I percorsi dei documenti. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


Rimuove gli attributi specificati da tutti i documenti nell'indice.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | attributi | java.lang.String[] | Gli attributi da rimuovere. |
|

### clear() {#clear--}
```
public void clear()
```


Rimuove tutti gli attributi da tutti i documenti nell'indice.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
