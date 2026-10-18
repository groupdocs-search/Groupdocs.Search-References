---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een tekenvervangingswoordenboek dat tijdens het indexeerproces wordt gebruikt."
type: docs
weight: 16
url: /nl/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Definieert de interface van een tekenvervangingswoordenboek dat wordt gebruikt tijdens het indexeerproces. Tekenvervanging kan bijvoorbeeld worden gebruikt om accenten van geaccentueerde tekens te verwijderen of om een hoofdletterongevoelige index te maken.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal tekens op dat in dit  CharacterReplacementDictionary  zit. |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Voegt de opgegeven collectie van tekenvervangingen toe aan deze instantie van het  CharacterReplacementDictionary . |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Voegt de opgegeven collectie van tekenvervangingen toe aan deze instantie van het  CharacterReplacementDictionary . |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Verwijdert de opgegeven collectie tekenvervangingen van deze instantie van de  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | Bepaalt of een  CharacterReplacementDictionary  object een vervanging bevat voor het opgegeven teken. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Haalt een vervanging op voor het opgegeven teken. |
|
|  | [clear()](#clear--) | Verwijdert alle tekenvervangingen uit een  CharacterReplacementDictionary  object. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal tekens op dat in dit  CharacterReplacementDictionary  zit.


**Returns:**
int - Het aantal tekens in het woordenboek.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Voegt de opgegeven collectie van tekenvervangingen toe aan deze instantie van het  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | De collectie tekenvervangingen die aan het woordenboek moet worden toegevoegd. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Voegt de opgegeven collectie van tekenvervangingen toe aan deze instantie van het  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | De collectie tekenvervangingen die aan het woordenboek moet worden toegevoegd. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Verwijdert de opgegeven collectie tekenvervangingen van deze instantie van de  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekens | char[] | De collectie tekens die verwijderd moeten worden. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Bepaalt of een  CharacterReplacementDictionary  object een vervanging bevat voor het opgegeven teken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | teken | char | Het teken dat moet worden opgezocht in het  CharacterReplacementDictionary  object. |
|

**Returns:**
boolean -  true  als het  CharacterReplacementDictionary  object het opgegeven teken bevat; anders,  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Haalt een vervanging op voor het opgegeven teken.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | teken | char | Het teken waarvoor een vervanging moet worden opgehaald. |
|

**Returns:**
char - De vervanging voor het opgegeven teken.

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle tekenvervangingen uit een  CharacterReplacementDictionary  object.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.Character> - Een iterator die kan worden gebruikt om door de collectie te itereren.

