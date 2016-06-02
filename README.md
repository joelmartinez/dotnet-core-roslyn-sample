Using Roslyn in .NET Core
-------------------------
This is a simple example of using Roslyn to compile some code from a string,
 load it into the currently executing `AppDomain`, and activate and invoke the code.
 It is based on [this article](http://www.tugberkugurlu.com/archive/compiling-c-sharp-code-into-memory-and-executing-it-with-roslyn)
 and was adapted for the slightly different API surface area on .net core.
 
## Dependencies
This was written to work with [.NET Core RC2](https://github.com/dotnet/core/releases/tag/v1.0.0-rc2). 
In order to resolve the prerelease dependencies, you'll have to add the `aspnetcidev` myget feed. 
You can do so by adding or modifying the
[`~/.config/NuGet/NuGet.Config`](https://docs.nuget.org/consume/nuget-config-file) 
file (on mac) to include the `AspNetCiDev` key listed below:

```xml
<?xml version="1.0" encoding="utf-8"?>
<configuration>
  <activePackageSource>
    <add key="AspNetCiDev" value="https://www.myget.org/F/aspnetcidev/api/v3/index.json" />
    <add key="Official NuGet Gallery" value="https://www.nuget.org/api/v2/" />
  </activePackageSource>
</configuration>
```

## Running the Sample

```bash
git clone https://github.com/joelmartinez/dotnet-core-roslyn-sample.git
cd dotnet-core-roslyn-sample
dotnet restore && dotnet run
```
