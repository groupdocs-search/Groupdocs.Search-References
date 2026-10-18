---
title: "FragmentContainer"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un contenedor para fragmentos de texto con términos encontrados resaltados de un campo de documento."
type: docs
weight: 22
url: /es/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Representa un contenedor para fragmentos de texto con términos encontrados resaltados de un campo de documento.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructores

| Constructor | Descripción |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Obtiene el nombre del campo del documento. |
|
|  | [getCount()](#getCount--) | Obtiene el número de fragmentos de texto contenidos. |
|
|  | [getFragments()](#getFragments--) | Obtiene un arreglo de fragmentos de texto contenidos. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Obtiene el nombre del campo del documento.


**Returns:**
java.lang.String - El nombre del campo del documento.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtiene el número de fragmentos de texto contenidos.


**Returns:**
int - El número de fragmentos de texto contenidos.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Obtiene un arreglo de fragmentos de texto contenidos.


**Returns:**
java.lang.String[] - Un arreglo de fragmentos de texto contenidos.

