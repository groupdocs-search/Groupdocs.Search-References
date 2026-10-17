---
title: "NodeConfigurator"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مكوّن عقدة شبكة البحث."
type: docs
weight: 13
url: /ar/java/com.groupdocs.search.scaling.configuring/nodeconfigurator/
---
**Inheritance:**
java.lang.Object
```
public abstract class NodeConfigurator
```

يمثل مكوّن عقدة شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
| [NodeConfigurator()](#NodeConfigurator--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [setTcpEndpoint(String hostNameOrAddress, int port)](#setTcpEndpoint-java.lang.String-int-) | يضبط نقطة النهاية TCP. |
|
|  | [addLogSink()](#addLogSink--) | يضيف مستقبل سجل إلى عقدة شبكة البحث. |
|
|  | [addSearcher(String storagePath)](#addSearcher-java.lang.String-) | يضيف خدمة الباحث إلى عقدة شبكة البحث. |
|
|  | [addIndexer(String storagePath)](#addIndexer-java.lang.String-) | يضيف خدمة الفهرس إلى عقدة شبكة البحث. |
|
|  | [addExtractor(String storagePath)](#addExtractor-java.lang.String-) | يضيف خدمة المستخرج إلى عقدة شبكة البحث. |
|
|  | [addShard(String storagePath)](#addShard-java.lang.String-) | يضيف خدمة الشظية إلى عقدة شبكة البحث. |
|
|  | [completeNode()](#completeNode--) | يكمل تكوين عقدة شبكة البحث. |
|
### NodeConfigurator() {#NodeConfigurator--}
```
public NodeConfigurator()
```


### setTcpEndpoint(String hostNameOrAddress, int port) {#setTcpEndpoint-java.lang.String-int-}
```
public abstract NodeConfigurator setTcpEndpoint(String hostNameOrAddress, int port)
```


يضبط نقطة النهاية TCP.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | hostNameOrAddress | java.lang.String | اسم المضيف أو العنوان. |
|
|  | المنفذ | int | رقم المنفذ. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addLogSink() {#addLogSink--}
```
public abstract NodeConfigurator addLogSink()
```


يضيف مستقبل سجل إلى عقدة شبكة البحث.


**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addSearcher(String storagePath) {#addSearcher-java.lang.String-}
```
public abstract NodeConfigurator addSearcher(String storagePath)
```


يضيف خدمة الباحث إلى عقدة شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | storagePath | java.lang.String | مسار التخزين لخدمة الإضافة. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addIndexer(String storagePath) {#addIndexer-java.lang.String-}
```
public abstract NodeConfigurator addIndexer(String storagePath)
```


يضيف خدمة الفهرس إلى عقدة شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | storagePath | java.lang.String | مسار التخزين لخدمة الإضافة. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addExtractor(String storagePath) {#addExtractor-java.lang.String-}
```
public abstract NodeConfigurator addExtractor(String storagePath)
```


يضيف خدمة المستخرج إلى عقدة شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | storagePath | java.lang.String | مسار التخزين لخدمة الإضافة. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### addShard(String storagePath) {#addShard-java.lang.String-}
```
public abstract NodeConfigurator addShard(String storagePath)
```


يضيف خدمة الشظية إلى عقدة شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | storagePath | java.lang.String | مسار التخزين لخدمة الإضافة. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - This search network node configurator.

### completeNode() {#completeNode--}
```
public abstract Configurator completeNode()
```


يكمل تكوين عقدة شبكة البحث.


**Returns:**
[Configurator](../../com.groupdocs.search.scaling.configuring/configurator) - The configurator.

