---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "비밀번호로 보호된 문서가 인덱싱될 때 발생하는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.search.events/passwordrequiredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class PasswordRequiredEventArgs extends BaseIndexEventArgs
```

비밀번호로 보호된 문서가 인덱싱될 때 발생하는 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentFullPath()](#getDocumentFullPath--) | 문서의 전체 경로를 가져옵니다. |
|
|  | [getPassword()](#getPassword--) | 문서를 열기 위한 비밀번호를 가져옵니다. |
|
|  | [setPassword(String value)](#setPassword-java.lang.String-) | 문서를 열기 위한 비밀번호를 설정합니다. |
|
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


문서의 전체 경로를 가져옵니다.


**Returns:**
java.lang.String - 문서의 전체 경로.

### getPassword() {#getPassword--}
```
public final String getPassword()
```


문서를 열기 위한 비밀번호를 가져옵니다.


**Returns:**
java.lang.String - 문서를 열기 위한 비밀번호.

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


문서를 열기 위한 비밀번호를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 문서를 열기 위한 비밀번호. |
|

