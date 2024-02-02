---
title: FragmentContainer
second_title: GroupDocs.Search for Java API Reference
description: Represents a container for text fragments with highlighted found terms of one document field.
type: docs
weight: 22
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
## Constructors

| Constructor | Description |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getFieldName()](#getFieldName--) | Gets the document field name. |
| [getCount()](#getCount--) | Gets the number of contained text fragments. |
| [getFragments()](#getFragments--) | Gets an array of contained text fragments. |
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


Gets the document field name.

**Returns:**
java.lang.String - The document field name.
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gets the number of contained text fragments.

**Returns:**
int - The number of contained text fragments.
### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


Gets an array of contained text fragments.

**Returns:**
java.lang.String[] - An array of contained text fragments.
