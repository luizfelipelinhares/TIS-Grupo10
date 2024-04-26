## 4. Projeto da solução
  Atualmente a empresa L&R Kits e Freios utiliza o Excel como a principal plataforma para operações e gerenciamentos de várias atividades. Tendo em vista que esta ferramenta é limitada e que é possível implementar meios mais efetivos de trabalho através de um programa mais robusto, nosso objetivo macro neste projeto é criar esta possibilidade para o estabelecimento em questão.  
	Em primeiro lugar, podemos identificar um problema de concorrência, considerando o modelo AS IS de todos os processos da L&R. Isto porque não é possível trabalhar em um determinado campo do Excel sem que haja uma tarefa manual de verificação prévia para saber se algum colaborador está trabalhando no programa. Caso alguém já esteja usando a ferramenta, o outro deve esperar pois, se mais de um integrante operar ao mesmo tempo, há grandes chances do documento ser salvo sem todas as modificações que deveriam ser feitas.  
	Levando em conta a modelagem TO BE, este problema de uso exclusivo do Excel por um trabalhador é eliminado com o uso do novo programa, ERP – L&R, que está sendo proposto no projeto. Este será capaz de permitir que um número grande de pessoas opere simultaneamente, extinguindo a necessidade de fazer o colaborador perder tempo verificando se o programa já se encontra em uso e ainda de aguardar esta tarefa terminar.  
	No quesito segurança dos dados, o fato do programa ser armazenado em nuvem de forma eficiente vai ajudar tanto na não conformidade de concorrência quanto na de segurança de acesso aos dados e documentos da L&R. O fato do Excel não possuir um sistema completo de backups recorrentes e proteção contra exclusão e corrupção faz com que o estado atual da empresa seja de possuir um sistema de trabalho vulnerável. No entanto, esta fragilidade será resolvida com a proposta de implementar em nossa aplicação web um armazenamento em nuvem que deixe os dados seguros e tenha backups pontuais que protejam a empresa de qualquer violação.  
	Analisando os processos no modelo AS IS, podemos perceber que são processos simples porém demorados, devido algumas limitações do Excel que são: falta de integridade em seus registros, onde fórmulas ou disposições importantes podem ser alteradas a qualquer momento, até mesmo acidentalmente; pouca usabilidade, pois é necessário conhecimento avançado para fazer fórmulas corretas e criar dinamicidade no fluxo de trabalho desta ferramenta.  
	A partir dos problemas de desperdício de tempo identificados no parágrafo anterior, pensamos no ERP – L&R como uma solução que deixaria o fluxo de trabalho da L&R muito mais dinâmico, fluido e fácil. Portanto, a nova ferramenta apresentaria: alta usabilidade, exigindo apenas que o usuário leia o botão com linguagem simples e objetiva, faça uma interpretação e use-o de acordo com a sua demanda; simplificação no uso dos comandos, pois as fórmulas e demais cálculos necessários ficariam prontos como requisitos não funcionais, eliminando qualquer necessidade do usuário gastar tempo para aprender a usar estes recursos; alta integridade nos registros, já que o fluxo mais simples que não necessite da inserção de fórmulas e cálculos deixa estes métodos seguros o suficiente para não serem alterados a qualquer momento.     


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
