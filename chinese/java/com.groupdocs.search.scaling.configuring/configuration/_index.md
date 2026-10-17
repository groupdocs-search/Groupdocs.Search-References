---
title: "Configuration"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示搜索网络配置。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.scaling.configuring/configuration/
---
**Inheritance:**
java.lang.Object
```
public abstract class Configuration
```

表示搜索网络配置。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Configuration()](#Configuration--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [save(String filePath)](#save-java.lang.String-) | 将此配置保存到文件。 |
|
|  | [save(OutputStream stream)](#save-java.io.OutputStream-) | 将此配置保存到流中。 |
|
|  | [load(String filePath)](#load-java.lang.String-) | 从文件加载搜索网络配置。 |
|
|  | [load(InputStream stream)](#load-java.io.InputStream-) | 从流中加载搜索网络配置。 |
|
### Configuration() {#Configuration--}
```
public Configuration()
```


### save(String filePath) {#save-java.lang.String-}
```
public abstract void save(String filePath)
```


将此配置保存到文件。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 要保存的文件。 |
|

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public abstract void save(OutputStream stream)
```


将此配置保存到流中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 流 | java.io.OutputStream | 要保存的流。 |
|

### load(String filePath) {#load-java.lang.String-}
```
public static Configuration load(String filePath)
```


从文件加载搜索网络配置。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 要加载的文件。 |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### load(InputStream stream) {#load-java.io.InputStream-}
```
public static Configuration load(InputStream stream)
```


从流中加载搜索网络配置。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 流 | java.io.InputStream | 要加载的流。 |
|

**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

