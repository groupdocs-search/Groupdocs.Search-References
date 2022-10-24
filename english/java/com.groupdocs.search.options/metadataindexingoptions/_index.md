---
title: MetadataIndexingOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for indexing metadata fields.
type: docs
weight: 27
url: /java/com.groupdocs.search.options/metadataindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class MetadataIndexingOptions
```

Provides options for indexing metadata fields.

**Learn more**

 *  [Indexing options][]
 *  MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents][]
 *  MetadataIndexingOptions are used when highlighting search results: [Highlighting search results][]


[Indexing options]: https://docs.groupdocs.com/display/searchjava/Indexing+options
[Getting indexed documents]: https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents
[Highlighting search results]: https://docs.groupdocs.com/display/searchjava/Highlighting+search+results
## Methods

| Method | Description |
| --- | --- |
| [getIndexingEmptyValues()](#getIndexingEmptyValues--) | Gets a value indicating whether to index empty field values or not. |
| [setIndexingEmptyValues(boolean value)](#setIndexingEmptyValues-boolean-) | Sets a value indicating whether to index empty field values or not. |
| [getIndexingEmptyNames()](#getIndexingEmptyNames--) | Gets a value indicating whether to index empty field names or not. |
| [setIndexingEmptyNames(boolean value)](#setIndexingEmptyNames-boolean-) | Sets a value indicating whether to index empty field names or not. |
| [getDefaultFieldName()](#getDefaultFieldName--) | Gets the default field name used to index empty field names. |
| [setDefaultFieldName(String value)](#setDefaultFieldName-java.lang.String-) | Sets the default field name used to index empty field names. |
| [getSeparatorInCompoundName()](#getSeparatorInCompoundName--) | Gets the separator in the compound name of a field. |
| [setSeparatorInCompoundName(String value)](#setSeparatorInCompoundName-java.lang.String-) | Sets the separator in the compound name of a field. |
| [getMaxBytesToIndexField()](#getMaxBytesToIndexField--) | Gets the maximum number of values in an array of type byte to index the field. |
| [setMaxBytesToIndexField(int value)](#setMaxBytesToIndexField-int-) | Sets the maximum number of values in an array of type byte to index the field. |
| [getMaxIntsToIndexField()](#getMaxIntsToIndexField--) | Gets the maximum number of values in an array of type int to index the field. |
| [setMaxIntsToIndexField(int value)](#setMaxIntsToIndexField-int-) | Sets the maximum number of values in an array of type int to index the field. |
| [getMaxLongsToIndexField()](#getMaxLongsToIndexField--) | Gets the maximum number of values in an array of type long to index the field. |
| [setMaxLongsToIndexField(int value)](#setMaxLongsToIndexField-int-) | Sets the maximum number of values in an array of type long to index the field. |
| [getMaxDoublesToIndexField()](#getMaxDoublesToIndexField--) | Gets the maximum number of values in an array of type double to index the field. |
| [setMaxDoublesToIndexField(int value)](#setMaxDoublesToIndexField-int-) | Sets the maximum number of values in an array of type double to index the field. |
| [getSeparatorBetweenValues()](#getSeparatorBetweenValues--) | Gets the separator between values in a field of type array. |
| [setSeparatorBetweenValues(String value)](#setSeparatorBetweenValues-java.lang.String-) | Sets the separator between values in a field of type array. |
### getIndexingEmptyValues() {#getIndexingEmptyValues--}
```
public final boolean getIndexingEmptyValues()
```


Gets a value indicating whether to index empty field values or not. The default value is  true .

**Returns:**
boolean - A value indicating whether to index empty field values or not.
### setIndexingEmptyValues(boolean value) {#setIndexingEmptyValues-boolean-}
```
public final void setIndexingEmptyValues(boolean value)
```


Sets a value indicating whether to index empty field values or not. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to index empty field values or not. |

### getIndexingEmptyNames() {#getIndexingEmptyNames--}
```
public final boolean getIndexingEmptyNames()
```


Gets a value indicating whether to index empty field names or not. The default value is  true .

**Returns:**
boolean - A value indicating whether to index empty field names or not.
### setIndexingEmptyNames(boolean value) {#setIndexingEmptyNames-boolean-}
```
public final void setIndexingEmptyNames(boolean value)
```


Sets a value indicating whether to index empty field names or not. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to index empty field names or not. |

### getDefaultFieldName() {#getDefaultFieldName--}
```
public final String getDefaultFieldName()
```


Gets the default field name used to index empty field names. The default value is  "unknown" .

**Returns:**
java.lang.String - The default field name used to index empty field names.
### setDefaultFieldName(String value) {#setDefaultFieldName-java.lang.String-}
```
public final void setDefaultFieldName(String value)
```


Sets the default field name used to index empty field names. The default value is  "unknown" .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The default field name used to index empty field names. |

### getSeparatorInCompoundName() {#getSeparatorInCompoundName--}
```
public final String getSeparatorInCompoundName()
```


Gets the separator in the compound name of a field. The default value is  "." .

**Returns:**
java.lang.String - The separator in the compound name of a field.
### setSeparatorInCompoundName(String value) {#setSeparatorInCompoundName-java.lang.String-}
```
public final void setSeparatorInCompoundName(String value)
```


Sets the separator in the compound name of a field. The default value is  "." .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The separator in the compound name of a field. |

### getMaxBytesToIndexField() {#getMaxBytesToIndexField--}
```
public final int getMaxBytesToIndexField()
```


Gets the maximum number of values in an array of type byte to index the field. The default value is  Integer.MAX\_VALUE .

**Returns:**
int - The maximum number of values in an array of type byte to index the field.
### setMaxBytesToIndexField(int value) {#setMaxBytesToIndexField-int-}
```
public final void setMaxBytesToIndexField(int value)
```


Sets the maximum number of values in an array of type byte to index the field. The default value is  Integer.MAX\_VALUE .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of values in an array of type byte to index the field. |

### getMaxIntsToIndexField() {#getMaxIntsToIndexField--}
```
public final int getMaxIntsToIndexField()
```


Gets the maximum number of values in an array of type int to index the field. The default value is  Integer.MAX\_VALUE .

**Returns:**
int - The maximum number of values in an array of type int to index the field.
### setMaxIntsToIndexField(int value) {#setMaxIntsToIndexField-int-}
```
public final void setMaxIntsToIndexField(int value)
```


Sets the maximum number of values in an array of type int to index the field. The default value is  Integer.MAX\_VALUE .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of values in an array of type int to index the field. |

### getMaxLongsToIndexField() {#getMaxLongsToIndexField--}
```
public final int getMaxLongsToIndexField()
```


Gets the maximum number of values in an array of type long to index the field. The default value is  Integer.MAX\_VALUE .

**Returns:**
int - The maximum number of values in an array of type long to index the field.
### setMaxLongsToIndexField(int value) {#setMaxLongsToIndexField-int-}
```
public final void setMaxLongsToIndexField(int value)
```


Sets the maximum number of values in an array of type long to index the field. The default value is  Integer.MAX\_VALUE .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of values in an array of type long to index the field. |

### getMaxDoublesToIndexField() {#getMaxDoublesToIndexField--}
```
public final int getMaxDoublesToIndexField()
```


Gets the maximum number of values in an array of type double to index the field. The default value is  Integer.MAX\_VALUE .

**Returns:**
int - The maximum number of values in an array of type double to index the field.
### setMaxDoublesToIndexField(int value) {#setMaxDoublesToIndexField-int-}
```
public final void setMaxDoublesToIndexField(int value)
```


Sets the maximum number of values in an array of type double to index the field. The default value is  Integer.MAX\_VALUE .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of values in an array of type double to index the field. |

### getSeparatorBetweenValues() {#getSeparatorBetweenValues--}
```
public final String getSeparatorBetweenValues()
```


Gets the separator between values in a field of type array. The default value is the space sign.

**Returns:**
java.lang.String - The separator between values in a field of type array.
### setSeparatorBetweenValues(String value) {#setSeparatorBetweenValues-java.lang.String-}
```
public final void setSeparatorBetweenValues(String value)
```


Sets the separator between values in a field of type array. The default value is the space sign.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The separator between values in a field of type array. |

