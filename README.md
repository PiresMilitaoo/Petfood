# 1. Introdução

### 1.1. Propósito
- Fornecer um software que gerencia uma casa de ração, onde realizará serviços para o usuário durante seu horário de trabalho.
Ele será capaz de consultar, cadastrar e alterar produtos no estoque, além de emitir um relatório geral de vendas.Também será capaz de efetuar cadastro e controle de usuários.

### 1.2. Público Alvo
- Usuários internos da empresa PetFood.

### 1.3. Definições, Acrônimos e Abreviações 
- 


# 2. Descrição Geral do Produto

### 2.1. Situação Atual

 A empresa PetFood já possui um sistema de vendas no local, que atualmente apresenta os seguintes problemas: 

- Manutenção cara;
- Lentidão no sistema;
- Falha de registro de produtos;
- Falha no cadastro de usuário;
- Impossibilidade de mudar o preço;
- Falta de suporte aos usuários;
- Falha no histórico de vendas;

### 2.2. Objetivos do Produto

- A empresa PetFood solicitou o desenvolvimento de um novo software para fazer um gerenciamento total da empresa, desde o começo, meio e o fim do processo de venda. Além disso, o produto deverá solucionar os problemas apresentados no sistema anterior.
- O software tratará das pendências de logística, a fim de organizar todos os processos relacionados às vendas e o bom funcionamento da empresa.

### 2.3. Benefícios do Projeto

- Inicialização rápida;
- Facilidade no processo de vendas;
- Maior controle de entrada/saída de produtos;
- Sistema de login de usuários eficiente;
- Facilidade no processo de busca de produtos;
- Controle de vendas individuais de cada usuário;
- Manutenção mais acessível e ágil;
 
### 2.4. Escopo

### 2.5. Atores

- Funcionário (Responsável por consultar produtos e realizar as vendas)
- Gerente (Responsável por incluir, excluir e alterar os itens e os preços no estoque. Também poderá consultar produtos e realizar vendas)

<p align="center">
  <img src="https://i.imgur.com/JlrTSbB_d.webp?maxwidth=760&fidelity=grand" alt="Relação de hierarquia entre gerente e funcionário"></a>
</p>


### 2.6. Premissas

### 2.7. Itens fora do Escopo


# Requisitos Específicos

### 3.1. Requisitos Funcionais 

- RF01 - O sistema deverá solicitar ao usuário seu login e senha e verificar se o mesmo possui permissão de acesso ao sistema
- RF02 - O sistema deve permitir a criação, exclusão e alteração dos itens no estoque
- RF03 - O sistema deve armazenar o histórico de vendas, incluindo o valor total, usuário responsável e a data
- RF04 - O sistema deve permitir consultar e alterar o preço dos produtos cadastrados

### 3.2. Requisitos não Funcionais

- RNF01 - O sistema rodará no Windows (Operacional)
- RNF02 - O sistema será de linguagem simples e acessível. (Usabilidade)
- RNF03 - Somente usuários cadastrados terão acesso. (Segurança)
- RNF04 - O sistema deverá inicializar em menos de dois minutos. (Desempenho)

### 3.4. Regras de negocios
- RN01 - Alteração dos produtos (Somente será permitida alterações se o usuário logado for um gerente).
- RN02 - Movimentação de estoque (Só poderá ser feito a venda de um item se houver uma quantidade equivalente no estoque).
- RN03 - Cadastro de usuários (Será permitido cadastro de usuário somente se o usuário logado for um gerente).
- RN04 - Consulta do relatório geral de vendas (Será permitido consultas ao relatório geral de vendas somente se o usuário logado for um gerente).


### 3.4. Restrições de Hardware
- Mínimo de 8GB de memória RAM.
- Necessário um SSD para a locação/armazenamento do sistema e base de dados.


### 3.5. Restrições de Software
- Será permitida a utilização somente no sistema Windows.


### 3.6. Restrições de Ambiente
- O acesso ao sistema será apenas em ambiente local.

### 3.7. Lista de riscos 


# 4. Diagramas UML

### 4.1. Identificação dos Casos de Uso

### 4.2. Diagramas de Casos de Uso

### 4.3. Diagrama de Atividades

### 4.4. Diagrama de Classes

### 4.5. Diagrama de Objetos

### 4.6. Diagrama de Sequência 

### 4.7. Diagrama de Estados


# 5. Apêndice

# 6. Aprovação

# Histórias de usuário

## Histórias de usuário Funcionário/Gerente

### História 1 - Entrando no sistema

- Como funcionário/gerente quero colocar as minhas informações (login, senha) para entrar no sistema

### Critério de aceitação 

- Campo para colocar o usuário
- Campo para colocar a senha
- Campo esqueci a senha

### História 2 - Menu do sistema

- Como funcionário/gerente , após o login , observo o menu do sistema , para que possa prosseguir a uma funcionalidade do sistema.

### Critério de aceite

- Campo para vendas
  - Caso o usuário seja um funcionário, será automaticamente redirecionado para o campo de vendas
- Campo para cadastro de usuários (exclusivo para o gerente)
- Campo para estoque (exclusivo para o gerente)
- Campo para financeiro (exclusivo para o gerente)

### História 3 - Campo de vendas

- Como funcionário/gerente quero entrar na aba de vendas para vender/pesquisar um produto

### Critério de aceite

- Tela de pré-venda
- Campo com a lista de produtos escolhidos
- Campo com as formas de pagamento (dinheiro, cartão, pix)
- Campo para cancelar pré-venda
  - Caso escolha a opção cancelar pré-venda, todos os produtos escolhidos sairão da pré-venda
- Campo para cancelar um produto
  - Caso escolha a opção cancelar um produto, será permitido a escolha de um produto para ser retirado da pré-venda 
- Campo para pesquisa de produtos
  - Caso escolha o campo de pesquisa de produtos, aparecerá uma lista completa dos produtos e uma aba para pesquisar um produto específico
- Campo para categorias de produtos
  - Caso escolha o campo de categorias de produtos, aparecerá 4 campos
    - Campo Alimentícios, Campo medicamentos, Campo brinquedos, Campo acessórios



### História 4 - Consultando produtos

- Como funcionário/gerente quero pesquisar um produto da loja para obter informações sobre ele

### Critério de aceitação 

- Tela de pré-venda (Campo vendas)
- Atalho/Botão para categoria de produto
  - Ao escolher esse campo será redirecionado para as categorias (alimentícios, medicamentos, brinquedos, acessórios)
     - Após escolher uma categoria, aparecerá uma lista com apenas produtos da categoria escolhida
- Atalho/Botão para pesquisa de um produto 
  - Ao escolher esse campo, aparecerá uma lista com todos os produtos(com barra de rolagem) e um campo para pesquisar um produto específico

### História 5 - Escolhendo o produto

- Como funcionário/gerente quero escolher um produto da loja para encaminhá-lo à pré-venda

### Critério de aceitação

- Tela de pré-venda (Campo vendas)
- Atalho/Botão para pesquisar um produto
- Lista com os produtos
 


### História 6 - Vendendo um produto

- Como funcionário/gerente quero escolher um produto para realizar a venda do mesmo
  
### Critério de aceitação
- Campo com a lista de produtos
  - Após selecionar o produto, escolherá a quantidade que será vendida, após isso, o produto será redirecionado para a pré-venda
- Produtos com quantidades zeradas não serão encaminhados para a pré-venda e aparecerá uma mensagem na tela:
  - ''O produto não pode ser vendido pois não há quantidade no estoque''
- Campo com a lista de produtos escolhidos , onde é mostrado nome, preço e quantidade
- Campo com forma de pagamento
- Não permite vendas com quantidades que ultrapassam o estoque
- Campo com a confirmação de valor, quantidade e forma de pagamento

  
## Histórias de usuário Gerente (Exclusivo)

### História 5 - Adicionando um produto

- Como gerente quero adicionar um produto ao sistema

### Critério de aceitação

- Campo para pesquisa de produtos
- Campo com um (+) para adicionar produtos
- Campo onde será inserido o nome
- Campo onde será inserido o preço
- Campo onde será inserido a quantidade
- Campo onde será inserido o NCM
- Campo onde será inserido o código de barras
- Campo para confirmação de dados
- Mensagem produto adicionado com sucesso

### História 6 - Alterando preço de um produto

- Como gerente quero alterar o preço de um produto

### Critério de aceitação

- Campo para pesquisa de produtos
- Campos com as informações do produto
- Campo com o preço
- Campo com a confirmação da alteração do produto
- Mensagem produto alterado com sucesso

### História 7 - Alterando quantidade de um produto

- Como gerente quero alterar a quantidade de um produto

### Critério de aceitação

- Campo para pesquisa de produtos
- Campos com as informações do produto
- Campo com a quantidade
- Campo com a confirmação da alteração do produto
- Mensagem produto alterado com sucesso

### História 8 - Excluindo um produto

- Como gerente quero excluir um produto

### Critério de aceitação

- Campo para pesquisa de produtos
- Campos com as informações do produto
- Campo com um (x) para excluir um produto
- Campo com a confirmação da exclusão do produto
- Mensagem produto excluído com sucesso


