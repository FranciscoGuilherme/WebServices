# ASP.NET Web API (REST)

## Summary

- [Project Presentation](#presentation)
- [Environment Configuration](#installation)
- [Execution](#execution)

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
