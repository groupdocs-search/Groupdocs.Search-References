---
title: DateFormatCollection
second_title: GroupDocs.Search for Java API Reference
description: Represents a collection of DateFormat objects.
type: docs
weight: 14
url: /java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

Represents a collection of  DateFormat  objects.

**Learn more**

 *  [Date range search][]


[Date range search]: https://docs.groupdocs.com/display/searchjava/Date+range+search
## Constructors

| Constructor | Description |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## Methods

| Method | Description |
| --- | --- |
| [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | Adds an date format object to the collection. |
| [clear()](#clear--) | Removes all elements from the collection. |
| [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | Determines whether the collection contains a specific item. |
| [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | Copies the elements of the collection to an  Array , starting at a particular  Array  index. |
| [size()](#size--) | Gets the number of elements contained in the collection. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether the collection is read-only. |
| [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | Removes the first occurrence of a specific element from the collection. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through the collection. |
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


Adds an date format object to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [DateFormat](../../com.groupdocs.search.options/dateformat) | The date format object to add to the collection. |

### clear() {#clear--}
```
public abstract void clear()
```


Removes all elements from the collection.

### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


Determines whether the collection contains a specific item.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [DateFormat](../../com.groupdocs.search.options/dateformat) | The item to locate in the collection. |

**Returns:**
boolean -  true  if item is found in the collection; otherwise,  false .
### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


Copies the elements of the collection to an  Array , starting at a particular  Array  index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | The one-dimensional  Array  that is the destination of the elements copied from the collection. |
| arrayIndex | int | The zero-based index in array at which copying begins. |

### size() {#size--}
```
public abstract int size()
```


Gets the number of elements contained in the collection.

**Returns:**
int - The number of elements contained in the collection.
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Gets a value indicating whether the collection is read-only.

**Returns:**
boolean -  true  if the collection is read-only; otherwise,  false .
### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


Removes the first occurrence of a specific element from the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [DateFormat](../../com.groupdocs.search.options/dateformat) | The item to remove from the collection. |

**Returns:**
boolean -  true  if item was successfully removed from the collection; otherwise,  false . This method also returns  false  if item is not found in the collection.
### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


Returns an enumerator that iterates through the collection.

**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - An enumerator that can be used to iterate through the collection.
