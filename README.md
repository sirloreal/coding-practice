# coding-practice
Some coding practice, mostly focused on .NET - Space to add other katas and concepts. 

From .NET Core 3.0 you can use the command: `dotnet new gitignore` to generate a customizable .gitignore file in your git repo (That's what I did for this one)

Use the following steps to create a new web api project:
```
dotnet new webapi --use-controllers -o ProjectName
cd ProjectName
dotnet add package Microsoft.EntityFrameworkCore.InMemory
```

Run the following to trust the https development certificate:
```
dotnet dev-certs https --trust
```

Use the following command to run the application:
```
dotnet run --launch-profile https
```

With this template set up, you can add a new controller scaffold for the project.

Use the following commands:
```
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet add package Microsoft.EntityFrameworkCore.SqlServer
dotnet add package Microsoft.EntityFrameworkCore.Tools
dotnet tool uninstall -g dotnet-aspnet-codegenerator
dotnet tool install -g dotnet-aspnet-codegenerator
dotnet tool update -g dotnet-aspnet-codegenerator
```

Then:
```
dotnet aspnet-codegenerator controller -name YourNameController -async -api -m YourModel -dc YourContext -outDir Controllers
```

