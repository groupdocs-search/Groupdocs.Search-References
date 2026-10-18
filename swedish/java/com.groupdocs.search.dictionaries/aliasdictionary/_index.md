---
title: "AliasDictionary"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en aliasordbok."
type: docs
weight: 14
url: /sv/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Definierar gränssnittet för en aliasordbok.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet alias som finns i AliasDictionary. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Lägger till den angivna samlingen av alias/ersättningspar till den här instansen av AliasDictionary. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Lägger till den angivna samlingen av alias/ersättningspar till den här instansen av AliasDictionary. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Lägger till det angivna paret av alias och tillhörande text till den här instansen av AliasDictionary. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Tar bort det angivna aliaset från ett AliasDictionary objekt. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Bestämmer om ett AliasDictionary objekt innehåller det angivna aliaset. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Hämtar en text som är associerad med det angivna aliaset. |
|
|  | [clear()](#clear--) | Tar bort alla alias från ett AliasDictionary objekt. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet alias som finns i AliasDictionary.


**Returns:**
int - Antalet alias som finns i AliasDictionary.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Lägger till den angivna samlingen av alias/ersättningspar till den här instansen av AliasDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | par | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | Samlingen av alias/ersättningspar att lägga till i ordboken. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Lägger till den angivna samlingen av alias/ersättningspar till den här instansen av AliasDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | Samlingen av alias/ersättningspar att lägga till i ordboken. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Lägger till det angivna paret av alias och tillhörande text till den här instansen av AliasDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | alias | java.lang.String | Aliaset att lägga till i ordboken. |
|
|  | text | java.lang.String | Texten som ska associeras med aliaset. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Tar bort det angivna aliaset från ett AliasDictionary objekt.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | alias | java.lang.String | Aliaset att ta bort. |
|

**Returns:**
boolean - Denna metod returnerar  true  om aliaset hittas och tas bort. Metoden returnerar  false  om aliaset inte hittas i  AliasDictionary  -objektet.

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Bestämmer om ett AliasDictionary objekt innehåller det angivna aliaset.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | alias | java.lang.String | Aliaset att lokalisera i  AliasDictionary  -objektet. |
|

**Returns:**
boolean -  true  om  AliasDictionary  -objektet innehåller det angivna aliaset; annars  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Hämtar en text som är associerad med det angivna aliaset.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | alias | java.lang.String | Aliaset att lokalisera i  AliasDictionary  -objektet. |
|

**Returns:**
java.lang.String - En text associerad med det angivna aliaset eller  null .

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla alias från ett AliasDictionary objekt.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.String> - En iterator som kan användas för att iterera genom samlingen.

