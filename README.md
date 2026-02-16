# Maximino Kokots

**`Full Stack Developer`**

O meu nome é Maximino Kokots, tenho 22 anos e sou de Portugal. Concluí a minha licenciatura de Engenheria de Telecomunicações e Informática no Instituto Superior de Engenharia do Porto (ISEP), e de momento estou a à procura de trabalho e a realizar em regime parcial algumas cadeiras de mestrado, Engenharia de software. Profissionalmente ainda só tive a oportunidade de estagiar na Samsys - Consultoria e Soluções Informáticas em Ermesinde, onde tive a possibilidade de fortalecer uma componente de um produto já em funcionamento, a gestão de estados, da aplicação Assistsys - Plataforma de Assistência Técnica. Para o desenvolvimento desta aplicação, tive que mexer tanto no backend como no Frontend, utilizando C# e TypeScript, respetivamente. Em baixo irei disponibilizar algumas informações de trabalhos desenvolvidos ao longo do meu percurso acadêmico, assim como os trabalhos no meu perfil.

### Linguagens e ferramentas

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/Javascript-%23007ACC.svg?style=for-the-badge&logo=javascript&logoColor=white)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=cplusplus&logoColor=white)
![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white)
![C](https://img.shields.io/badge/-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-%23C0392B.svg?style=for-the-badge&logo=css3&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-%23FF6600.svg?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![React Native](https://img.shields.io/badge/react%20native-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![SQL Server](https://img.shields.io/badge/sql%20server-%23CC2927.svg?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Bitbucket](https://img.shields.io/badge/bitbucket-%230052CC.svg?style=for-the-badge&logo=bitbucket&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/azure%20devops-%230078D7.svg?style=for-the-badge&logo=azuredevops&logoColor=white)
#

### Estatísticas

<p align="left">
  <img 
    alt="GitHub Stats" 
    height="200" 
    style="padding-right: 10px;" 
    src="https://github-stats-card-generator.vercel.app/api/svg?username=max1124&theme=radical" 
  />
  <img 
    alt="Tecnologias" 
    height="200" 
    style="padding-right: 10px;"  
    src="https://github-stats-card-generator.vercel.app/api/svg?username=max1124&type=languages&theme=radical"
  />
</p>

### Trabalhos Acadêmicos

### [Sistema de Gestão de Bibliotecas (React)](https://github.com/Max1124/DSSMV_ProjectDroid_1211378_1240708) - Aplicação móvel para Android, desenvolvida com boa arquitetura, separação de responsabilidades, código limpo e organizado, consumindo uma API REST fornecida pelos professores
**Descrição das Camadas e Funções**
- **Fragment** - onde se encontra a lógica da aplicação e a interação com o utilizador, com a configuração de cliques, botões, popups e decide quando se deve chamar as funções que comunicam com o backend
- **HttpOperation** - onde se encontram todas as funções que pedem dados à API, através dos seus diferentes endpoints
- **JsonHandler** - responsável por tranformar o JSON recebido da API em DTOs (Data Tranfer Object), onde como o nome indica irá armazenar temporariamente os dados do objeto, esta separação permite o parsing do JSON isolado
- **Mapper** - responsável por converter os DTOs em models concretos da aplicação (que são utilizados pela UI)
- **Adapter** - ponte entre os models e o RecyclerView (lista), tranformando cada objeto em elementos visuais na interface
- **UI (Interface do Utilizador)** - interface do utilizador, onde o mesmo consegue visualizar botões, listas, mensagens, entre outros
#

### [Sistema de Gestão de Biblioteca (React Native)](https://github.com/Max1124/Library_Management_React) - Aplicação para Android que permite gerenciar bibliotecas, consumindo uma API REST fornecida pelos professores e uma API externa para autenticação
**Descrição das Camadas e Funções**
- **Service** - Responsável por buscar dados da API.
- **Pasta Utils** - Contém funções auxiliares para manter o código limpo e facilitar testes unitários.
- **Pasta context** - esta pasta dentro da aplicação contêm é responsável por gerir o estado de forma unidirecional e previsível, dentro desta pasta podemos encontrar os seguintes elementos: Action, appContext, appProvider e Reducer. Utilizando arquitetura Flux:  
  `View -> Action -> Dispatcher -> Store -> View`
  - **Action**: lista as ações da aplicação. Exemplo:
    - `buscarBibliotecas()`: dispara ação para buscar bibliotecas
    - `buscarBibliotecasSucesso(lista)`: atualiza o estado com os dados recebidos
    - `buscarBibliotecasErro(mensagem)`: atualiza o estado em caso de erro
  - **Reducer**: recebe a action e atualiza o estado da aplicação
  - **Provider**: 
    1. Chama funções do **Service**
    2. Expõe funções para as screens usarem
    3. Processa actions via **dispatch**, atualizando o estado conforme o resultado do Service (sucesso ou erro)
- **Fluxo resumido do Provider**:
  1. Dispatch identifica a ação a executar
  2. Reducer atualiza o estado conforme a ação
  3. Service busca os dados na API
  4. Dispatch atualiza novamente o estado com sucesso ou erro
#

### [Sistemas Distribuídos](https://github.com/Max1124/sisdis) - Aplicação inicialmente monolítica, reconstruída para uma arquitetura distribuída com comunicação assíncrona entre serviços com a utilização de AMQP e RabbitMQ
**Descrição**:
- **Aplicação Monolítica** - aplicação onde todas as funcionalidades então dentro de um único bloco de código, exemplo: frontend, backend e base de dados todos juntos
- **Arquitetura Distribuída** - aplicação dividida em vários serviços independentes entre si (cada serviço é responsável por uma funcionalidade específica), no entanto que conseguem comunicar entre si
- **AMQP** - protocolo de mensagens usado para enviar informações entre diferentes sistemas, permitindo comunicação assíncrona, ou seja, o serviço que envia a mensagem não necessita de esperar pela receção da informação enviada para poder continuar a funcionar normalmente
- **RabbitMQ** - broker de mensagens que funciona com AMQP. Tem como função receber, armazenar e entregar mensagens entre os serviços da aplicação, facilitando a entrega segura da mensagem, mesmo com o serviço offline
#
