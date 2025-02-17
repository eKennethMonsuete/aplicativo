# aplicativo

1. API (Interface)
Cont�m os Controllers que lidam com as requisi��es HTTP.
Converte os dados de entrada em DTOs e chama os servi�os.
Retorna as respostas para o cliente (JSON, HTTP status, etc.).
 2. Application (Servi�os e Casos de Uso)
Aplica a l�gica de neg�cio e valida��es.
Utiliza os reposit�rios do Domain para manipular dados.
Implementa casos de uso (exemplo: "Cadastrar Usu�rio").
 3. Domain (Entidades e Regras de Neg�cio)
Define as Entidades principais do sistema.
Cont�m Interfaces de Reposit�rio para abstrair o banco de dados.
Regras de neg�cio independentes de banco ou frameworks.
 4. Infrastructure (Acesso a Dados e Configura��es)
Implementa os reposit�rios concretos usando Entity Framework.
Configura��es de banco de dados e outras integra��es.
Pode conter reposit�rios para armazenar logs ou acessar APIs externas.