---
title: "PasswordDictionary"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een woordenboek van documentwachtwoorden."
type: docs
weight: 20
url: /nl/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Definieert de interface van een woordenboek van documentwachtwoorden.


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal elementen op dat in het woordenboek is opgenomen. |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | Haalt het wachtwoord voor het bestand op. |
|
|  | [clear()](#clear--) | Verwijdert alle wachtwoorden uit dit  PasswordDictionary  object. |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | Bepaalt of het woordenboek een wachtwoord bevat voor het opgegeven document. |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Voegt een wachtwoord voor een document toe aan het woordenboek. |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | Verwijdert een wachtwoord van het opgegeven document uit het woordenboek. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal elementen op dat in het woordenboek is opgenomen.


**Returns:**
int - Het aantal elementen dat in het woordenboek is opgenomen.

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Haalt het wachtwoord voor het bestand op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestandspad. |
|

**Returns:**
java.lang.String - Het wachtwoord voor het bestand.

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle wachtwoorden uit dit  PasswordDictionary  object.


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Bepaalt of het woordenboek een wachtwoord bevat voor het opgegeven document.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestandspad van het document. |
|

**Returns:**
boolean -  true  als het woordenboek een wachtwoord bevat voor het document; anders,  false .

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Voegt een wachtwoord voor een document toe aan het woordenboek.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestandspad van het document. |
|
|  | wachtwoord | java.lang.String | Het documentwachtwoord. |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Verwijdert een wachtwoord van het opgegeven document uit het woordenboek.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | filePath | java.lang.String | Het bestandspad van het document. |
|

**Returns:**
boolean -  true  als het wachtwoord succesvol is verwijderd; anders,  false . Deze methode retourneert ook  false  als  filePath  niet in het woordenboek werd gevonden.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.String> - Een iterator die kan worden gebruikt om door de collectie te itereren.

