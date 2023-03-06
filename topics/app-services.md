## Serviços de Aplicativo

O Serviço de Aplicativo do Azure **(App services)** é um serviço baseado em HTTP para hospedar aplicativos da web, APIs REST e back-ends móveis, é uma estrutura pronta **(Paas)**. Você pode desenvolver em sua linguagem favorita, seja .NET, .NET Core, Java, Ruby, Node.js, PHP ou Python. Os aplicativos são executados e escalonados com facilidade em ambientes baseados em Windows e Linux.

Aqui você paga pelos recursos de computação do Azure utilizados, determinados pelo plano de serviço de aplicativo em que você executa seus aplicativos.

### Criando uma aplicação

- A documentação completa pode ser encontrada [aqui](https://learn.microsoft.com/pt-br/azure/app-service/)
- Para o exemplo usaremos o vscode e subiremos uma aplicação ASP.NET;
- No vscode instalar o complemento **Azure App Service**;
- Realizar a autenticação na conta Azure;
- Criar a aplicação teste:
  - No terminal criar o diretório e abrir o mesmo no vscode: 
  ```
  mkdir MyFirstAzureWebApp
  code MyFirstAzureWebApp
  ```
  - Com o vscode aberto na pasta do projeto criar um aplicativo:
  ```
  dotnet new webapp -f net6.0
  ```
  - Para verificar se tudo deu certo abrir o aplicativo recém criado:
  ```
  dotnet run --urls=https://localhost:5001/
  ```
- Se tudo correu bem com a criação da aplicação ao acessar o link no browser a mesma será aberta;
- Agora a publicação na Azure:
  - Acesse o menu do Azure na barra lateral do vscode;
  - Escolha sua inscrição e a abra, dentre as opções escolha "App Services";
  - Em "App Services" clique com o botão direito e escolha "Create New Web App";
  - Defina um nome único;
  - Defina a stack (.NET 6 no meu caso);
  - Defina a forma de cobrança (no meu caso escolhi Free);
  - Após esses passos a configuração será realizada e se tudo der certo nos será mostrada uma mensagem de sucesso;
  - Agora para ver a aplicação publicada basta ir no painel do Azure, escolher "Serviços de Aplicativos" (ou App Services), clicar no serviço que acabamos de criar e por fim clicar no link referente ao dominio, com isso nossa aplicação deve ser mostrada em uma nova aba;