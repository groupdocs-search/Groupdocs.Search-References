---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "パスワードで保護されたドキュメントがインデックス作成される際に発生するイベントの引数を表します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

パスワードで保護されたドキュメントがインデックス作成される際に発生するイベントの引数を表します。


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | ドキュメントのフルパスを取得します。 |
|
|  | [getPassword()](#getPassword--) | ドキュメントを開くためのパスワードを取得します。 |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | ドキュメントを開くためのパスワードを設定します。 |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


ドキュメントのフルパスを取得します。


**Returns:**
java.lang.String - ドキュメントのフルパス。

### getPassword() {#getPassword--}
```
public final String getPassword()
```


ドキュメントを開くためのパスワードを取得します。


**Returns:**
java.lang.String - ドキュメントを開くためのパスワード。

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


ドキュメントを開くためのパスワードを設定します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | 値 | java.lang.String | ドキュメントを開くためのパスワード。 |
|

