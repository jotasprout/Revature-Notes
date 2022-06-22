## dotnet cmds
- To create a new console application, `dotnet new console -n appName`
- `dotnet run` to run your program
    - dotnet run actually runs dotnet build under the hood -> dotnet build && dotnet run
- `dotnet build` to just compile your program
- make sure to actually be at the project folder before you execute any of these commands


## Gitignore
.gitignore file is a file telling git to ignore certain files/folders and do not track/add these to the repository.
`dotnet new gitignore` at the root of your repository