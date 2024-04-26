## 4. Projeto da solução
Insira aqui a parte do projeto da solução


### 4.1. Tecnologias utilizadas
Optamos por utilizar prioritariamente as tecnologias, bibliotecas, softwares e frameworks da Microsoft devido a qualidade e facilidade de integração. Vamos utilizar a IDE Visual Studio Community 2022 e o projeto será desenvolvido em Blazor, um framework de desenvolvimento Web da Microsoft que permite a utilização de código C# junto ao HTML nas páginas web. Para o banco de dados, vamos utilizar o SQL Server, e para fazer a conexão com banco de dados vamos utilizar o EntityFrameworkCore junto ao ASP.NET Core. Para a autenticação e login, iremos utilizar o OpenID Connect (OIDC) junto ao Microsoft Identity para permitir o login apenas de contas Microsoft, pois dessa forma aumentamos o nível de segurança ao delegar o processo de login e recuperação de senhas para a Microsoft. Optamos também por utilizar um framework front-end da Microsoft chamado Fluent UI para a estilização da ferramenta,  também por possuir recursos prontos interessantes como menus e tabelas com filtros. Para a publicação da ferramenta, iremos utilizar o Azure App Services.

### 4.2. Requisitos funcionais e não funcionais
Aqui ficará um breve texto sobre os requisitos

### Requisitos Funcionais
|  ID	|  Descrição do Requisito	|	Prioridade  |
|  ---  |  ---  |  ---  |
|  RF-001  |  Fazer login através de conta microsoft  |
|  RF-002  |  Visualizar os produtos do estoque  |
|  RF-003  |  Cadastrar produtos  |
|  RF-004  |  Editar produtos  |
|  RF-005  |  Inativar produtos  |
|  RF-006  |  Excluir produtos  |
|  RF-007  |  Cadastrar clientes  |
|  RF-008  |  Editar clientes  |
|  RF-009  |  Inativar clientes  |
|  RF-010  |  Excluir clientes  |
|  RF-011  |  Cadastrar fornecedores  |
|  RF-012  |  Editar fornecedores  |
|  RF-013  |  Inativar fornecedores  |
|  RF-014  |  Excluir fornecedores  |
|  RF-015  |  Emitir orçamento de compras  |
|  RF-016  |  Emitir orçamento de vendas  |
|  RF-017  |  Registrar movimento de entrada no estoque  |
|  RF-018  |  Registrar movimento de saída no estoque  |
|  RF-019  |  Cadastrar kits  |
|  RF-020  |  Editar kits  |
|  RF-021  |  Inativar kits  |
|  RF-022  |  Excluir kits  |
|  RF-023  |  Criar kits com produtos em estoque  |
|  RF-024  |  Consultar disponibilidade de produto em estoque  |
|  RF-025  |  Gerar relatório de saídas  |
|  RF-026  |  Gerar relatório de entradas  |

### Requisitos não Funcionais
|  ID	|  Descrição do Requisito	|	Prioridade  |
|  ---  |  ---  |  ---  |
|  RF-001  |  Garantir a segurança dos dados  |
|  RF-001  |  Garantir a segurança dos dados  |
|  RF-001  |  Garantir a segurança dos dados  |
|  RF-001  |  Garantir a segurança dos dados  |
|  RF-001  |  Garantir a segurança dos dados  |
