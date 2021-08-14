# ASP.NETCore 6.0 Minimal API

Contains source code of ASP.NET Core Minimal API Building Microservice

[![.NET](https://github.com/executeautomation/ASPNETCore_MinimalAPI/actions/workflows/dotnet.yml/badge.svg)](https://github.com/executeautomation/ASPNETCore_MinimalAPI/actions/workflows/dotnet.yml)

## The Repo contains following code covered

* ASP NET Core Minimal API code
* ASP NET Core with Entity Framework
* Entity Framework with DataSeeder
* Repository Pattern for Data
* Swagger Support

## Complete Video Tutorial

[![Youtube Video](https://github.com/executeautomation/ASPNETCore_MinimalAPI/blob/main/Image/asp.png)](https://www.youtube.com/playlist?list=PL6tu16kXT9PrlCX-b1o0WdBc56rXHJXLy)

## Install instructions:-

* run sql server docker with the following code (change the SA_PASSWORD)

```powershell
docker run  -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=Password%1#29' -p 1433:1433 -v sqlvolume:/var/opt/mssql --name sqlserver -h sqlserver --network=aspnetwork -it mcr.microsoft.com/mssql/server:2019-latest
```

* check the connection string in "appsettings.json" file if you change connection settings like password...

* run the following command in the project directory to create the database and tables:-

```powershell
dotnet ef database update
```

* run the application with "seeddata" argument:-

```powershell
dotnet run seeddata
```
