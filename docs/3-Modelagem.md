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
![CadastrarProdutos](images/bpmn/(As-Is)-1-Cadastrar-Produtos.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/70a327f8-1d79-4068-a80b-7f348e93504d)

#### Registrar movimento no estoque
![CadastrarProdutos](images/bpmn/(As-Is)-2-Registrar-movimento-no-estoque.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/b060fecb-8e28-41b6-bc2d-dcb4a71d2b13)

#### Verificar disponibilidade no estoque
![CadastrarProdutos](images/bpmn/(As-Is)-3-Verificar-disponibilidade-no-estoque.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/2e4803af-2fe1-4ba3-8b2e-b94c8032bf88)

#### Gerar orçamento
![CadastrarProdutos](images/bpmn/(As-Is)-4-Gerar-orçamento.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/3319ae55-4aa2-4659-9530-3c96c93719a9)

#### Verificar as fórmulas da planilha
![CadastrarProdutos](images/bpmn/(As-Is)-5-Verificar-as-formulas-da-planilha.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/9db1e703-689d-45a3-b39f-feb583207d54)

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
![CadastrarProdutos](images/bpmn/(To-Be)-1-Cadastrar-Produtos.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/9c55d229-329e-4f8e-96cc-c29c2e12ec29)

#### Cadastrar fornecedores
![CadastrarProdutos](images/bpmn/(To-Be)-2-Cadastrar-Fornecedores.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/a49c3f41-1cff-4eb2-b77c-5b7e12ed06aa)

#### Cadastrar clientes
![CadastrarProdutos](images/bpmn/(To-Be)-3-Cadastrar-Clientes.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/c710523f-2b9f-4fc8-844f-1a489c649766)

#### Registrar movimento no estoque
![CadastrarProdutos](images/bpmn/(To-Be)-4-Registrar-movimento-no-estoque.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/ac965f2f-c3f7-4a00-a83f-855b1a4ff396)

#### Verificar disponibilidade no estoque
![CadastrarProdutos](images/bpmn/(To-Be)-5-Verificar-disponibilidade-no-estoque.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/b07e6266-5268-4a09-92f7-6fd8510b7ca2)

#### Gerar orçamento
![CadastrarProdutos](images/bpmn/(To-Be)-6-Gerar-orçamento.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/a9d8adeb-42a0-40a5-bba9-4dd1445e7a08)

#### Gerar Relatório
![CadastrarProdutos](images/bpmn/(To-Be)-7-Gerar-relatório.png)
Disponível online em: [Camunda](https://modeler.cloud.camunda.io/share/ff3c69fa-d6ec-4ecc-9732-b5521eee0a7d)
