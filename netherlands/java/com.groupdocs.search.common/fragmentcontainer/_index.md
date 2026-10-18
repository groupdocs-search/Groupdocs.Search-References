---
title: "FragmentContainer"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een container voor tekstfragmenten met gemarkeerde gevonden termen van één documentveld voor."
type: docs
weight: 22
url: /nl/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Stelt een container voor tekstfragmenten met gemarkeerde gevonden termen van één documentveld voor.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Haalt de documentveldnaam op. |
|
|  | [getCount()](#getCount--) | Haalt het aantal opgenomen tekstfragmenten op. |
|
|  | [getFragments()](#getFragments--) | Haalt een array van opgenomen tekstfragmenten op. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Haalt de documentveldnaam op.


**Returns:**
java.lang.String - De documentveldnaam.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal opgenomen tekstfragmenten op.


**Returns:**
int - Het aantal opgenomen tekstfragmenten.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Haalt een array van opgenomen tekstfragmenten op.


**Returns:**
java.lang.String[] - Een array van opgenomen tekstfragmenten.

