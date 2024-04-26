# projeto2-bd1

O projeto descrito envolve a criação de um sistema de banco de dados complexo, destinado a gerenciar uma série de informações relacionadas a um negócio de varejo, potencialmente focado em vendas de livros e artigos de papelaria. O sistema é projetado para armazenar e manipular dados sobre clientes, endereços, pedidos, pagamentos, produtos e autores, oferecendo uma estrutura integrada para operações comerciais eficientes. Aqui está uma descrição mais detalhada das características e funcionalidades deste sistema de banco de dados:

### Objetivo
O objetivo principal do sistema é facilitar o gerenciamento de todas as etapas das transações comerciais, desde o registro de clientes até a finalização de compras e pagamentos, incluindo o gerenciamento de inventários de produtos específicos como livros e artigos de papelaria.

### Estrutura de Dados
- **Clientes**: A tabela `cliente` armazena informações pessoais e de contato dos clientes, incluindo nome, sobrenome, telefone, email e CPF. Essas informações são cruciais para o processo de venda e para comunicação com o cliente.
  
- **Endereços**: A tabela `endereco` lida com os detalhes de endereçamento dos clientes, conectando cada endereço ao respectivo cliente por meio de uma chave estrangeira. Isso é essencial para processos como a entrega de produtos.

- **Pedidos**: A tabela `pedido` registra detalhes dos pedidos feitos pelos clientes, incluindo a data do pedido e o valor total, vinculados ao cliente que fez o pedido. Esta tabela é a base para o gerenciamento de transações de vendas.

- **Pagamentos**: A tabela `pagamento` monitora os detalhes dos pagamentos de cada pedido, especificando a forma de pagamento, a data do pagamento e a validade do pagamento, relacionando-o ao pedido correspondente.

- **Carrinho**: A tabela `carrinho` detalha os itens comprados em cada pedido, incluindo a quantidade de produtos e o preço por item, permitindo a análise de vendas detalhada e gerenciamento de estoque.

- **Papelaria**: A tabela `papelaria` gerencia um inventário de produtos de papelaria, especificando nome, tipo, marca e quantidade em estoque.

- **Livros**: A tabela `livro` mantém um registro de livros disponíveis, com informações sobre avaliações, títulos, datas de publicação, descrições e quantidades em estoque.

- **Autores**: A tabela `autor` associa autores a livros, permitindo uma gestão detalhada dos direitos autorais e promoções de livros baseadas em autores específicos.

### Funcionalidades
- **Gestão de Clientes e Endereços**: Permite um registro detalhado e atualizações de informações dos clientes e seus endereços para facilitar a entrega e a comunicação.
- **Processamento de Pedidos**: Automatiza a criação de pedidos, acompanhamento e finalização das vendas.
- **Gerenciamento de Pagamentos**: Controla as formas e eficácia dos pagamentos, assegurando a precisão financeira.
- **Administração de Estoque**: Gerencia o estoque de produtos, ajudando a evitar excessos ou faltas e facilitando a reposição.
- **Relacionamento de Dados**: Utiliza chaves estrangeiras para manter a integridade referencial entre tabelas, garantindo que as operações de dados entre diferentes seções do banco sejam precisas e confiáveis.

### Benefícios
- **Integração**: Todas as partes do processo de vendas estão integradas em um único sistema, facilitando o acesso e a gestão.
- **Eficiência Operacional**: A automatização de tarefas reduz a necessidade de intervenção manual, aumentando a eficiência.
- **Confiabilidade**: A manutenção da integridade dos dados ajuda a garantir que as informações sejam precisas e confiáveis.
