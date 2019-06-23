# ASP.NET Web API (REST)

Read this documentation in English: [Click here](https://github.com/FranciscoGuilherme/WebServices/blob/ASP.NET/ASP.NET/README.en.md)

## Sumário

- [Apresentação do projeto](#apresentacao)
- [Configuração do ambiente](#instalacao)
- [Execução](#execucao)

## <span id="apresentacao">Apresentação do projeto</span>

Estrutura inicial básica para a construção de uma API com ASP.NET

## <span id="instalacao">Configuração do ambiente</span>

- Registre em seu ambiente Linux a chave da Microsoft
    ```sh
    $ wget -q https://packages.microsoft.com/config/ubuntu/18.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
    $ sudo dpkg -i packages-microsoft-prod.deb
    ```
- Instale o .NET SDK
    ```sh
    $ sudo add-apt-repository universe
    $ sudo apt-get install apt-transport-https
    $ sudo apt-get update
    $ sudo apt-get install dotnet-sdk-2.2
    ```
- Verifique se a instalação funcionou
    ```sh
    $ dotnet --version
    ```

## <span id="execucao">Execução</span>

- Construa as imagens do projeto
    ```sh
    $ docker-compose build
    ```
- Coloque o container para funcionar
    ```sh
    $ docker-compose up
    ```
