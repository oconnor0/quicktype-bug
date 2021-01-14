# quicktype-bug

I am trying to convert the Plaid JSON API to C# classes using [quicktype](https://github.com/quicktype/quicktype).

I am running Quicktype version 15.0.258.

I have generated some sample JSON that matches their specification.

When I run `.\gen.bat`, or:

    quicktype --lang cs --namespace Plaid --out Plaid.cs .

I do not get a top-level class definition for `AccountsGet.Request.json` and the `Options` field for `AuthGet.Request.json` has the name `AccountsGetRequestOptions` even though that class is never used in the `AccountsGet.Request.json`.
