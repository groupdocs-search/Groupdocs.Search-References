---
title: "PasswordDictionary"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "文書パスワード辞書のインターフェイスを定義します。"
type: docs
weight: 20
url: /ja/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

文書パスワード辞書のインターフェイスを定義します。


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getCount()](#getCount--) | 辞書に含まれる要素数を取得します。 |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | ファイルのパスワードを取得します。 |
|
|  | [clear()](#clear--) | この PasswordDictionary オブジェクトからすべてのパスワードを削除します。 |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | 指定されたドキュメントのパスワードが辞書に含まれているかどうかを判断します。 |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | ドキュメントのパスワードを辞書に追加します。 |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | 指定されたドキュメントのパスワードを辞書から削除します。 |
|
|  | [iterator()](#iterator--) | コレクションを反復するイテレータを返します。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


辞書に含まれる要素数を取得します。


**Returns:**
int - 辞書に含まれる要素数。

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


ファイルのパスワードを取得します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ファイルパス。 |
|

**Returns:**
java.lang.String - ファイルのパスワード。

### clear() {#clear--}
```
public abstract void clear()
```


この PasswordDictionary オブジェクトからすべてのパスワードを削除します。


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


指定されたドキュメントのパスワードが辞書に含まれているかどうかを判断します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ドキュメントのファイルパスです。 |
|

**Returns:**
boolean - 辞書にドキュメントのパスワードが含まれている場合は true、そうでない場合は false。

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


ドキュメントのパスワードを辞書に追加します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ドキュメントのファイルパスです。 |
|
|  | password | java.lang.String | ドキュメントのパスワード。 |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


指定されたドキュメントのパスワードを辞書から削除します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | filePath | java.lang.String | ドキュメントのファイルパスです。 |
|

**Returns:**
boolean - パスワードが正常に削除された場合は true、そうでない場合は false。このメソッドは、辞書に filePath が見つからなかった場合も false を返します。

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


コレクションを反復するイテレータを返します。


**Returns:**
java.util.Iterator<java.lang.String> - コレクションを反復するために使用できるイテレータ。

