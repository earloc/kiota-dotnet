﻿# Contributing to Kiota Dotnet

Kiota Dotnet is a mono-repo containing source code for the following packages:

## Libraries

| Library                                                              | NuGet Release                                                                                                                                                                              |
|----------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Abstractions](./src/abstractions/README.md)                         | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Abstractions?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Abstractions/)                       |
| [Authentication - Azure](./src/authentication/azure/README.md)       | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Authentication.Azure?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Authentication.Azure/)       |
| [Http - HttpClientLibrary](./src/http/httpClient/README.md)          | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Http.HttpClientLibrary?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Http.HttpClientLibrary/)   |
| [Serialization - JSON](./src/serialization/json/README.md)           | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Serialization.Json?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Serialization.Json/)           |
| [Serialization - FORM](./src/serialization/form/README.md)           | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Serialization.Form?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Serialization.Form/)           |
| [Serialization - TEXT](./src/serialization/text/README.md)           | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Serialization.Text?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Serialization.Text/)           |
| [Serialization - MULTIPART](./src/serialization/multipart/README.md) | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Serialization.Multipart?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Serialization.Multipart/) |
| [Bundle](./src/bundle/README.md)                                     | [![NuGet Version](https://img.shields.io/nuget/vpre/Microsoft.Kiota.Bundle?label=Latest&logo=nuget)](https://www.nuget.org/packages/Microsoft.Kiota.Bundle/)                                   |


Kiota Dotnet is open to contributions. There are a couple of different recommended paths to get contributions into the released version of this library.

__NOTE__ A signed a contribution license agreement is required for all contributions, and is checked automatically on new pull requests. Please read and sign [the agreement](https://cla.microsoft.com/) before starting any work for this repository.

## File issues

The best way to get started with a contribution is to start a dialog with the owners of this repository. Sometimes features will be under development or out of scope for this SDK and it's best to check before starting work on contribution. Discussions on bugs and potential fixes could point you to the write change to make.

## Submit pull requests for bug fixes and features

Feel free to submit a pull request with a linked issue against the __main__ branch.  The main branch will be updated frequently.
## Commit message format

To support our automated release process, pull requests are required to follow the [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/)
format.
Each commit message consists of a __header__, an optional __body__ and an optional __footer__. The header is the first line of the commit and
MUST have a __type__ (see below for a list of types) and a __description__. An optional __scope__ can be added to the header to give extra context.

```
<type>[optional scope]: <short description>
<BLANK LINE>
<optional body>
<BLANK LINE>
<optional footer(s)>
```

The recommended commit types used are:

- __feat__ for feature updates (increments the _minor_ version)
- __fix__ for bug fixes (increments the _patch_ version)
- __perf__ for performance related changes e.g. optimizing an algorithm
- __refactor__ for code refactoring changes
- __test__ for test suite updates e.g. adding a test or fixing a test
- __style__ for changes that don't affect the meaning of code. e.g. formatting changes
- __docs__ for documentation updates e.g. ReadMe update or code documentation updates
- __build__ for build system changes (gradle updates, external dependency updates)
- __ci__ for CI configuration file changes e.g. updating a pipeline
- __chore__ for miscallaneous non-sdk changes in the repo e.g. removing an unused file

Adding an exclamation mark after the commit type (`feat!`) or footer with the prefix __BREAKING CHANGE:__ will cause an increment of the _major_ version.