# About `Net50.Preview6.FixMissingIsExternalInit`
This library contains a workaround for an issue in .NET 5 Preview 6 where, when using records or init -only properties, compiler raises an error about not finding `System.Runtime.CompilerServices.IsExternalInit`

Remove this library from your project once it has a version that fixex this issue.

Compiler uses this class internally for records and init -only properties but it wasn't included in Preview 6.  [[github](https://github.com/dotnet/roslyn/issues/45510#issuecomment-651831045)]

A fix to this issue has been merged to upcoming Preview 7. [[github](https://github.com/dotnet/runtime/pull/37763)]
