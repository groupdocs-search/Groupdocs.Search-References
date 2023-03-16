---
title: SearchQuery
second_title: GroupDocs.Search для справочника API .NET
description: Представляет поисковый запрос в форме объекта.
type: docs
weight: 1240
url: /ru/net/groupdocs.search/searchquery/
---
## SearchQuery class

Представляет поисковый запрос в форме объекта.

```csharp
public abstract class SearchQuery
```

## Характеристики

| Имя | Описание |
| --- | --- |
| virtual [ChildCount](../../groupdocs.search/searchquery/childcount) { get; } | Получает количество дочерних запросов. |
| virtual [FieldName](../../groupdocs.search/searchquery/fieldname) { get; } | Получает имя поля. |
| virtual [FirstChild](../../groupdocs.search/searchquery/firstchild) { get; } | Получает первый дочерний запрос. |
| [SearchOptions](../../groupdocs.search/searchquery/searchoptions) { get; set; } | Получает или задает параметры поиска для этого поискового запроса. |
| virtual [SecondChild](../../groupdocs.search/searchquery/secondchild) { get; } | Получает второй дочерний запрос. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateAndQuery](../../groupdocs.search/searchquery/createandquery)(SearchQuery, SearchQuery) | Создает комбинированный запрос, который найдет только те документы, которые будут найдены для каждого исходного запроса. |
| static [CreateDateRangeQuery](../../groupdocs.search/searchquery/createdaterangequery)(DateTime, DateTime) | Создает запрос диапазона дат. |
| static [CreateFieldQuery](../../groupdocs.search/searchquery/createfieldquery)(string, SearchQuery) | Добавляет поле к указанному запросу. |
| static [CreateNotQuery](../../groupdocs.search/searchquery/createnotquery)(SearchQuery) | Создает инвертированный запрос, который находит остальные документы в индексе по сравнению с теми, которые будут найдены для исходного запроса. |
| static [CreateNumericRangeQuery](../../groupdocs.search/searchquery/createnumericrangequery)(long, long) | Создает запрос числового диапазона. |
| static [CreateOrQuery](../../groupdocs.search/searchquery/createorquery)(SearchQuery, SearchQuery) | Создает комбинированный запрос, который найдет все документы, которые будут найдены хотя бы для одного из исходных запросов. |
| static [CreatePhraseSearchQuery](../../groupdocs.search/searchquery/createphrasesearchquery)(params SearchQuery[]) | Создает поисковый запрос по фразе. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery)(string) | Создает запрос регулярного выражения. |
| static [CreateRegexQuery](../../groupdocs.search/searchquery/createregexquery#createregexquery_1)(string, RegexOptions) | Создает запрос регулярного выражения. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery)(int) | Создает подстановочный знак для поиска по фразе. |
| static [CreateWildcardQuery](../../groupdocs.search/searchquery/createwildcardquery#createwildcardquery_1)(int, int) | Создает подстановочный знак для поиска по фразе. |
| static [CreateWordPatternQuery](../../groupdocs.search/searchquery/createwordpatternquery)(WordPattern) | Создает запрос шаблона слова. |
| static [CreateWordQuery](../../groupdocs.search/searchquery/createwordquery)(string) | Создает простой словесный запрос. |
| abstract [GetChild](../../groupdocs.search/searchquery/getchild)(int) | Получает дочерний запрос по индексу. |
| abstract [ToString](../../groupdocs.search/searchquery/tostring)() | ВозвращаетString который представляет текущий[`SearchQuery`](../searchquery) экземпляр. |

### Примечания

**Узнать больше**

* [Идет поиск](https://docs.groupdocs.com/display/searchnet/Searching)
* [Запросы в текстовом и объектном виде](https://docs.groupdocs.com/display/searchnet/Queries+in+text+and+object+form)
* [Вложение поисковых запросов в объектную форму](https://docs.groupdocs.com/display/searchnet/Nesting+search+queries+in+object+form)

### Примеры

Пример демонстрирует типичное использование класса.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

// Создание подзапроса поиска диапазона дат
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Создание подзапроса подстановочного знака с количеством пропущенных слов от 0 до 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Создание подзапроса простого слова
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Установка параметров поиска только для подзапроса 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Создание объекта опций поиска с увеличенной емкостью найденных вхождений
SearchOptions options = new SearchOptions(); // Общие параметры поиска
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Идет поиск
```

### Смотрите также

* пространство имен [GroupDocs.Search](../../groupdocs.search)
* сборка [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
