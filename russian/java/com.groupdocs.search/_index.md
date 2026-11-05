---
title: "com.groupdocs.search"
second_title: "GroupDocs.Search для Java API Reference"
description: "Пакет предоставляет классы для индексации и поиска текстовых данных в документах разных форматов."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search/
---

Пакет предоставляет классы для индексации и поиска текстовых данных в документах разных форматов. Основные классы в этом пакете:

Index является точкой входа для операций индексации и поиска.

SearchQuery является базовым классом и фабрикой для всех типов поисковых запросов в объектной форме.

IndexRepository является контейнерным классом для объединения нескольких индексов и выполнения общих операций над ними.



## Классы

| Класс | Описание |
| --- | --- |
| [Action](../com.groupdocs.search/action) | Инкапсулирует метод, который не имеет параметров и не возвращает значение. |
| [Action1<T>](../com.groupdocs.search/action1) | Инкапсулирует метод, который имеет один параметр и не возвращает значение. |
| [Action2<T1,T2>](../com.groupdocs.search/action2) | Инкапсулирует метод, который имеет два параметра и не возвращает значение. |
| [Document](../com.groupdocs.search/document) | Представляет базовый класс для документов, добавляемых в индекс из файловой системы, потока или структуры. |
| [DocumentFilter](../com.groupdocs.search/documentfilter) | Представляет базовый класс для фильтров документов. |
| [ExtractedData](../com.groupdocs.search/extracteddata) | Представляет данные, полученные из документа и подготовленные для индексации. |
| [Extractor](../com.groupdocs.search/extractor) | Представляет инструмент для предварительного извлечения данных из документов, позволяющий отделить этап последующей быстрой индексации. |
| [Index](../com.groupdocs.search/index) | Представляет основной класс для индексации документов и поиска по ним. |
| [IndexRepository](../com.groupdocs.search/indexrepository) | Представляет контейнер для объединения нескольких индексов и выполнения общих операций над ними. |
| [IndexSettings](../com.groupdocs.search/indexsettings) | Представляет настройки индекса, позволяющие настраивать операции индексации. |
| [IndexUpdater](../com.groupdocs.search/indexupdater) | Представляет обновитель индекса. |
| [LicenseRestrictionException](../com.groupdocs.search/licenserestrictionexception) | Исключение, которое выбрасывается, когда срабатывает ограничение лицензии. |
| [Notification](../com.groupdocs.search/notification) | Базовый класс для всех уведомлений индекса. |
| [PleaseReportException](../com.groupdocs.search/pleasereportexception) | Представляет исключение, которое выбрасывается, когда в библиотеке произошла ошибка. |
| [SearchDocumentFilter](../com.groupdocs.search/searchdocumentfilter) | Содержит методы для создания фильтров поисковых документов. |
| [SearchQuery](../com.groupdocs.search/searchquery) | Представляет поисковый запрос в виде объекта. |
