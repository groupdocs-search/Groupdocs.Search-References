---
title: "FragmentContainer"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Container für Textfragmente mit hervorgehobenen gefundenen Begriffen eines Dokumentfeldes dar."
type: docs
weight: 22
url: /de/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Stellt einen Container für Textfragmente mit hervorgehobenen gefundenen Begriffen eines Dokumentfeldes dar.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Liefert den Namen des Dokumentfelds. |
|
|  | [getCount()](#getCount--) | Liefert die Anzahl der enthaltenen Textfragmente. |
|
|  | [getFragments()](#getFragments--) | Liefert ein Array der enthaltenen Textfragmente. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Liefert den Namen des Dokumentfelds.


**Returns:**
java.lang.String - Der Name des Dokumentfelds.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Liefert die Anzahl der enthaltenen Textfragmente.


**Returns:**
int - Die Anzahl der enthaltenen Textfragmente.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Liefert ein Array der enthaltenen Textfragmente.


**Returns:**
java.lang.String[] - Ein Array der enthaltenen Textfragmente.

