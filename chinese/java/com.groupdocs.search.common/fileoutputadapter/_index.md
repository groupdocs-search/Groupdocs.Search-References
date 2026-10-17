---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示将输出收集到文件中的输出适配器。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

表示将输出收集到文件中的输出适配器。


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
DocumentInfo[] documents = index.getIndexedDocuments(); // 获取已索引文档的信息
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // 创建文件输出适配器
index.getDocumentText(documents[0], adapter); // 将文档文本生成到输出文件
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | 初始化 FileOutputAdapter 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | 获取输出文件路径。 |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


初始化 FileOutputAdapter 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 输出格式。 |
|
|  | 文件路径 | java.lang.String | 输出文件路径。 |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


获取输出文件路径。


**Returns:**
java.lang.String - 输出文件路径。

