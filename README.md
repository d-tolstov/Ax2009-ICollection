# Аналог интерфейса [ICollection\<T\>](https://docs.microsoft.com/ru-ru/dotnet/api/system.collections.generic.icollection-1?view=netframework-4.8) в Ax2009

Стало не хватать в аксапте интерфейса, в который можно было бы обернуть такие объекты как `Set`, `List`, а также объекты CLR типа [`List<T>`](https://docs.microsoft.com/ru-ru/dotnet/api/system.collections.generic.list-1?view=netframework-4.8), [`SortedSet<T>`](https://docs.microsoft.com/ru-ru/dotnet/api/system.collections.generic.sortedset-1?view=netframework-4.8).

Реализовать методы :
* `Add(anytype item)`
* `Count`
* `Contains(anytype item)`

Отнаследовать от :
* `Enumerable`

## Диаграмма классов
<img src="out\schema\ICollection.png" alt="схема">

### Зависимости от других репозиториев
* [SysEnumerators](https://github.com/mazzy-ax/SysEnumerators)
