---
title: PasswordRequiredEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event that occurs when document protected by a password is indexing.
type: docs
weight: 20
url: /java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event that occurs when document protected by a password is indexing.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getDocumentFullPath()](#getDocumentFullPath--) | Gets the document full path. |
| [getPassword()](#getPassword--) | Gets the password for opening the document. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Sets the password for opening the document. |
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Gets the document full path.

**Returns:**
java.lang.String - The document full path.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Gets the password for opening the document.

**Returns:**
java.lang.String - The password for opening the document.
### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Sets the password for opening the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The password for opening the document. |

