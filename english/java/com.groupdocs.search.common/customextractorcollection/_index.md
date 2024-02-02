---
title: CustomExtractorCollection
second_title: GroupDocs.Search for Java API Reference
description: Contains a collection of custom extractors.
type: docs
weight: 13
url: /java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

Contains a collection of custom extractors. If the collection contains an extractor for some file extension that is covered by build-in extractors, then this extractor will be used instead of built-in one.

**Learn more**

 *  [Custom text extractors][]


[Custom text extractors]: https://docs.groupdocs.com/display/searchjava/Custom+text+extractors
## Constructors

| Constructor | Description |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## Methods

| Method | Description |
| --- | --- |
| [size()](#size--) | Gets the number of extractors contained in the collection. |
| [isReadOnly()](#isReadOnly--) | Gets a value indicating whether the collection is read-only. |
| [iterator()](#iterator--) | Returns an iterator for this collection. |
| [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | Adds an extractor to the collection. |
| [clear()](#clear--) | Removes all extractors from the collection. |
| [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | Determines whether the collection contains a specific extractor. |
| [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | Copies the elements of the collection to an array, starting at a particular array index. |
| [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | Removes an extractor from the collection. |
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


Gets the number of extractors contained in the collection.

**Returns:**
int - The number of extractors contained in the collection.
### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


Gets a value indicating whether the collection is read-only.

**Returns:**
boolean - A value indicating whether the collection is read-only.
### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


Returns an iterator for this collection.

**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - An iterator object that can be used to iterate through the collection.
### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


Adds an extractor to the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The extractor to add to the collection. |

### clear() {#clear--}
```
public abstract void clear()
```


Removes all extractors from the collection.

### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


Determines whether the collection contains a specific extractor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The extractor to locate in the collection. |

**Returns:**
boolean -  true  if  item  is found in the collection; otherwise,  false .
### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


Copies the elements of the collection to an array, starting at a particular array index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | The one-dimensional array that is the destination of the elements copied from collection. The array must have zero-based indexing. |
| arrayIndex | int | The zero-based index in array at which copying begins. |

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


Removes an extractor from the collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The extractor to remove from the collection. |

**Returns:**
boolean -  true  if  extractor  was successfully removed from the collection; otherwise,  false . This method also returns  false  if  extractor  is not found in the original collection.
