---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示一个将输出收集到 java.io.OutputStream 的输出适配器。"
type: docs
weight: 31
url: /zh/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

表示将输出收集到 java.io.OutputStream 中的输出适配器。


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // 创建输出流
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // 创建流输出适配器
index.getDocumentText(documents[0], adapter); // 将文档文本生成到流中
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | 初始化 StreamOutputAdapter 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getStream()](#getStream--) | 获取输出流。 |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


初始化 StreamOutputAdapter 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 输出格式。 |
|
|  | 流 | java.io.OutputStream | 输出流。 |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


获取输出流。


**Returns:**
java.io.OutputStream - 输出流。

