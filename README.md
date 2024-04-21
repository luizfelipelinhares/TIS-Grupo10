# TIS - Grupo 10: Controle de Estoque L&R Kits e Freios

## Integrantes
- Luiz Felipe Linhares Vieira (lzfdev@gmail.com)
- Henrique Taite Mendes (henriquetaite@gmail.com)
- Nathan Filipe Carvalho Cota (nathancarvalhocota@gmail.com)
- Bruno Alexandre Anastácio De Almeida (brunoanastacio07@gmail.com)

**Instituto de Informática e Ciências Exatas – Pontifícia Universidade Católica de Minas Gerais (PUC MINAS)  
Belo Horizonte – MG – Brasil**

## Resumo 
*A empresa L&R Kits e Freios é uma pequena distribuidora de peças e kits para freios de caminhão, e estes últimos são montados pela própria organização com as peças que têm em estoque. Para fazer os cadastros e emissão de orçamentos para seus clientes, a L&R utiliza o programa Excel que possui certas limitações, que não deixam o serviço tão efetivo quanto poderia ser, além de não possuir qualquer nível de segurança, assim sendo muito suscetível a erros manuais dos usuários.
Diante disso, consideramos viável e muito útil criar um projeto de uma aplicação WEB para gerenciar o controle de estoque e geração de orçamentos, de forma otimizada e segura, além de trazer outras possíveis funções e benefícios para a organização em questão. Será possível emitir orçamentos e fazer o controle de estoque com mais agilidade, segurança e efetividade.*

## 1. Introdução
De acordo com artigo do site https://www.mindtek.com.br/, em 2022, 90% das empresas ainda utilizavam o Excel como ferramenta para realizar orçamentos, planejamentos e previsões de operações. Muito disso provavelmente se deve ao fato de ser um programa tradicional e pouco oneroso. No entanto, por mais que o Excel apresente uma infinidade de recursos, existem meios mais eficientes e completos de se realizar as atividades de planejamento, orçamentos e controles em geral de uma empresa. 
Segundo artigo do site https://gdoor.com.br/, o Excel possui as seguintes limitações/problemas: exige atualização manual constante, atrasando o trabalho; é muito vulnerável à ataques; não têm recursos para armazenar e integrar uma quantidade grande de dados; não integra os setores da organização, ou seja, não existe a propriedade de concorrência para controlar atualização do documento; vulnerabilidade à perda de dados.
Distribuidora de pequeno porte, a L&R Kits e Freios é uma das organizações que ainda utiliza o Excel como ferramenta para fazer os seus controles habituais. Diante de todas as características descritas sobre o Excel anteriormente, que são razões para que o mesmo seja substituído por um novo programa, viemos com a proposta de criar uma aplicação WEB a ser implementada na L&R. 
A aplicação será capaz de emitir orçamentos e fazer controle de estoque da distribuidora com mais flexibilidade e segurança, além de tornar possível cadastrar produtos, cadastrar movimentos de entrada e saída e gerar relatórios, tudo isto em uma ferramenta mais otimizada e segura que o Excel. Por fim, é essencial que esta criação seja capaz de não apresentar as mesmas limitações/problemas do Excel, tornando os processos mais eficientes, a empresa mais sólida e competitiva no mercado.

### 1.1. Objetivos geral e específicos
O objetivo geral do projeto é desenvolver uma aplicação web para otimizar os processos de controle de estoque, emissão de orçamentos e melhorar a segurança dos dados da L&R Kits e Freios, uma pequena distribuidora de peças de freios de caminhão.
Dentre os objetivos específicos, tem-se:
Desenvolver uma aplicação web de interface simples e intuitiva, hospedada na nuvem para assegurar a disponibilidade, integridade e segurança dos dados do estoque da empresa e prevenir erros de operação dos usuários.
Otimizar a geração de pedidos e orçamentos, fazendo a devida integração com o banco de dados do estoque. 

### 1.2. Justificativas
Com a evolução da tecnologia, muitos empreendedores pequenos não conseguem acompanhar as novas ferramentas e soluções para otimização de suas atividades. Diante disso, é necessário a utilização de novos mecanismos para acompanhar a evolução e velocidade do mercado, se adequando às novas tendências. O projeto é necessário para otimizar e melhorar o processo da loja, através da criação de uma nova ferramenta que irá gerir e controlar todas as informações de uma forma mais prática, rápida e segura, sem as limitações do modelo utilizado anteriormente.  

## 2. Participantes do processo de negócio
Os processos do negócio são realizados pelo dono da empresa, pelos funcionários dos setores administrativo, almoxarifado e vendas, e os processos mapeados foram:

### Compra de mercadorias
A compra de mercadorias é um processo de suporte e garante que o estoque esteja sempre abastecido. O processo ocorre da seguinte maneira:

1. **Contato com o fornecedor e solicitar do orçamento**  
O funcionário do administrativo entra em contato com o fornecedor e envia um orçamento das mercadorias que pretende comprar.

2. **Negocias os preços**  
O funcionário administrativo negocia o preço das mercadorias com o fornecedor.

3. **Confirmar compra**  
O funcionário do administrativo confirma a compra e realiza o pedido com o fornecedor.

4. **Receber mercadorias**  
A funcionária do almoxarifado recebe, contabiliza, e armazena as mercadorias recebidas no estoque.

5. **Registrar entrada no estoque**  
O funcionário do setor administrativo registra a entrada das mercadorias na aba “Registro de movimentos” da planilha “Controle de Estoque” no Excel.

### Venda de mercadorias
A venda de mercadorias é um processo primário e a fonte de receita de toda a empresa. O processo ocorre da seguinte maneira:

1. **Contato do cliente com a funcionária do setor de vendas**  
O cliente entra em contato com o setor de vendas por meio de email, Whatsapp ou telefone, solicitando um orçamento das mercadorias.

2. **Verificar a disponibilidade no estoque**  
A funcionária do setor de vendas verifica a disponibilidade e o preço das mercadorias no estoque através de uma planilha no Excel e gera o orçamento solicitado pelo cliente por meio da mesma planilha, utilizando um macro VBA.

3. **Emitir o orçamento**  
A funcionária do setor de vendas gera o orçamento solicitado pelo cliente por meio de uma planilha no excel, utilizando um macro VBA.

4. **Confirmar o pedido**  
O cliente confirma o pedido e o meio de entrega.

5. **Separar as mercdorias**  
A funcionária do almoxarifado separa e embala as mercadorias para a coleta da transportadora.

6. **Registrar saída do estoque**  
Após a confirmação do pedido e separação das mercadorias, o funcionário administrativo realiza o registro do movimento de saída na aba “Registro de movimentos” da planilha “Controle de Estoque” no Excel.

### Gerenciamento e monitoramento do estoque
O monitoramento de estoque é um processo gerencial importante para garantir a disponibilidade das mercadorias no estoque e evitar compras desnecessárias. O gerenciamento do estoque na empresa é feito através de uma planilha no Excel. O processo é realizado pelo dono da empresa e pelo funcionário do administrativo, e compreende os seguinte subprocessos:

1. **Cadastrar produtos**  
O dono da empresa ou funcionário do administrativo registra novos produtos na aba “Estoque” da planilha “Controle de Estoque” no Excel para habilitar futuras entradas e saídas na aba “Registro de Movimentos”.

2. **Criar kits**  
A funcionária do almoxarifado separa Kits com as mercadorias disponíveis no estoque, e então o funcionário do setor administrativo registra o movimento de entrada dos Kits no estoque na aba “Registro de movimentos” da planilha “Controle de Estoque” no Excel, ao mesmo tempo que registra o movimento de saída das mercadorias utilizadas para montar o Kit.

3. **Verificar o estoque**  
O dono da empresa e o funcionário do setor administrativo monitoram a quantidade de mercadorias disponíveis no estoque, utilizando a aba “Estoque” da planilha “Controle de Estoque” no Excel para verificar se é necessário abastecer o estoque.

## 3. Modelagem do Processo de Negócio
Os processos identificados abaixo foram escolhidos para otimização por serem processos manuais repletos de retrabalho, com pouca segurança, grande margem de erro, compartilharem da mesma ferramenta (Excel) utilizada para sua execução e possuírem subprocessos comuns entre si que podem ser eliminados e otimizados através da implementação da ferramenta proposta neste trabalho.  
- Cadastrar de produtos
- Emitir orçamento para compras
- Emitir orçamento para vendas
- Registrar movimento de entrada no estoque
- Registrar movimento de saída do estoque
- Verificar disponibilidade no estoque
- Criar Kits

### 3.1. Modelagem da situação atual (Modelagem AS IS)

#### Cadastrar produtos
Disponível em: https://modeler.cloud.camunda.io/share/c8862ae1-3bd2-4f32-a023-5fe5e1a62b59

#### Emitir orçamento para compras
Disponível em: https://modeler.cloud.camunda.io/share/64af7abf-0015-4886-bb1e-e72ced7e4e59

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
**Não conformidades gerais**

- **Segurança dos dados** 
A empresa utiliza o Excel como “base de dados” e ferramenta para a gestão do estoque, e este não possui qualquer segurança ao abrir a planilha, backup e proteção contra a exclusão do arquivo em que os dados estão armazenados.

- **Integridade das informações**
Muitos dados ficam expostos ao abrir a planilha e ficam sujeitos a alterações indesejadas tanto em registros antigos quanto nas fórmulas da planilha que podem afetar os dados passados e futuros.

- **Concorrência**
A planilha fica armazenada na rede do escritório e apenas uma pessoa pode utilizar a planilha por vez, e se a mesma esquecer a planilha aberta em seu computador, outra pessoa não poderá utilizar.

- **Tempo**
Algumas atividades levam tempo demais para serem executadas e são muito repetitivas, suscetíveis a erros.

### 3.3.  Desenho dos Processos (To Be)
Os processos abaixo foram modelados novamente representando o uso da ferramenta proposta para resolver as não conformidades descritas no tópico acima:

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