---
title: "AliasDictionary"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een aliaswoordenboek."
type: docs
weight: 14
url: /nl/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Definieert de interface van een aliaswoordenboek.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal aliassen op dat in de  AliasDictionary  zit. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Voegt de opgegeven collectie van alias/vervangingsparen toe aan deze instantie van de  AliasDictionary . |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Voegt de opgegeven collectie van alias/vervangingsparen toe aan deze instantie van de  AliasDictionary . |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Voegt het opgegeven paar van alias en bijbehorende tekst toe aan deze instantie van de  AliasDictionary . |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Verwijdert de opgegeven alias uit een  AliasDictionary  object. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Bepaalt of een  AliasDictionary  object de opgegeven alias bevat. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Haalt een tekst op die aan de opgegeven alias is gekoppeld. |
|
|  | [clear()](#clear--) | Verwijdert alle aliassen uit een  AliasDictionary  object. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal aliassen op dat in de  AliasDictionary  zit.


**Returns:**
int - Het aantal aliassen dat in de  AliasDictionary  zit.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Voegt de opgegeven collectie van alias/vervangingsparen toe aan deze instantie van de  AliasDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | paren | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | De collectie van alias/vervangingsparen om toe te voegen aan het woordenboek. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Voegt de opgegeven collectie van alias/vervangingsparen toe aan deze instantie van de  AliasDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | De collectie van alias/vervangingsparen om toe te voegen aan het woordenboek. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Voegt het opgegeven paar van alias en bijbehorende tekst toe aan deze instantie van de  AliasDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | alias | java.lang.String | De alias om toe te voegen aan het woordenboek. |
|
|  | tekst | java.lang.String | De tekst die aan de alias moet worden gekoppeld. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Verwijdert de opgegeven alias uit een  AliasDictionary  object.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | alias | java.lang.String | De alias om te verwijderen. |
|

**Returns:**
boolean - Deze methode retourneert  true  als de alias succesvol wordt gevonden en verwijderd. Deze methode retourneert  false  als de alias niet wordt gevonden in het  AliasDictionary  object.

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Bepaalt of een  AliasDictionary  object de opgegeven alias bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | alias | java.lang.String | De alias om te zoeken in het  AliasDictionary  object. |
|

**Returns:**
boolean -  true  als het  AliasDictionary  object de opgegeven alias bevat; anders,  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Haalt een tekst op die aan de opgegeven alias is gekoppeld.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | alias | java.lang.String | De alias om te zoeken in het  AliasDictionary  object. |
|

**Returns:**
java.lang.String - Een tekst geassocieerd met de opgegeven alias of  null .

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle aliassen uit een  AliasDictionary  object.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.String> - Een iterator die kan worden gebruikt om door de collectie te itereren.

