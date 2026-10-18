---
title: "IndexUpdater"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет обновитель индекса."
type: docs
weight: 20
url: /ru/java/com.groupdocs.search/indexupdater/
---
**Inheritance:**
java.lang.Object
```
public class IndexUpdater
```

Представляет обновитель индекса. Этот класс выполняет переиндексацию документов в индексе старой версии.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)


Пример демонстрирует типичное использование класса.

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


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [IndexUpdater()](#IndexUpdater--) | Инициализирует новый экземпляр класса  IndexUpdater  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isLatestVersion(String indexPath)](#isLatestVersion-java.lang.String-) | Проверяет, содержит ли указанный каталог индекс последней версии. |
|
|  | [canUpdateVersion(String indexPath)](#canUpdateVersion-java.lang.String-) | Проверяет, может ли индекс в указанном каталоге быть обновлён до последней версии. |
|
|  | [updateVersion(String indexPath, String newIndexPath)](#updateVersion-java.lang.String-java.lang.String-) | Выполняет переиндексацию документов в индексе старой версии. |
|
### IndexUpdater() {#IndexUpdater--}
```
public IndexUpdater()
```


Инициализирует новый экземпляр класса  IndexUpdater  .


### isLatestVersion(String indexPath) {#isLatestVersion-java.lang.String-}
```
public final boolean isLatestVersion(String indexPath)
```


Проверяет, содержит ли указанный каталог индекс последней версии.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexPath | java.lang.String | Путь к каталогу индекса. |
|

**Returns:**
boolean -  true  если указанный каталог содержит индекс последней версии; иначе  false .

### canUpdateVersion(String indexPath) {#canUpdateVersion-java.lang.String-}
```
public final boolean canUpdateVersion(String indexPath)
```


Проверяет, может ли индекс в указанном каталоге быть обновлён до последней версии.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexPath | java.lang.String | Путь к каталогу индекса. |
|

**Returns:**
boolean -  true  если индекс в указанном каталоге может быть обновлён до последней версии; иначе  false .

### updateVersion(String indexPath, String newIndexPath) {#updateVersion-java.lang.String-java.lang.String-}
```
public final VersionUpdateResult updateVersion(String indexPath, String newIndexPath)
```


Выполняет переиндексацию документов в индексе старой версии. Обновлённый индекс будет размещён в каталоге  newIndexPath . Индекс в каталоге  indexPath  изменён не будет.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexPath | java.lang.String | Путь к каталогу индекса. |
|
|  | newIndexPath | java.lang.String | Каталог для обновлённого индекса. |
|

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult) - The result of the index version update operation.

