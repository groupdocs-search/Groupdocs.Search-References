---
title: "FileLogger"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이벤트와 오류를 로컬 파일에 기록하는 로거를 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

이벤트와 오류를 로컬 파일에 기록하는 로거를 나타냅니다.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // 로그 파일 경로와 최대 4 MB 길이를 지정합니다
Index index = new Index(indexFolder, settings); // 지정된 폴더에 인덱스를 생성합니다
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchResult result = index.search(query); // 인덱스 검색
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | FileLogger 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | 인덱스에서 발생한 오류를 기록합니다. |
|
|  | [trace(String message)](#trace-java.lang.String-) | 인덱스에서 발생한 이벤트를 기록합니다. |
|
|  | [getFilePath()](#getFilePath--) | 로그 파일 경로를 가져옵니다. |
|
|  | [getMaxSize()](#getMaxSize--) | 로그 파일의 최대 크기를 메가바이트 단위로 가져옵니다. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


FileLogger 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 로그 파일 경로. |
|
|  | maxSize | double | 로그 파일의 최대 크기(메가바이트). 값은 0.1에서 1000 사이여야 합니다. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


인덱스에서 발생한 오류를 기록합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 메시지 | java.lang.String | 오류 메시지. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


인덱스에서 발생한 이벤트를 기록합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 메시지 | java.lang.String | 이벤트 메시지. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


로그 파일 경로를 가져옵니다.


**Returns:**
java.lang.String - 로그 파일 경로.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


로그 파일의 최대 크기를 메가바이트 단위로 가져옵니다.


**Returns:**
double - 로그 파일의 최대 크기(메가바이트).

