# Maximino Kokots

**`Full Stack Software Engineer`**

I hold a Bachelor's degree in Telecommunications and Informatics Engineering from the Instituto Superior de Engenharia do Porto (ISEP) and I am currently pursuing a Master's degree in Software Engineering, while actively seeking new professional opportunities.

I completed an internship at Samsys – IT Consulting and Solutions, where I contributed to the development of the Assistsys application – a technical support management platform, with a focus on improving the state management component.

During this experience, I worked in full stack development using C# on the backend and TypeScript on the frontend.

Throughout my academic path, I have developed several projects, which are listed below and available on my GitHub profile.

### Languages and Tools

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
![Scala](https://img.shields.io/badge/scala-%23DC322F.svg?style=for-the-badge&logo=scala&logoColor=white)
![SQL Server](https://img.shields.io/badge/sql%20server-%23CC2927.svg?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Bitbucket](https://img.shields.io/badge/bitbucket-%230052CC.svg?style=for-the-badge&logo=bitbucket&logoColor=white)
![Azure DevOps](https://img.shields.io/badge/azure%20devops-%230078D7.svg?style=for-the-badge&logo=azuredevops&logoColor=white)
#

### Statistics

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

### Academic Projects

### [Library Management System (React)](https://github.com/Max1124/DSSMV_ProjectDroid_1211378_1240708) - Mobile Android application developed with a clean architecture approach, separation of concerns, and structured code, consuming a REST API provided by lecturers
**Layer Description and Responsibilities**
- **Fragment** - contains application logic and user interaction, handling UI events (buttons, dialogs, popups) and triggering backend communication functions
- **HttpOperation** - contains all functions responsible for API requests through different endpoints
- **JsonHandler** - responsible for converting JSON responses into DTOs (Data Transfer Objects), isolating parsing logic
- **Mapper** - converts DTOs into application models used by the UI
- **Adapter** - bridge between models and RecyclerView, transforming objects into visual UI elements
- **UI (User Interface)** - presentation layer where users interact with buttons, lists, messages, etc
#

### [Library Management System (React Native)](https://github.com/Max1124/Library_Management_React) - Android application for library management, consuming a REST API provided by lecturers and an external authentication API
**Layer Description and Responsibilities**
- **Service** - responsible for fetching data from the API
- **Utils folder** - contains helper functions to keep code clean and support unit testing
- **Context folder** - manages state in a unidirectional and predictable way using Flux architecture: 
  `View -> Action -> Dispatcher -> Store -> View`
  - **Action**: defines application actions, e.g.:
    - `fetchLibraries()`: triggers library retrieval
    - `fetchLibrariesSuccess(data)`: updates state with received data
    - `fetchLibrariesError(message)`:handles errors
  - **Reducer**: receives actions and updates application state
  - **Provider**: 
    1. Calls Service functions
    2. Exposes functions to screens
    3. Processes dispatched actions and updates state accordingly
- **Provider flow summary:**
  1. Dispatch identifies the action
  2. Reducer updates state
  3. Service fetches data from API
  4. Dispatch updates state with success or error
#

### [Distributed Systems](https://github.com/Max1124/sisdis) - Application initially monolithic, later refactored into a distributed architecture with asynchronous communication using AMQP and RabbitMQ
**Description**:
- **Monolithic Application** - system where all functionalities (frontend, backend, database) are contained in a single codebase
- **Distributed Architecture** - system split into independent services that communicate with each other
- **AMQP** - messaging protocol enabling asynchronous communication between services without blocking execution
- **RabbitMQ** - message broker responsible for receiving, storing, and delivering messages reliably
#

### [Secure Software Development (VendNet)](https://github.com/Af-Oliveira/desofs2026_thu_ffs_5) - Secure backend API for vending machine management, focusing on authentication, access control, and continuous quality within a DevSecOps pipeline.
**Description**:
- **Project Goal** - backend system for managing products, machines, sales, and telemetry in a vending network with strong security requirements
- **Spring Boot API** - REST API structured in layers (controller, service, repository) with clean separation of business logic
- **JWT + RBAC** - token-based authentication and role-based access control (CUSTOMER, OPERATOR, ADMINISTRATOR)
- **Security & Quality Testing** - black-box, white-box, integration, and abuse-case testing (e.g. missing JWT, HMAC tampering, concurrency issues)
- **DevSecOps Pipeline** - automated validation using SAST, SCA, IAST, DAST, and SonarQube, blocking deployments on failures
- **Result** - Quality Gate passed (>80%) and improved delivery confidence, security, and stability
#

### [Nurse Scheduling System (Scala)](https://github.com/tap-mei-isep/tap-pj-ncf-04) - System for generating nurse schedules using hybrid optimization and functional validation.
**Description**:
- **Project Goal** - generate nurse schedules from XML data while respecting operational constraints and maximizing seniority-based preferences
- **Functional Scala Architecture** - immutable data structures, pure functions, and modular design for parsing, validation, and scheduling logic
- **Hybrid Scheduling Approach** - combination of exact (Backtracking with Branch and Bound) and heuristic (Genetic Algorithm) methods, selecting the best solution based on instance complexity
- **Constraints Validation** - enforcement of capacity limits, shift conflicts, consecutivity rules, and global schedule consistency
- **Testing & Quality** - unit, functional, and property-based testing using ScalaCheck, including edge-case and failure scenario generators
- **Result** - robust and extensible solution capable of producing valid and high-quality schedules across different complexity levels 
#
