---
title: FragmentContainer
second_title: GroupDocs.Search for Java API Reference
description: Represents a container for text fragments with highlighted found terms of one document field.
type: docs
weight: 24
url: /java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

Represents a container for text fragments with highlighted found terms of one document field.

**Learn more**

 *  [Highlighting search results][]


[Highlighting search results]: https://docs.groupdocs.com/display/searchjava/Highlighting+search+results
## Methods

| Method | Description |
| --- | --- |
| [getFieldName()](#getFieldName--) | Gets the document field name. |
| [getCount()](#getCount--) | Gets the number of contained text fragments. |
| [getFragments()](#getFragments--) | Gets an array of contained text fragments. |
### getFieldName() {#getFieldName--}
```
public final String getFieldName()
```


Gets the document field name.

**Returns:**
java.lang.String - The document field name.
### getCount() {#getCount--}
```
public final int getCount()
```


Gets the number of contained text fragments.

**Returns:**
int - The number of contained text fragments.
### getFragments() {#getFragments--}
```
public final String[] getFragments()
```


Gets an array of contained text fragments.

**Returns:**
java.lang.String[] - An array of contained text fragments.
