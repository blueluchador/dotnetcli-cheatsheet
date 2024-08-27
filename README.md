# dotnet cli Cheat Sheet

More commands will be added periodically. Please come back often.

### `dotnet new` Commands

| Command                                      | Description                                |
|----------------------------------------------|--------------------------------------------|
| `dotnet new`                                 | Create a new project or solution           |
| `dotnet new sln`                             | Create a new solution file                 |
| `dotnet new console`                         | Create a new console application           |
| `dotnet new classlib`                        | Create a new class library                 |
| `dotnet new mvc`                             | Create a new ASP.NET Core Web App          |
| `dotnet new xunit`                           | Create a new XUnit test project            |
| `dotnet new list`                            | List all available templates               |

### `dotnet sln` Commands

| Command                                                          | Description                                    |
|------------------------------------------------------------------|------------------------------------------------|
| `dotnet sln`                                                     | Manage solution files                          |
| `dotnet sln list`                                                | List all projects in a solution file           |
| `dotnet sln mySolution.sln add myProject/myProject.csproj`       | Add a C# project to a solution                 |
| `dotnet sln mySolution.sln remove myProject/myProject.csproj`    | Remove a C# project from a solution            |
| `dotnet sln todo.sln add **/*.csproj`                            | Add multiple C# projects to a solution         |

### `dotnet run` Commands

| Command                                                    | Description                                |
|------------------------------------------------------------|--------------------------------------------|
| `dotnet run`                                               | Run the project in the current directory   |
| `dotnet run --project ./projects/helloWorld/helloWorld.csproj` | Run the specified project                  |
| `dotnet myapp.dll`                                         | Run a framework-dependent app named myapp.dll|

### `dotnet clean` Commands

| Command                                          | Description                                        |
|--------------------------------------------------|----------------------------------------------------|
| `dotnet clean`                                   | Clean the output of a project                      |
| `dotnet clean --configuration Release`           | Clean a project built using the Release configuration|

### `dotnet publish` Commands

| Command                                                | Description                                        |
|--------------------------------------------------------|----------------------------------------------------|
| `dotnet publish`                                       | Publish the project in the current directory       |
| `dotnet publish ~/projects/myApp/myApp.csproj`         | Publish the application using the specified project file|

### `dotnet pack` Commands

| Command                                                       | Description                                    |
|---------------------------------------------------------------|------------------------------------------------|
| `dotnet pack`                                                 | Build the project and create NuGet packages    |
| `dotnet pack --no-build --output nupkgs`                      | Pack the project but skip the build            |
| `dotnet pack /p:PackageVersion=3.0.0`                         | Set the package version while packing          |
