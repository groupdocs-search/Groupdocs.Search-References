---
title: HighlightOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for highlighting found terms.
type: docs
weight: 20
url: /java/com.groupdocs.search.options/highlightoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.TextOptions](../../com.groupdocs.search.options/textoptions)

**All Implemented Interfaces:**
[com.groupdocs.search.options.IHighlightOptions](../../com.groupdocs.search.options/ihighlightoptions)
```
public class HighlightOptions extends TextOptions implements IHighlightOptions
```

Provides options for highlighting found terms.

**Learn more**

 *  [Highlighting search results][]


[Highlighting search results]: https://docs.groupdocs.com/display/searchjava/Highlighting+search+results
## Constructors

| Constructor | Description |
| --- | --- |
| [HighlightOptions()](#HighlightOptions--) | Initializes a new instance of the  HighlightOptions  class. |
| [HighlightOptions(Object data)](#HighlightOptions-java.lang.Object-) | Initializes a new instance of the  TextOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getTermsBefore()](#getTermsBefore--) | Gets the maximum number of words in a text snippet before highlighted word. |
| [setTermsBefore(int value)](#setTermsBefore-int-) | Sets the maximum number of words in a text snippet before highlighted word. |
| [getTermsAfter()](#getTermsAfter--) | Gets the maximum number of words in a text snippet after highlighted word. |
| [setTermsAfter(int value)](#setTermsAfter-int-) | Sets the maximum number of words in a text snippet after highlighted word. |
| [getTermsTotal()](#getTermsTotal--) | Gets the maximum number of words in a text snippet. |
| [setTermsTotal(int value)](#setTermsTotal-int-) | Sets the maximum number of words in a text snippet. |
| [getUseInlineStyles()](#getUseInlineStyles--) | Gets a value indicating whether inline styles are used to highlight occurrences. |
| [setUseInlineStyles(boolean value)](#setUseInlineStyles-boolean-) | Sets a value indicating whether inline styles are used to highlight occurrences. |
| [getHighlightColor()](#getHighlightColor--) | Gets a color that is used to highlight occurrences. |
| [setHighlightColor(Color value)](#setHighlightColor-com.groupdocs.search.options.Color-) | Sets a color that is used to highlight occurrences. |
| [getTermHighlightStartTag()](#getTermHighlightStartTag--) | Gets the start tag of the highlighting of the found word. |
| [setTermHighlightStartTag(String value)](#setTermHighlightStartTag-java.lang.String-) | Sets the start tag of the highlighting of the found word. |
| [getTermHighlightEndTag()](#getTermHighlightEndTag--) | Gets the end tag of the highlighting of the found word. |
| [setTermHighlightEndTag(String value)](#setTermHighlightEndTag-java.lang.String-) | Sets the end tag of the highlighting of the found word. |
### HighlightOptions() {#HighlightOptions--}
```
public HighlightOptions()
```


Initializes a new instance of the  HighlightOptions  class.

### HighlightOptions(Object data) {#HighlightOptions-java.lang.Object-}
```
public HighlightOptions(Object data)
```


Initializes a new instance of the  TextOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | java.lang.Object | The serialized data. |

### getTermsBefore() {#getTermsBefore--}
```
public int getTermsBefore()
```


Gets the maximum number of words in a text snippet before highlighted word. The value must be in the range from 0 to 10000. The default value is  7 .

**Returns:**
int - The maximum number of words in a text snippet before highlighted word.
### setTermsBefore(int value) {#setTermsBefore-int-}
```
public void setTermsBefore(int value)
```


Sets the maximum number of words in a text snippet before highlighted word. The value must be in the range from 0 to 10000. The default value is  7 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of words in a text snippet before highlighted word. |

### getTermsAfter() {#getTermsAfter--}
```
public int getTermsAfter()
```


Gets the maximum number of words in a text snippet after highlighted word. The value must be in the range from 0 to 10000. The default value is  7 .

**Returns:**
int - The maximum number of words in a text snippet after highlighted word.
### setTermsAfter(int value) {#setTermsAfter-int-}
```
public void setTermsAfter(int value)
```


Sets the maximum number of words in a text snippet after highlighted word. The value must be in the range from 0 to 10000. The default value is  7 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of words in a text snippet after highlighted word. |

### getTermsTotal() {#getTermsTotal--}
```
public int getTermsTotal()
```


Gets the maximum number of words in a text snippet. The value must be in the range from 0 to 10000. The default value is  21 .

**Returns:**
int - The maximum number of words in a text snippet.
### setTermsTotal(int value) {#setTermsTotal-int-}
```
public void setTermsTotal(int value)
```


Sets the maximum number of words in a text snippet. The value must be in the range from 0 to 10000. The default value is  21 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of words in a text snippet. |

### getUseInlineStyles() {#getUseInlineStyles--}
```
public boolean getUseInlineStyles()
```


Gets a value indicating whether inline styles are used to highlight occurrences. The default value is  true .

**Returns:**
boolean - A value indicating whether inline styles are used to highlight occurrences.
### setUseInlineStyles(boolean value) {#setUseInlineStyles-boolean-}
```
public void setUseInlineStyles(boolean value)
```


Sets a value indicating whether inline styles are used to highlight occurrences. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether inline styles are used to highlight occurrences. |

### getHighlightColor() {#getHighlightColor--}
```
public Color getHighlightColor()
```


Gets a color that is used to highlight occurrences. The default value is \#FFD800.

**Returns:**
[Color](../../com.groupdocs.search.options/color) - A color that is used to highlight occurrences.
### setHighlightColor(Color value) {#setHighlightColor-com.groupdocs.search.options.Color-}
```
public void setHighlightColor(Color value)
```


Sets a color that is used to highlight occurrences. The default value is \#FFD800.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.groupdocs.search.options/color) | A color that is used to highlight occurrences. |

### getTermHighlightStartTag() {#getTermHighlightStartTag--}
```
public String getTermHighlightStartTag()
```


Gets the start tag of the highlighting of the found word. This tag is used only when highlighting in plain text. The default value is an empty string.

**Returns:**
java.lang.String - The start tag of the highlighting of the found word.
### setTermHighlightStartTag(String value) {#setTermHighlightStartTag-java.lang.String-}
```
public void setTermHighlightStartTag(String value)
```


Sets the start tag of the highlighting of the found word. This tag is used only when highlighting in plain text. The default value is an empty string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The start tag of the highlighting of the found word. |

### getTermHighlightEndTag() {#getTermHighlightEndTag--}
```
public String getTermHighlightEndTag()
```


Gets the end tag of the highlighting of the found word. This tag is used only when highlighting in plain text. The default value is an empty string.

**Returns:**
java.lang.String - The end tag of the highlighting of the found word.
### setTermHighlightEndTag(String value) {#setTermHighlightEndTag-java.lang.String-}
```
public void setTermHighlightEndTag(String value)
```


Sets the end tag of the highlighting of the found word. This tag is used only when highlighting in plain text. The default value is an empty string.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The end tag of the highlighting of the found word. |

