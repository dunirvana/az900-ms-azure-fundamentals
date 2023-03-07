## Funções Azure

- Funções **(Azure Functions)** são uma solução serverless que permite o foco apenas no código, toda infraestrutura é fornecida e mantida para que a preocupação seja focada apenas no código;

- As funções funcionam baseadas em gatilhos **(triggers)** que são o momento que essas funções devem ser executadas, são eles que causam a execução de uma função. Um gatilho define como uma função é invocada e uma função deve ter exatamente um gatilho. Gatilhos têm dados associados, que geralmente são fornecidos como o conteúdo da função;

- Para saber mais sobre os gatilhos bas consultar [aqui](https://learn.microsoft.com/pt-br/azure/azure-functions/functions-triggers-bindings?tabs=csharp);

- Praticando:
  - No vscode instalar o complemento "Azure Functions";
  - No vscode abrir a pasta local onde o código será salvo;
  - No menu lateral expandir a opção "Azure", expandir a assinatura desejada;
  - Nas opções da assinatura clicar com o botão direito em "Funcion App" e escolher a opção "Create Funcion App in Azure";
  - Defina o nome da função:
    - Selecione a stack (no nosso caso .NET 6);
    - Escolha a localização (no nosso caso foi recomendado East US);
    - Depois desses passos a ferramenta realizará todas as configurações e criará uma "Function App";
  - Nas opções da assinatura expandir "Funcion App" e escolher a função recém criada;  
  - Ainda no menu lateral descer até "WORKSPACE" e clicar no botão "raio" que é referente a "Create Function":
    - Selecione o diretório onde ficará a função;
    - Selecione a linguagem, no nosso caso C#;
    - Selecione a stack (no nosso caso .NET 6);
    - Selecione o gatilho (trigger, no nosso caso HTTP);
    - Defina o nome para a função;
    - Defina o nome do namespace;
    - Defina os direitos de acesso (no nosso caso público/anonimo);
    - Selecione como abrir o projeto (no nosso caso Add to workspace);
    - Feito isso toda a estrutura do projeto será criada;
  - É possivel testar o código localmente, basta pressionar "F5" e abrir no browser a url, não esquecer de incluir o parâmetro ao final ("?name=Eduardo" por exemplo);
  - Para publicar a função:
    - Ainda no menu lateral descer até "WORKSPACE" e clicar no botão "nuvem" que é referente a "Deploy";
    - Escolha a opção "Deploy to Function App";
    - Escolha o diretório e depois a função;
    - Pronto, agora é possivel usar nossa função a partir do que esta publicado na Azure;




