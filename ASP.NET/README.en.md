# ASP.NET Web API (REST)

## Summary

- [Project Presentation](#presentation)
- [Environment Configuration](#installation)
- [Execution](#execution)
- [Additional Information](#information)

## <span id="presentation">Project Presentation</span>

Basic initial structure for building an API with ASP.NET

## <span id="installation">Environment Configuration</span>

- Register Microsoft key in your Linux environment
    ```sh
    $ wget -q https://packages.microsoft.com/config/ubuntu/18.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
    $ sudo dpkg -i packages-microsoft-prod.deb
    ```
- Install the .NET SDK
    ```sh
    $ sudo add-apt-repository universe
    $ sudo apt-get install apt-transport-https
    $ sudo apt-get update
    $ sudo apt-get install dotnet-sdk-2.2
    ```
- Verify that the installation worked
    ```sh
    $ dotnet --version
    ```

## <span id="execution">Execution</span>

- Build the project images
    ```sh
    $ docker-compose build
    ```
- Put the container to work
    ```sh
    $ docker-compose up
    ```

## <span id="information">Additional Information</span>

- To create the base skeleton for ASP.NET Web API projects
    ```sh
    $ dotnet new webapi -o <project_name>
    ```
- To run application with an observer of changes in the code
    ```sh
    $ dotnet watch run
    ```
