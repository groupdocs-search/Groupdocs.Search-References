---
title: "FragmentContainer"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "1つのドキュメントフィールドのハイライトされた検索語句を含むテキストフラグメントのコンテナを表します。"
type: docs
weight: 22
url: /ja/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

1つのドキュメントフィールドのハイライトされた検索語句を含むテキストフラグメントのコンテナを表します。


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | ドキュメントフィールド名を取得します。 |
|
|  | [getCount()](#getCount--) | 含まれるテキストフラグメントの数を取得します。 |
|
|  | [getFragments()](#getFragments--) | 含まれるテキストフラグメントの配列を取得します。 |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


ドキュメントフィールド名を取得します。


**Returns:**
java.lang.String - ドキュメントフィールド名。

### getCount() {#getCount--}
```
public abstract int getCount()
```


含まれるテキストフラグメントの数を取得します。


**Returns:**
int - 含まれるテキストフラグメントの数。

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


含まれるテキストフラグメントの配列を取得します。


**Returns:**
java.lang.String[] - 含まれるテキストフラグメントの配列。

