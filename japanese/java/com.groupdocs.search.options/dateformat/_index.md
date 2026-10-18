---
title: "DateFormat"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "日付形式を表します。"
type: docs
weight: 13
url: /ja/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

日付形式を表します。


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


この例はクラスの典型的な使用方法を示しています。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // 指定されたフォルダーにインデックスを作成しています
index.add(documentsFolder); // 指定されたフォルダーからドキュメントをインデックス化しています
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // デフォルトの日付形式を削除
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// 'MM/dd/yyyy' の日付フォーマットパターンを作成
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // インデックス内を検索
 
```
 
````


## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | DateFormat クラスの新しいインスタンスを初期化します。 |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | DateFormat クラスの新しいインスタンスを初期化します。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | 日付区切り文字を取得します。 |
|
|  | [toString()](#toString--) | 現在の DateFormat を表す String を返します。 |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


DateFormat クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | cultureName | java.lang.String | カルチャー名。 |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | フォーマット要素。 |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


DateFormat クラスの新しいインスタンスを初期化します。


**Parameters:**
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | フォーマット要素。 |
|
|  | dateSeparator | java.lang.String | 日付区切り文字です。 |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


日付区切り文字を取得します。


**Returns:**
java.lang.String - 日付区切り文字です。

### toString() {#toString--}
```
public String toString()
```


現在の DateFormat を表す String を返します。


**Returns:**
java.lang.String - 現在の DateFormat を表す String です。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
