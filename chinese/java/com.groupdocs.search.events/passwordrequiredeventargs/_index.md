---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示对受密码保护的文档进行索引时发生的事件的参数。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

表示对受密码保护的文档进行索引时发生的事件的参数。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | 获取文档的完整路径。 |
|
|  | [getPassword()](#getPassword--) | 获取打开文档的密码。 |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | 设置打开文档的密码。 |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


获取文档的完整路径。


**Returns:**
java.lang.String - 文档的完整路径。

### getPassword() {#getPassword--}
```
public final String getPassword()
```


获取打开文档的密码。


**Returns:**
java.lang.String - 打开文档的密码。

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


设置打开文档的密码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 值 | java.lang.String | 打开文档的密码。 |
|

