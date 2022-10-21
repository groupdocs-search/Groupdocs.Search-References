---
title: IndexErrorEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of index error occurred.
type: docs
weight: 17
url: /java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event of index error occurred.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getMessage()](#getMessage--) | Gets the error message. |
| [isCritical()](#isCritical--) | Gets a flag indicating that the error occurred is critical and the index should be restarted. |
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Gets the error message.

**Returns:**
java.lang.String - The error message.
### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


Gets a flag indicating that the error occurred is critical and the index should be restarted.

**Returns:**
boolean - The flag indicating that the error occurred is critical and the index should be restarted.
