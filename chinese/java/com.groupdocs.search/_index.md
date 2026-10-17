---
title: "com.groupdocs.search"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "该包提供用于对不同格式文档中的文本数据进行索引和搜索的类。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search/
---

该包提供用于对不同格式文档中的文本数据进行索引和搜索的类。此包中的主要类有：

Index 是索引和搜索操作的入口点。

SearchQuery 是基类，也是所有类型搜索查询对象形式的工厂。

IndexRepository 是用于合并多个索引并对其执行通用操作的容器类。



## 类

| 类 | 描述 |
| --- | --- |
| [Action](../com.groupdocs.search/action) | 封装了一个没有参数且不返回值的方法。 |
| [Action1<T>](../com.groupdocs.search/action1) | 封装一个具有单个参数且不返回值的方法。 |
| [Action2<T1,T2>](../com.groupdocs.search/action2) | 封装一个具有两个参数且不返回值的方法。 |
| [Document](../com.groupdocs.search/document) | 表示从文件系统、流或结构添加到索引的文档的基类。 |
| [DocumentFilter](../com.groupdocs.search/documentfilter) | 表示文档过滤器的基类。 |
| [ExtractedData](../com.groupdocs.search/extracteddata) | 表示从文档检索并准备进行索引的数据。 |
| [Extractor](../com.groupdocs.search/extractor) | 表示用于从文档进行初步数据提取以分离后续快速索引阶段的工具。 |
| [Index](../com.groupdocs.search/index) | 表示用于索引文档并在其中搜索的主类。 |
| [IndexRepository](../com.groupdocs.search/indexrepository) | 表示用于组合多个索引并对其执行通用操作的容器。 |
| [IndexSettings](../com.groupdocs.search/indexsettings) | 表示允许自定义索引操作的索引设置。 |
| [IndexUpdater](../com.groupdocs.search/indexupdater) | 表示索引更新器。 |
| [LicenseRestrictionException](../com.groupdocs.search/licenserestrictionexception) | 当触发许可证限制时抛出的异常。 |
| [Notification](../com.groupdocs.search/notification) | 索引所有通知的基类。 |
| [PleaseReportException](../com.groupdocs.search/pleasereportexception) | 表示库中发生错误时抛出的异常。 |
| [SearchDocumentFilter](../com.groupdocs.search/searchdocumentfilter) | 包含用于创建搜索文档过滤器的方法。 |
| [SearchQuery](../com.groupdocs.search/searchquery) | 表示对象形式的搜索查询。 |
