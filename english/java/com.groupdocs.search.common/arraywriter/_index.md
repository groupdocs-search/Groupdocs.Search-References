---
title: ArrayWriter
second_title: GroupDocs.Search for Java API Reference
description: Represents a byte array data writer.
type: docs
weight: 11
url: /java/com.groupdocs.search.common/arraywriter/
---
**Inheritance:**
java.lang.Object
```
public class ArrayWriter
```

Represents a byte array data writer.
## Constructors

| Constructor | Description |
| --- | --- |
| [ArrayWriter(byte[] array)](#ArrayWriter-byte---) | Initializes a new instance of the  ArrayWriter  class. |
## Methods

| Method | Description |
| --- | --- |
| [getArray()](#getArray--) | Gets the byte array. |
| [getIndex()](#getIndex--) | Gets the current writing position. |
| [checkIndex()](#checkIndex--) | Throws an exception if writing index is not equal to the length of the array. |
| [write(byte value)](#write-byte-) | Writes a byte value to the array. |
| [write(boolean value)](#write-boolean-) | Writes a boolean value to the array. |
| [write(char value)](#write-char-) | Writes a char value to the array. |
| [write(int value)](#write-int-) | Writes an int value to the array. |
| [write(long value)](#write-long-) | Writes a long value to the array. |
| [write(double value)](#write-double-) | Writes a double value to the array. |
| [write(String value)](#write-java.lang.String-) | Writes a String value to the array. |
### ArrayWriter(byte[] array) {#ArrayWriter-byte---}
```
public ArrayWriter(byte[] array)
```


Initializes a new instance of the  ArrayWriter  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | byte[] | The byte array to write to. |

### getArray() {#getArray--}
```
public final byte[] getArray()
```


Gets the byte array.

**Returns:**
byte[] - The byte array.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Gets the current writing position.

**Returns:**
int - The current writing position.
### checkIndex() {#checkIndex--}
```
public final void checkIndex()
```


Throws an exception if writing index is not equal to the length of the array.

### write(byte value) {#write-byte-}
```
public final void write(byte value)
```


Writes a byte value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | The value to write to the array. |

### write(boolean value) {#write-boolean-}
```
public final void write(boolean value)
```


Writes a boolean value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to write to the array. |

### write(char value) {#write-char-}
```
public final void write(char value)
```


Writes a char value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | char | The value to write to the array. |

### write(int value) {#write-int-}
```
public final void write(int value)
```


Writes an int value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The value to write to the array. |

### write(long value) {#write-long-}
```
public final void write(long value)
```


Writes a long value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | long | The value to write to the array. |

### write(double value) {#write-double-}
```
public final void write(double value)
```


Writes a double value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | The value to write to the array. |

### write(String value) {#write-java.lang.String-}
```
public final void write(String value)
```


Writes a String value to the array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The value to write to the array. |

