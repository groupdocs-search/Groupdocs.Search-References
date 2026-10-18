---
title: "알림"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에 대한 모든 알림의 기본 클래스입니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.search/notification/
---
**Inheritance:**
java.lang.Object
```
public abstract class Notification
```

인덱스에 대한 모든 알림의 기본 클래스입니다. 이 클래스는 알림 객체를 생성하는 메서드도 포함합니다.


**Learn more**

* [Document renaming](../https://docs.groupdocs.com/display/searchjava/Document+renaming)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Notification()](#Notification--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [createRenameNotification(String oldPath, String newPath)](#createRenameNotification-java.lang.String-java.lang.String-) | 인덱싱된 문서가 이름이 변경되었고 재인덱싱이 필요하지 않을 때, 해당 문서를 이름 변경하기 위한 알림 객체를 생성합니다. |
|
### Notification() {#Notification--}
```
public Notification()
```


### createRenameNotification(String oldPath, String newPath) {#createRenameNotification-java.lang.String-java.lang.String-}
```
public static Notification createRenameNotification(String oldPath, String newPath)
```


인덱싱된 문서가 이름이 변경되었고 재인덱싱이 필요하지 않을 때, 해당 문서를 이름 변경하기 위한 알림 객체를 생성합니다. 이름이 변경된 문서는 내용이 변경되었더라도 다음 업데이트 작업 중에 재인덱싱되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | oldPath | java.lang.String | 인덱싱된 문서의 이전 경로입니다. |
|
|  | newPath | java.lang.String | 인덱싱된 문서의 새로운 경로입니다. |
|

**Returns:**
[Notification](../../com.groupdocs.search/notification) - A new rename notification object.

