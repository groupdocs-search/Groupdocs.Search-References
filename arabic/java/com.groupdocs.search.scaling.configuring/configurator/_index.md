---
title: "Configurator"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مكوّن شبكة البحث."
type: docs
weight: 11
url: /ar/java/com.groupdocs.search.scaling.configuring/configurator/
---
**Inheritance:**
java.lang.Object
```
public class Configurator
```

يمثل مكوّن شبكة البحث.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Configurator()](#Configurator--) | يُنشئ مثيلًا جديدًا من الفئة Configurator. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [setIndexSettings()](#setIndexSettings--) | يبدأ تكوين إعدادات الفهرس لكل شظية في شبكة البحث. |
|
|  | [addNode(int nodeIndex)](#addNode-int-) | يضيف عقدة إلى تكوين شبكة البحث. |
|
|  | [completeConfiguration()](#completeConfiguration--) | يكمل عملية التكوين ويعيد مثيلًا من تكوين شبكة البحث. |
|
| [getCore()](#getCore--) |  |
### Configurator() {#Configurator--}
```
public Configurator()
```


يُنشئ مثيلًا جديدًا من الفئة Configurator.


### setIndexSettings() {#setIndexSettings--}
```
public IndexSettingsConfigurator setIndexSettings()
```


يبدأ تكوين إعدادات الفهرس لكل شظية في شبكة البحث.


**Returns:**
[IndexSettingsConfigurator](../../com.groupdocs.search.scaling.configuring/indexsettingsconfigurator) - The index settings configurator.

### addNode(int nodeIndex) {#addNode-int-}
```
public NodeConfigurator addNode(int nodeIndex)
```


يضيف عقدة إلى تكوين شبكة البحث.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | nodeIndex | int | فهرس العقدة. |
|

**Returns:**
[NodeConfigurator](../../com.groupdocs.search.scaling.configuring/nodeconfigurator) - The node configurator.

### completeConfiguration() {#completeConfiguration--}
```
public Configuration completeConfiguration()
```


يكمل عملية التكوين ويعيد مثيلًا من تكوين شبكة البحث.


**Returns:**
[Configuration](../../com.groupdocs.search.scaling.configuring/configuration) - The configuration.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
