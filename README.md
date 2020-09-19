# Аналог интерфейса [ICollection\<T\>](https://docs.microsoft.com/ru-ru/dotnet/api/system.collections.generic.icollection-1?view=netframework-4.8) в Ax2009

Стало не хватать в аксапте интерфейса, в который можно было бы обернуть такие объекты как `Set`, `List`, а также объекты CLR типа [`List<T>`](https://docs.microsoft.com/ru-ru/dotnet/api/system.collections.generic.list-1?view=netframework-4.8), [`SortedSet<T>`](https://docs.microsoft.com/ru-ru/dotnet/api/system.collections.generic.sortedset-1?view=netframework-4.8).

Реализовать методы :
* `Add(anytype item)`
* `Any`
* `Concat(ICollection collection)`
* `Contains(anytype item)`
* `Count`
* `Except(ICollection collection)`
* `Min`
* `Max`
* `Remove(anytype item)`
* `Single`
* `Sum`
* `Union(ICollection collection)`

Отнаследовать от :
* `Enumerable`

## Class diagram
<img src="out\schema\ICollection.png" alt="схема">

### Необходимые референсы в аксапте
* `System.Linq`
* `System.Core`

### Dependencies
* [SysEnumerators](https://github.com/mazzy-ax/SysEnumerators)
* [.Net Framework 4 Support](https://github.com/d-tolstov/Ax2009-NetFramework4-Support)
* [SysCLRReflection](https://github.com/d-tolstov/Ax2009-SysCLRReflection)
* [IDictionary](https://github.com/d-tolstov/Ax2009-IDictionary)