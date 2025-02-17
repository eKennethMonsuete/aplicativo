# aplicativo

1. API (Interface)
Contém os Controllers que lidam com as requisições HTTP.
Converte os dados de entrada em DTOs e chama os serviços.
Retorna as respostas para o cliente (JSON, HTTP status, etc.).
 2. Application (Serviços e Casos de Uso)
Aplica a lógica de negócio e validações.
Utiliza os repositórios do Domain para manipular dados.
Implementa casos de uso (exemplo: "Cadastrar Usuário").
 3. Domain (Entidades e Regras de Negócio)
Define as Entidades principais do sistema.
Contém Interfaces de Repositório para abstrair o banco de dados.
Regras de negócio independentes de banco ou frameworks.
 4. Infrastructure (Acesso a Dados e Configurações)
Implementa os repositórios concretos usando Entity Framework.
Configurações de banco de dados e outras integrações.
Pode conter repositórios para armazenar logs ou acessar APIs externas.