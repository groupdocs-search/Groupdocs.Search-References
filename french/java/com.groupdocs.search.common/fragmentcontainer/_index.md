---
title: "FragmentContainer"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un conteneur pour les fragments de texte avec les termes trouvés mis en surbrillance d'un champ de document."
type: docs
weight: 22
url: /fr/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Représente un conteneur pour les fragments de texte avec les termes trouvés mis en surbrillance d'un champ de document.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Obtient le nom du champ du document. |
|
|  | [getCount()](#getCount--) | Obtient le nombre de fragments de texte contenus. |
|
|  | [getFragments()](#getFragments--) | Obtient un tableau de fragments de texte contenus. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Obtient le nom du champ du document.


**Returns:**
java.lang.String - Le nom du champ du document.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Obtient le nombre de fragments de texte contenus.


**Returns:**
int - Le nombre de fragments de texte contenus.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Obtient un tableau de fragments de texte contenus.


**Returns:**
java.lang.String[] - Un tableau de fragments de texte contenus.

