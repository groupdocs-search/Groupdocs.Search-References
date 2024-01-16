---
title: AliasDictionary
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a dictionary of aliases.
type: docs
weight: 14
url: /java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Defines interface of a dictionary of aliases.

**Learn more**

 *  [Using aliases][]
 *  [Managing alias dictionary][]


[Using aliases]: https://docs.groupdocs.com/display/searchjava/Using+aliases
[Managing alias dictionary]: https://docs.groupdocs.com/display/searchjava/Alias+dictionary
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of aliases contained in the  AliasDictionary . |
| [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Adds the specified collection of alias/replacement pairs to this instance of the  AliasDictionary . |
| [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Adds the specified collection of alias/replacement pairs to this instance of the  AliasDictionary . |
| [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Adds the specified pair of alias and associated text to this instance of the  AliasDictionary . |
| [remove(String alias)](#remove-java.lang.String-) | Removes the specified alias from an  AliasDictionary  object. |
| [contains(String alias)](#contains-java.lang.String-) | Determines whether an  AliasDictionary  object contains the specified alias. |
| [getText(String alias)](#getText-java.lang.String-) | Gets a text that is associated with the specified alias. |
| [clear()](#clear--) | Removes all aliases from a  AliasDictionary  object. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of aliases contained in the  AliasDictionary .

**Returns:**
int - The number of aliases contained in the  AliasDictionary .
### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Adds the specified collection of alias/replacement pairs to this instance of the  AliasDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pairs | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | The collection of alias/replacement pairs to add to the dictionary. |

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Adds the specified collection of alias/replacement pairs to this instance of the  AliasDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | The collection of alias/replacement pairs to add to the dictionary. |

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Adds the specified pair of alias and associated text to this instance of the  AliasDictionary .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| alias | java.lang.String | The alias to add to the dictionary. |
| text | java.lang.String | The text to be associated with the alias. |

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Removes the specified alias from an  AliasDictionary  object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| alias | java.lang.String | The alias to remove. |

**Returns:**
boolean - This method returns  true  if the alias is successfully found and removed. This method returns  false  if the alias is not found in the  AliasDictionary  object.
### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Determines whether an  AliasDictionary  object contains the specified alias.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| alias | java.lang.String | The alias to locate in the  AliasDictionary  object. |

**Returns:**
boolean -  true  if the  AliasDictionary  object contains the specified alias; otherwise,  false .
### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Gets a text that is associated with the specified alias.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| alias | java.lang.String | The alias to locate in the  AliasDictionary  object. |

**Returns:**
java.lang.String - A text associated with the specified alias or  null .
### clear() {#clear--}
```
public abstract void clear()
```


Removes all aliases from a  AliasDictionary  object.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.String> - An iterator that can be used to iterate through the collection.
