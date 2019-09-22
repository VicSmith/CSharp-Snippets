# CSharp-Snippets
Snippets of CSharp AKA C#
## Just Added Feature branch
### Second Commit in the new Feature Branch
# Commands needed to use Visual Studio Code and .Net Core ( dotnet-sdk-2.2.109-win-x64 ) on a Windows 10 Machine.

## 1- Download .Net Core - https://dotnet.microsoft.com/download 

## 2- After download and install navigate to the project directory using the command prompt and run "dotnet".

#### You should get:  

            λ dotnet

            Usage: dotnet [options]
            Usage: dotnet [path-to-application]

            Options:
            -h|--help         Display help.
            --info            Display .NET Core information.
            --list-sdks       Display the installed SDKs.
            --list-runtimes   Display the installed runtimes.

            path-to-application:
            The path to an application .dll file to execute.


## 2- While in the project direcotry take a look at the project types using the command prompt and run "dotnet new" from the command prompt.

#### You should get:  
            λ dotnet new

            Welcome to .NET Core!
            ---------------------
            Learn more about .NET Core: https://aka.ms/dotnet-docs
            Use 'dotnet --help' to see available commands or visit: https://aka.ms/dotnet-cli-docs

            Telemetry
            ---------
            The .NET Core tools collect usage data in order to help us improve your experience. The data is anonymous and doesn't include command-line arguments. The data is collected by Microsoft and shared with the community. You can opt-out of telemetry by setting the DOTNET_CLI_TELEMETRY_OPTOUT environment variable to '1' or 'true' using your favorite shell.

            Read more about .NET Core CLI Tools telemetry: https://aka.ms/dotnet-cli-telemetry

            ASP.NET Core
            ------------
            Successfully installed the ASP.NET Core HTTPS Development Certificate.
            To trust the certificate run 'dotnet dev-certs https --trust' (Windows and macOS only). For establishing trust on other platforms refer to the platform specific documentation.
            For more information on configuring HTTPS see https://go.microsoft.com/fwlink/?linkid=848054.
            Getting ready...
            Usage: new [options]

            Options:
            -h, --help          Displays help for this command.
            -l, --list          Lists templates containing the specified name. If no name is specified, lists all templates.
            -n, --name          The name for the output being created. If no name is specified, the name of the current directory is used.
            -o, --output        Location to place the generated output.
            -i, --install       Installs a source or a template pack.
            -u, --uninstall     Uninstalls a source or a template pack.
            --nuget-source      Specifies a NuGet source to use during install.
            --type              Filters templates based on available types. Predefined values are "project", "item" or "other".
            --dry-run           Displays a summary of what would happen if the given command line were run if it would result in a template creation.
            --force             Forces content to be generated even if it would change existing files.
            -lang, --language   Filters templates based on language and specifies the language of the template to create.


            Templates                                         Short Name         Language          Tags
            ----------------------------------------------------------------------------------------------------------------------------
            Console Application                               console            [C#], F#, VB      Common/Console
            Class library                                     classlib           [C#], F#, VB      Common/Library
            Unit Test Project                                 mstest             [C#], F#, VB      Test/MSTest
            NUnit 3 Test Project                              nunit              [C#], F#, VB      Test/NUnit
            NUnit 3 Test Item                                 nunit-test         [C#], F#, VB      Test/NUnit
            xUnit Test Project                                xunit              [C#], F#, VB      Test/xUnit
            Razor Page                                        page               [C#]              Web/ASP.NET
            MVC ViewImports                                   viewimports        [C#]              Web/ASP.NET
            MVC ViewStart                                     viewstart          [C#]              Web/ASP.NET
            ASP.NET Core Empty                                web                [C#], F#          Web/Empty
            ASP.NET Core Web App (Model-View-Controller)      mvc                [C#], F#          Web/MVC
            ASP.NET Core Web App                              webapp             [C#]              Web/MVC/Razor Pages
            ASP.NET Core with Angular                         angular            [C#]              Web/MVC/SPA
            ASP.NET Core with React.js                        react              [C#]              Web/MVC/SPA
            ASP.NET Core with React.js and Redux              reactredux         [C#]              Web/MVC/SPA
            Razor Class Library                               razorclasslib      [C#]              Web/Razor/Library/Razor Class Library
            ASP.NET Core Web API                              webapi             [C#], F#          Web/WebAPI
            global.json file                                  globaljson                           Config
            NuGet Config                                      nugetconfig                          Config
            Web Config                                        webconfig                            Config
            Solution File                                     sln                                  Solution

            Examples:
                dotnet new mvc --auth Individual
                dotnet new xunit
                dotnet new --help

## 3- While in the project initialize a new console project and run "dotnet new console -o MinimalCSharpProgramProject" from the command prompt.

#### You should get:                  
                λ dotnet new console -o MinimalCSharpProgramProject
                The template "Console Application" was created successfully.

                Processing post-creation actions...
                Running 'dotnet restore' on MinimalCSharpProgramProject\MinimalCSharpProgramProject.csproj...
                Restoring packages for <dir Path> Repos\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject\MinimalCSharpProgramProject.csproj...
                Generating MSBuild file <dir Path> CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject\obj\MinimalCSharpProgramProject.csproj.nuget.g.props.
                Generating MSBuild file <dir Path> pos\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject\obj\MinimalCSharpProgramProject.csproj.nuget.g.targets.
                Restore completed in 223.63 ms for \CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject\MinimalCSharpProgramProject.csproj.

                Restore succeeded.


### Running dotnet new console pulled down the project template from Microsoft and did initial setup.

## 4- Change Direcotry (CD) into the new project by typing "cd MinimalCSharpProgramProject"  
## 5- Install the C# Extension in Visual Studio Code from: https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp
## 6- Type "code ." and your project opens ready to work in Visual Studio Code.
## 7- Agree by saying Yes to the pop up from the Microsoft Ominisharp C# Visual Studio Code Extension so you can debug etc in Visual Studio Code.
## 8- Using Visual Studio Code, right click on the Program.cs file and select " Open in Terminal ". 
## 9- In the Visual Studio Code terminal, type "dotnet restore". 

#### You should get:  

                Windows PowerShell
                Copyright (C) Microsoft Corporation. All rights reserved.

                PS C:<Repo Path>\Vic's Repos\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject> dotnet restore
                Restore completed in 29.86 ms for <Repo Path> Vic's Repos\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject\MinimalCSharpProgramProject.csproj.
             


## 11- In the Visual Studio Code terminal, type "dotnet run Program.cs" or "dotnet run" and you should see your Hello World Program run.

#### You should get: 

            PS C:\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject> dotnet run
            Hello World!
            PS C:\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject> dotnet run Program.cs
            Hello World!
            PS C:\Vic's Repos\CSharp-Snippets\CSharp-Snippets\MinimalCSharpProgramProject>

