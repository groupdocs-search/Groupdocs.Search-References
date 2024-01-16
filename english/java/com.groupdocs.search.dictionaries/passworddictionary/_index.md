---
title: PasswordDictionary
second_title: GroupDocs.Search for Java API Reference
description: Defines interface of a dictionary of document passwords.
type: docs
weight: 20
url: /java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

Defines interface of a dictionary of document passwords.

**Learn more**

 *  [Indexing password protected documents][]
 *  [Managing document passwords][]


[Indexing password protected documents]: https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents
[Managing document passwords]: https://docs.groupdocs.com/display/searchjava/Document+passwords
## Methods

| Method | Description |
| --- | --- |
| [getCount()](#getCount--) | Gets the number of elements contained in the dictionary. |
| [getPassword(String filePath)](#getPassword-java.lang.String-) | Gets the password for the file. |
| [clear()](#clear--) | Removes all passwords from this  PasswordDictionary  object. |
| [contains(String filePath)](#contains-java.lang.String-) | Determines whether the dictionary contains a password for the specified document. |
| [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | Adds a password for a document to the dictionary. |
| [remove(String filePath)](#remove-java.lang.String-) | Removes a password of the specified document from the dictionary. |
| [iterator()](#iterator--) | Returns an iterator that iterates through the collection. |
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of elements contained in the dictionary.

**Returns:**
int - The number of elements contained in the dictionary.
### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


Gets the password for the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

**Returns:**
java.lang.String - The password for the file.
### clear() {#clear--}
```
public abstract void clear()
```


Removes all passwords from this  PasswordDictionary  object.

### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


Determines whether the dictionary contains a password for the specified document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The document file path. |

**Returns:**
boolean -  true  if the dictionary contains a password for the document; otherwise,  false .
### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


Adds a password for a document to the dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The document file path. |
| password | java.lang.String | The document password. |

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


Removes a password of the specified document from the dictionary.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The document file path. |

**Returns:**
boolean -  true  if the password was successfully removed; otherwise,  false . This method also returns  false  if  filePath  was not found in the dictionary.
### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returns an iterator that iterates through the collection.

**Returns:**
java.util.Iterator<java.lang.String> - An iterator that can be used to iterate through the collection.
