---
title: "FragmentContainer"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en behållare för textfragment med markerade funna termer i ett dokumentfält."
type: docs
weight: 22
url: /sv/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Representerar en behållare för textfragment med markerade funna termer i ett dokumentfält.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Hämtar dokumentfältets namn. |
|
|  | [getCount()](#getCount--) | Hämtar antalet textfragment som ingår. |
|
|  | [getFragments()](#getFragments--) | Hämtar en array av textfragment som ingår. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Hämtar dokumentfältets namn.


**Returns:**
java.lang.String - Dokumentfältets namn.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet textfragment som ingår.


**Returns:**
int - Antalet textfragment som ingår.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Hämtar en array av textfragment som ingår.


**Returns:**
java.lang.String[] - En array av textfragment som ingår.

