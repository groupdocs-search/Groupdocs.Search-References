---
title: "Notification"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "インデックスへのすべての通知の基底クラスです。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

インデックスへのすべての通知の基底クラスです。このクラスには通知オブジェクトを作成するメソッドも含まれています。


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Notification()](#Notification--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | 名前が変更されたインデックス化されたドキュメントを再インデックスせずに名前変更するための通知オブジェクトを作成します。 |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


名前が変更されたインデックス化されたドキュメントを再インデックスせずに名前変更するための通知オブジェクトを作成します。名前変更されたドキュメントは、内容が変更されていても次回の更新操作中に再インデックスされません。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | oldPath | java.lang.String | インデックス化されたドキュメントの古いパスです。 |
|
|  | newPath | java.lang.String | インデックスされたドキュメントへの新しいパスです。 |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

