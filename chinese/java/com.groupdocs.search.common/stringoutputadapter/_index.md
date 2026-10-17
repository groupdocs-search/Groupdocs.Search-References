---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示一个将输出收集为 System.String 的输出适配器。"
type: docs
weight: 32
url: /zh/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

表示将输出收集为 System.String 的输出适配器。


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
StringOutputAdapter adapter = new StringOutputAdapter(); // 创建一个字符串输出适配器
index.getDocumentText(documents[0], adapter); // 将文档文本生成到适配器中
String result = adapter.getResult(); // 获取结果
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | 初始化 StringOutputAdapter 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getResult()](#getResult--) | 获取结果字符串。 |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


初始化 StringOutputAdapter 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 输出格式。 |
|

### getResult() {#getResult--}
```
public final String getResult()
```


获取结果字符串。


**Returns:**
java.lang.String - 结果字符串。

