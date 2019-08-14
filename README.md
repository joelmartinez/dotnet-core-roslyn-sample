Using Roslyn in .NET Core
-------------------------
This is a simple example of using Roslyn to compile some code from a string,
 load it into the currently executing `AppDomain`, and activate and invoke the code.
 It is based on [this article](http://www.tugberkugurlu.com/archive/compiling-c-sharp-code-into-memory-and-executing-it-with-roslyn)
 and was adapted for the slightly different API surface area on .net core.
 
## Dependencies
This was written to work with [.NET Core 2.2](https://dotnet.microsoft.com/download). 

## Running the Sample

This example uses bash, but you can run this from any [dotnet core supported platform](https://docs.microsoft.com/en-us/dotnet/standard/cross-platform/)

```bash
git clone https://github.com/joelmartinez/dotnet-core-roslyn-sample.git
cd dotnet-core-roslyn-sample
dotnet restore && dotnet run
```
