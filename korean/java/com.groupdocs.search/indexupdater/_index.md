---
title: "IndexUpdater"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스 업데이트 프로그램을 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

인덱스 업데이트자를 나타냅니다. 이 클래스는 이전 버전의 인덱스에서 문서를 재인덱싱합니다.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String sourceIndexFolder = "c:\\MyOldIndex\\";
String targetIndexFolder = "c:\\MyNewIndex\\";
IndexUpdater updater = new IndexUpdater();
if (updater.canUpdateVersion(sourceIndexFolder)) {
int result = updater.updateVersion(sourceIndexFolder, targetIndexFolder);
}
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | 새로운 IndexUpdater 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | 지정된 디렉터리에 최신 버전의 인덱스가 포함되어 있는지 확인합니다. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | 지정된 디렉터리의 인덱스를 최신 버전으로 업데이트할 수 있는지 확인합니다. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | 이전 버전의 인덱스에서 문서를 재인덱싱합니다. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


새로운 IndexUpdater 클래스 인스턴스를 초기화합니다.


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


지정된 디렉터리에 최신 버전의 인덱스가 포함되어 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexPath | java.lang.String | 인덱스 디렉터리 경로. |
|

**Returns:**
boolean - 지정된 디렉터리에 최신 버전의 인덱스가 포함된 경우 true; 그렇지 않으면 false.

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


지정된 디렉터리의 인덱스를 최신 버전으로 업데이트할 수 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexPath | java.lang.String | 인덱스 디렉터리 경로. |
|

**Returns:**
boolean - 지정된 디렉터리의 인덱스를 최신 버전으로 업데이트할 수 있는 경우 true; 그렇지 않으면 false.

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


이전 버전의 인덱스에서 문서를 재인덱싱합니다. 업데이트된 인덱스는 newIndexPath 디렉터리에 배치됩니다. indexPath 디렉터리의 인덱스는 변경되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexPath | java.lang.String | 인덱스 디렉터리 경로. |
|
|  | newIndexPath | java.lang.String | 업데이트된 인덱스의 디렉터리. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

