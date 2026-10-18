---
title: "DateFormat"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "날짜 형식을 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

날짜 형식을 나타냅니다.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스를 생성합니다.
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // 기본 날짜 형식 제거
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// 날짜 형식 패턴 'MM/dd/yyyy' 생성
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // 인덱스에서 검색
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | DateFormat 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | DateFormat 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | 날짜 구분자를 가져옵니다. |
|
|  | [toString()](#toString--) | 현재 DateFormat을 나타내는 문자열을 반환합니다. |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


DateFormat 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | cultureName | java.lang.String | 문화 이름입니다. |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | 형식 요소입니다. |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


DateFormat 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | 형식 요소입니다. |
|
|  | dateSeparator | java.lang.String | 날짜 구분자입니다. |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


날짜 구분자를 가져옵니다.


**Returns:**
java.lang.String - 날짜 구분자입니다.

### toString() {#toString--}
```
public String toString()
```


현재 DateFormat을 나타내는 문자열을 반환합니다.


**Returns:**
java.lang.String - 현재 DateFormat을 나타내는 문자열입니다.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
