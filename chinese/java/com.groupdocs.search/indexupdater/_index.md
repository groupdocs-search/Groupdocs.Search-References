---
title: "IndexUpdater"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示索引更新器。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

表示索引更新器。此类在旧版本的索引中执行文档重新索引。


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


此示例演示了该类的典型用法。

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


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | 初始化  IndexUpdater  类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | 检查指定目录是否包含最新版本的索引。 |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | 检查指定目录中的索引是否可以更新到最新版本。 |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | 在旧版本的索引中执行文档重新索引。 |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


初始化  IndexUpdater  类的新实例。


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


检查指定目录是否包含最新版本的索引。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexPath | java.lang.String | 索引目录路径。 |
|

**Returns:**
boolean -  true  如果指定目录包含最新版本的索引；否则为  false 。

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


检查指定目录中的索引是否可以更新到最新版本。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexPath | java.lang.String | 索引目录路径。 |
|

**Returns:**
boolean -  true  如果指定目录中的索引可以更新到最新版本；否则为  false 。

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


在旧版本的索引中执行文档重新索引。更新后的索引将放置在  newIndexPath  目录中。位于  indexPath  目录中的索引将保持不变。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | indexPath | java.lang.String | 索引目录路径。 |
|
|  | newIndexPath | java.lang.String | 更新后索引的目录。 |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

