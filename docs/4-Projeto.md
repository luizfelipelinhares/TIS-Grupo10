## 4. Projeto da solução
Insira aqui a parte do projeto da solução


### 4.1. Tecnologias utilizadas
Optamos por utilizar prioritariamente as tecnologias, bibliotecas, softwares e frameworks da Microsoft devido a qualidade e facilidade de integração. Vamos utilizar a IDE Visual Studio Community 2022 e o projeto será desenvolvido em Blazor, um framework de desenvolvimento Web da Microsoft que permite a utilização de código C# junto ao HTML nas páginas web.  

Para o banco de dados vamos utilizar o SQL Server e para fazer a conexão com banco de dados vamos utilizar o EntityFrameworkCore junto ao ASP.NET Core, e para a autenticação e login iremos utilizar o OpenID Connect (OIDC) junto ao Microsoft Identity para permitir o login apenas de contas Microsoft, pois dessa forma aumentamos o nível de segurança ao delegar o processo de login e recuperação de senhas para a Microsoft.  

Optamos também por utilizar um framework front-end da Microsoft chamado Fluent UI para a estilização da ferramenta por possuir recursos prontos interessantes como menus e tabelas com filtros. Para a publicação da ferramenta, iremos utilizar o Azure App Services.  

### 4.2. Requisitos funcionais e não funcionais
### Requisitos Funcionais
|  ID	|  Descrição do Requisito	|
|  ---  |  ---  |
|  RF-001  |  Fazer login através de conta microsoft  |
|  RF-003  |  Cadastrar, ver, editar e excluir produtos  |
|  RF-005  |  Inativar produtos  |
|  RF-007  |  Cadastrar, ver, editar e excluir clientes  |
|  RF-009  |  Inativar clientes  |
|  RF-011  |  Cadastrar, ver, editar e excluir fornecedores  |
|  RF-013  |  Inativar fornecedores  |
|  RF-015  |  Gerar orçamento de compras  |
|  RF-016  |  Gerar orçamento de vendas  |
|  RF-017  |  Registrar movimento de entrada no estoque  |
|  RF-018  |  Registrar movimento de saída do estoque  |
|  RF-002  |  Visualizar os produtos do estoque  |
|  RF-019  |  Cadastrar kits  |
|  RF-020  |  Editar kits  |
|  RF-021  |  Inativar kits  |
|  RF-022  |  Excluir kits  |
|  RF-023  |  Criar kits com produtos em estoque  |
|  RF-024  |  Consultar disponibilidade de produto em estoque  |
|  RF-025  |  Gerar relatório de saídas  |
|  RF-026  |  Gerar relatório de entradas  |

### Requisitos não Funcionais
|  ID	|  Descrição do Requisito	|
|  ---  |  ---  |
|  RF-001  |  A ferramenta deve garantir a segurança dos dados  |
|  RF-002  |  A ferramenta deve ter uma interface simples e intuitiva  |
|  RF-003  |  A ferramenta deve ser rápida e sem congelamentos  |
|  RF-004  |  A ferramenta deve ser responsiva  |
|  RF-005  |  Os dados da ferramenta devem ser armazenados em nuvem  |
|  RF-006  |  Os dados da ferramenta devem ser armazenados em nuvem  |

### 4.3. Casos de uso
