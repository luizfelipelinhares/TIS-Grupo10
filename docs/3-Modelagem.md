## 3. Modelagem do Processo de Negócio
Os processos identificados abaixo foram escolhidos para otimização por serem processos manuais repletos de retrabalho, com pouca segurança, grande margem de erro, compartilharem da mesma ferramenta (Excel) utilizada para sua execução e possuírem subprocessos comuns entre si que podem ser eliminados e otimizados através da implementação da ferramenta proposta neste trabalho.  
- **Cadastrar de produtos**
- **Emitir orçamento para compras**
- **Emitir orçamento para vendas**
- **Registrar movimento de entrada no estoque**
- **Registrar movimento de saída do estoque**
- **Verificar disponibilidade no estoque**
- **Criar Kits**

### 3.1. Modelagem da situação atual (Modelagem AS IS)
Os processos escolhidos para otimização foram modelados abaixo conforme a maneira atual de execução para que os problemas e áreas de melhoria sejam identificados, são eles:

#### Cadastrar produtos
![CadastrarProdutos](images/bpmn/1.-Cadastrar-Produtos--As-Is.png)
Disponível em: https://modeler.cloud.camunda.io/share/c8862ae1-3bd2-4f32-a023-5fe5e1a62b59

#### Emitir orçamento para compras
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/64af7abf-0015-4886-bb1e-e72ced7e4e59)

#### Emitir orçamento para vendas

Disponível em: https://modeler.cloud.camunda.io/share/435751a7-6a88-4866-8fe6-e6f30cc09402

#### Registrar movimento de entrada no estoque

Disponível em: https://modeler.cloud.camunda.io/share/de838d2d-d5db-4e7f-a9d6-23c237b016da

#### Registrar movimento de saída do estoque

Disponível em: https://modeler.cloud.camunda.io/share/9acb471b-a8f2-45aa-87bf-7aa1900ca944

#### Verificar disponibilidade no estoque

Disponível em: https://modeler.cloud.camunda.io/share/d28b60bd-eef1-4de1-9a40-1d2e28f4b8a5

#### Criar Kits

Disponível em: https://modeler.cloud.camunda.io/share/d7c86aaa-d390-4870-961c-a3917fa3442d

### 3.2. Análise dos processos
De acordo com a modelagem "As Is" dos processos acima, diversos problemas foram identificados e podem ser melhorados com a implementação da ferramenta proposta. Os principais problemas identificados foram:  

- **Segurança dos dados**  
A empresa utiliza o Excel como “base de dados” e ferramenta para a gestão do estoque, e este não possui qualquer segurança ao abrir a planilha, backup e proteção contra a exclusão do arquivo em que os dados estão armazenados.

- **Integridade das informações**  
Muitos dados ficam expostos ao abrir a planilha e ficam sujeitos a alterações indesejadas tanto em registros antigos quanto nas fórmulas da planilha que podem afetar os dados passados e futuros.

- **Concorrência**  
A planilha fica armazenada na rede do escritório e apenas uma pessoa pode utilizar a planilha por vez, e se a mesma esquecer a planilha aberta em seu computador, outra pessoa não poderá utilizar.

- **Tempo**  
Algumas atividades levam tempo demais para serem executadas e são muito repetitivas, suscetíveis a erros.

### 3.3.  Desenho dos Processos (To Be)
Após a análise dos processos e identificação das áreas de melhoria, foi feita a modelagem dos processos ("To Be") representando o uso da ferramenta proposta e evidenciando os potenciais ganhos e melhorias. Abaixo estão listadas as principais otimizações propostas pela ferramenta:

- **Segurança dos dados**  
Com uma aplicação web armazenada em nuvem, os dados ficam seguros, com backups recorrentes e protegidos contra exclusão e corrupção.

- **Integridade das informações**  
Os dados são apenas exibidos no sistema de maneira segura, sem que possam sofrer alterações a qualquer momento, e não ficam dependentes de fórmulas que podem ser alteradas por engano ou falta de conhecimento do usuário, diferente do que acontece no Excel.

- **Concorrência**  
Vários usuários podem realizar as atividades no sistema simultaneamente, resolvendo assim o problema da exclusividade de uso da planilha do Excel.

- **Tempo**  
As atividades se tornam mais rápidas e diretas pela aplicação web, onde o usuário fica livre de ter que dar manutenção em fórmulas de excel e verificar linhas disponíveis para inserção dos registros, podendo cumprir seus objetivos apenas clicando em alguns botões objetivos.


#### Cadastrar produtos
Disponível em: https://modeler.cloud.camunda.io/share/46fe3f12-68af-474a-9830-ced0e592609d

#### Emitir orçamento para compras
Disponível em: https://modeler.cloud.camunda.io/share/9ea4e7a0-de27-4dac-8c91-90f3a3ca4c70


#### Emitir orçamento para vendas
Disponível em: https://modeler.cloud.camunda.io/share/92daa343-b4a9-46fb-bc5d-ce404cf7cf4a

#### Registrar movimento de entrada
Disponível em: https://modeler.cloud.camunda.io/share/0244c5ff-7c87-4e91-ae50-23240c825bc2

#### Registrar movimento de saída
Disponível em: https://modeler.cloud.camunda.io/share/3e9f5bbc-5643-479e-9daa-7734813eb999

#### Consulta do histórico de saídas
Disponível em: https://modeler.cloud.camunda.io/share/714e0aa5-baf1-4d87-a90d-17a9dedeb886

#### Verificar estoque
Disponível em: https://modeler.cloud.camunda.io/share/0ebc45d3-bed1-4533-a1aa-cbf217308271

#### Criar kits
Disponível em: https://modeler.cloud.camunda.io/share/1b2a090d-35c2-47b5-a519-dca00eb1339a
