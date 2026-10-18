---
title: "구성"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크 구성을 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

검색 네트워크 구성을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | 이 구성을 파일에 저장합니다. |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | 이 구성을 스트림에 저장합니다. |
|
|  | [load(String filePath)](#load-java.lang.String-) | 파일에서 검색 네트워크 구성을 로드합니다. |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | 스트림에서 검색 네트워크 구성을 로드합니다. |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


이 구성을 파일에 저장합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 저장할 파일. |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


이 구성을 스트림에 저장합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | stream | java.io.OutputStream | 저장할 스트림. |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


파일에서 검색 네트워크 구성을 로드합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 로드할 파일. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


스트림에서 검색 네트워크 구성을 로드합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 로드할 스트림. |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

