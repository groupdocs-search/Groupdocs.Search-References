---
title: "FragmentContainer"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un contenitore per frammenti di testo con termini trovati evidenziati di un campo del documento."
type: docs
weight: 22
url: /it/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Rappresenta un contenitore per frammenti di testo con termini trovati evidenziati di un campo del documento.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Restituisce il nome del campo del documento. |
|
|  | [getCount()](#getCount--) | Restituisce il numero di frammenti di testo contenuti. |
|
|  | [getFragments()](#getFragments--) | Restituisce un array di frammenti di testo contenuti. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Restituisce il nome del campo del documento.


**Returns:**
java.lang.String - Il nome del campo del documento.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Restituisce il numero di frammenti di testo contenuti.


**Returns:**
int - Il numero di frammenti di testo contenuti.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Restituisce un array di frammenti di testo contenuti.


**Returns:**
java.lang.String[] - Un array di frammenti di testo contenuti.

