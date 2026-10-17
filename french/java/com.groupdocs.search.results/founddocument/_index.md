---
title: "FoundDocument"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un document trouvé."
type: docs
weight: 14
url: /fr/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

Représente un document trouvé.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | Obtient les informations du document. |
|
|  | [getRelevance()](#getRelevance--) | Obtient la pertinence du résultat de recherche. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtient le nombre d'occurrences trouvées. |
|
|  | [getFoundFields()](#getFoundFields--) | Obtient les champs de document trouvés. |
|
|  | [getTerms()](#getTerms--) | Obtient les termes trouvés. |
|
|  | [getTermSequences()](#getTermSequences--) | Obtient les séquences de termes trouvées. |
|
|  | [getAttributes()](#getAttributes--) | Obtient les attributs associés au document trouvé. |
|
|  | [toString()](#toString--) | Renvoie la représentation sous forme de chaîne du document trouvé. |
|
|  | [serialize()](#serialize--) | Sérialise l'instance actuelle en un tableau d'octets. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Désérialise une instance à partir d'un tableau d'octets. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


Obtient les informations du document.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


Obtient la pertinence du résultat de recherche.


**Returns:**
double - La pertinence du résultat de recherche.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtient le nombre d'occurrences trouvées.


**Returns:**
int - Le nombre d'occurrences trouvées.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


Obtient les champs de document trouvés.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - Les champs de document trouvés.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Obtient les termes trouvés. La valeur est évaluée chaque fois que la propriété est accédée.


**Returns:**
java.lang.String[] - Les termes trouvés.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Obtient les séquences de termes trouvées.


**Returns:**
java.lang.String[][] - Les séquences de termes trouvées.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


Obtient les attributs associés au document trouvé. L'option correspondante doit être activée dans les options de recherche pour récupérer les attributs.


**Returns:**
java.lang.String[] - Les attributs associés au document trouvé.

### toString() {#toString--}
```
public abstract String toString()
```


Renvoie la représentation sous forme de chaîne du document trouvé.


**Returns:**
java.lang.String - Une chaîne qui représente le document trouvé.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Sérialise l'instance actuelle en un tableau d'octets.


**Returns:**
byte[] - Un tableau d'octets représentant l'instance actuelle.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


Désérialise une instance à partir d'un tableau d'octets.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | tableau | byte[] | Un tableau d'octets à désérialiser. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

