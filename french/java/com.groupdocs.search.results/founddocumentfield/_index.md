---
title: "FoundDocumentField"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un champ de document trouvé."
type: docs
weight: 15
url: /fr/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

Représente un champ de document trouvé.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | Obtient le nom du champ. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | Obtient le nombre d'occurrences trouvées. |
|
|  | [getTerms()](#getTerms--) | Obtient les termes trouvés. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | Obtient les occurrences des termes trouvés. |
|
|  | [getTermSequences()](#getTermSequences--) | Obtient les séquences de termes trouvées. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | Obtient les occurrences des séquences de termes trouvées. |
|
|  | [toString()](#toString--) | Renvoie la représentation sous forme de chaîne du champ de document trouvé. |
|
|  | [serialize()](#serialize--) | Sérialise l'instance actuelle en un tableau d'octets. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | Désérialise une instance à partir d'un tableau d'octets. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Obtient le nom du champ.


**Returns:**
java.lang.String - Le nom du champ.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


Obtient le nombre d'occurrences trouvées.


**Returns:**
int - Le nombre d'occurrences trouvées.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


Obtient les termes trouvés.


**Returns:**
java.lang.String[] - Les termes trouvés.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


Obtient les occurrences des termes trouvés.


**Returns:**
int[] - Les occurrences des termes trouvés.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


Obtient les séquences de termes trouvées.


**Returns:**
java.lang.String[][] - Les séquences de termes trouvées.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


Obtient les occurrences des séquences de termes trouvées.


**Returns:**
int[] - Les occurrences des séquences de termes trouvées.

### toString() {#toString--}
```
public abstract String toString()
```


Renvoie la représentation sous forme de chaîne du champ de document trouvé.


**Returns:**
java.lang.String - Une chaîne qui représente le champ de document trouvé.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


Sérialise l'instance actuelle en un tableau d'octets.


**Returns:**
byte[] - Un tableau d'octets représentant l'instance actuelle.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


Désérialise une instance à partir d'un tableau d'octets.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | tableau | byte[] | Un tableau d'octets à désérialiser. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

