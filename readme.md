# BaGet :baguette_bread:

A lightweight [NuGet service](https://docs.microsoft.com/en-us/nuget/api/overview) implementation.

## Getting Started

1. Install [.NET Core](https://www.microsoft.com/net/download/windows)
2. Run `git clone https://github.com/loic-sharma/BaGet.git`
3. Navigate to `.\BaGet\src\BaGet`
4. Start the service with `dotnet run`
5. Open the URL `http://localhost:5000/v3/index.json` in your browser

## Features

* Supports Sqlite and SQL Server to store metadata
* Supports local filesystem and Azure Blob Storage to store NuGet packages
* Supports Azure Search
* Supports read-through caching. For example, accessing `http://localhost:5000/v3/registration/newtonsoft.json/11.0.1.json`
will index [Newtonsoft.Json](https://www.nuget.org/packages/Newtonsoft.Json/11.0.1) using [nuget.org](https://www.nuget.org/)
* Can import download counts from [nuget.org](https://www.nuget.org)

Stay tuned, more features are planned!